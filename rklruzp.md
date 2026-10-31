代发 wailian999

Py:   isinstance(u, User)
来源：http://ch.shxzskj.cn

PHP:  $u instanceof User
来源：http://es.haigaiapp.cn

JS:   u instanceof User
来源：http://nf.shxzskj.cn

TS:   u instanceof User
来源：http://pq.haigaiapp.cn

Java: u instanceof User
来源：http://vi.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ff.szsharing.cn

Ruby: u.is_a?(User)
来源：http://yi.chemitech.net.cn

C#:   u is User
来源：http://uo.gzmigu.cn

[G14] 数据类 / record
来源：http://iw.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yw.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://lr.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://um.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://kh.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://su.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://pi.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jk.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://rp.chemitech.net.cn

[G15] 枚举
来源：http://ni.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hm.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://du.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fo.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pm.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://qp.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wn.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://ft.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xs.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://bw.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zu.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://sk.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://nb.colortex.cn

TS:   Object.entries(obj)
来源：http://gc.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mg.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ey.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://pf.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://uy.yuexingan06.cn

================================================================================
来源：http://uq.nszjky.cn

H. 异常与错误处理
来源：http://yl.bookmarksfly.cn

================================================================================
来源：http://iv.jctech888.com.cn

[H01] try / catch 基础
来源：http://hi.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jc.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fe.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://la.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kl.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tg.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gq.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dm.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jx.huanxung.cn

[H02] finally / ensure 收尾
来源：http://iv.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zx.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ux.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nh.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ci.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ez.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bm.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ky.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dt.colortex.cn

[H03] 主动抛出异常
来源：http://tz.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://ob.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dv.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://nn.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://rf.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jl.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ul.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yx.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qe.colortex.cn

[H04] 自定义异常类型
来源：http://vh.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://uf.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://md.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://kk.szsharing.cn

TS:   class MyError extends Error {}
来源：http://fb.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ea.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://je.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://rj.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://mx.hahajie.cn

[H05] 捕获特定类型
来源：http://vu.yuexingan06.cn

Py:   except ValueError as e:
来源：http://jg.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wq.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://of.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://ko.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://ow.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qm.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://ud.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dl.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://be.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://at.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vs.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lp.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://se.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://is.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xx.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://pf.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://lh.muxihuayi.cn

[H07] 断言
来源：http://us.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://zs.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://qv.hahajie.cn

JS:   console.assert(x > 0);
来源：http://it.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://qz.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://uj.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dq.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iy.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://nc.521024.cn

[H08] 获取错误信息与堆栈
来源：http://pa.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://de.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xi.nicolike.cn

JS:   e.message;  e.stack
来源：http://pn.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tb.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://da.huixinmuqiang.cn

Go:   err.Error()
来源：http://ta.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://po.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://ea.shxzskj.cn

[H09] 带错误码的异常
来源：http://jg.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mc.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hg.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qp.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dy.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ec.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://on.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nt.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ua.huanxung.cn

[H10] 资源自动释放
来源：http://cg.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dc.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zw.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hh.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qq.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hy.wgjwhj.cn

Go:   defer f.Close()
来源：http://ve.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://up.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bg.9csxet.cn

================================================================================
来源：http://mn.bookmarksfly.cn

I. 正则表达式
来源：http://ur.newstarts.cn

================================================================================
来源：http://lu.bjjhwx.cn

[I01] 判断是否匹配
来源：http://eo.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ei.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uf.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://nb.nicolike.cn

TS:   /\d+/.test(s)
来源：http://pw.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vh.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tw.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://qy.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rq.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://kg.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://hp.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kw.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eu.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://lt.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zm.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hi.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://ho.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oo.colortex.cn

[I03] 提取捕获分组
来源：http://oa.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://md.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://se.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kc.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cy.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ul.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fl.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://by.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sr.chemitech.net.cn

[I04] 正则替换
来源：http://mj.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cq.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kk.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tj.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://th.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ir.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cu.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mp.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zk.newstarts.cn

[I05] 按正则拆分
来源：http://tk.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rh.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mp.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://vr.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://wb.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://ot.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cv.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://da.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wp.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://di.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ks.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ph.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://no.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dw.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ew.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ys.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dc.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ss.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://ja.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://un.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tu.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iz.asd995.cn

TS:   /error/gim
来源：http://yd.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ga.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://la.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://lx.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://st.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://hr.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gk.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bc.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cl.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://it.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ir.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ai.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cv.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ry.9csxet.cn

================================================================================
来源：http://re.9csxet.cn

J. 日期与时间
来源：http://pz.asd995.cn

================================================================================
来源：http://rn.bjjhwx.cn

[J01] 获取当前时间
来源：http://op.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mg.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://av.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://nf.colortex.cn

TS:   new Date();  Date.now()
来源：http://ic.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fm.bookmarksfly.cn

Go:   time.Now()
来源：http://gy.muxihuayi.cn

Ruby: Time.now
来源：http://en.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mh.huixinmuqiang.cn

[J02] 格式化输出
来源：http://ge.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ez.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uu.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ac.haigaiapp.cn

TS:   d.toISOString()
来源：http://uv.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pp.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ns.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uv.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hi.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://vb.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ld.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ru.colortex.cn

JS:   new Date("2024-01-02")
来源：http://yg.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://xx.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bp.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rr.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ge.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://so.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://vh.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oz.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lj.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ax.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fe.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jh.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qm.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eh.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vb.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://qk.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://hm.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ws.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ms.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://od.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://js.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xm.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://av.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qm.muxihuayi.cn

[J06] 计算两时间之差
来源：http://fg.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://cp.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://ry.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gg.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ct.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dn.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://ef.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://bq.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://gc.521024.cn

[J07] 比较两个日期
来源：http://me.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ns.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uy.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nj.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tf.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tt.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tx.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fc.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://ex.521024.cn

[J08] 提取年月日与星期
来源：http://cp.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bl.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fm.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wg.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ky.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zm.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nq.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rt.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lo.yuntaijiaju.cn

[J09] 时区处理
来源：http://nv.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hg.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ou.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qq.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bm.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lm.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gt.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yz.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ed.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://uh.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ii.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mb.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vz.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kq.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yw.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ro.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wk.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gw.shxzskj.cn

================================================================================
来源：http://zl.chemitech.net.cn

K. JSON 与序列化
来源：http://fv.haigaiapp.cn

================================================================================
来源：http://di.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://uk.yuntaijiaju.cn


<!-- 参考信息 -->