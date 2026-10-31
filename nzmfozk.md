代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://zx.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://be.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://kh.muxihuayi.cn

[G13] 判断对象类型
来源：http://hf.9csxet.cn

Py:   isinstance(u, User)
来源：http://qb.muxihuayi.cn

PHP:  $u instanceof User
来源：http://nc.hnjuh.cn

JS:   u instanceof User
来源：http://ov.muxihuayi.cn

TS:   u instanceof User
来源：http://ok.yuexingan06.cn

Java: u instanceof User
来源：http://xc.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qg.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://gz.yuntaijiaju.cn

C#:   u is User
来源：http://hf.lnxyls.cn

[G14] 数据类 / record
来源：http://fd.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ma.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://na.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://so.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://rj.hahajie.cn

Java: record User(String name, int age) {}
来源：http://co.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://ue.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://va.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://bc.jianghongdianzi.cn

[G15] 枚举
来源：http://lj.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hd.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bh.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ac.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hl.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://we.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rq.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://gj.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tu.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://ab.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bp.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://wj.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://qi.nicolike.cn

TS:   Object.entries(obj)
来源：http://iz.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wv.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ca.colortex.cn

Ruby: obj.instance_variables
来源：http://hl.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://hn.bjjhwx.cn

================================================================================
来源：http://co.gzmigu.cn

H. 异常与错误处理
来源：http://zt.wgjwhj.cn

================================================================================
来源：http://ua.shxzskj.cn

[H01] try / catch 基础
来源：http://va.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oh.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ru.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oy.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pk.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ri.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ae.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jx.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uy.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://nw.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pm.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mw.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ec.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kk.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sz.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nd.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bi.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eh.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://jq.521024.cn

Py:   raise ValueError("错误信息")
来源：http://oj.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ch.colortex.cn

JS:   throw new Error("错误信息");
来源：http://dt.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://kx.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qw.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hc.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ew.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tk.wgjwhj.cn

[H04] 自定义异常类型
来源：http://pj.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://ya.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://he.9csxet.cn

JS:   class MyError extends Error {}
来源：http://rz.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://jt.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://gf.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pu.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://zn.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://ek.gzmigu.cn

[H05] 捕获特定类型
来源：http://tr.muxihuayi.cn

Py:   except ValueError as e:
来源：http://tv.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tb.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://az.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://jz.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://oi.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eo.521024.cn

Ruby: rescue ArgumentError => e
来源：http://wm.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ln.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://cb.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://zz.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tm.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ox.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ny.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rz.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kk.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://he.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://jt.lnxyls.cn

[H07] 断言
来源：http://xw.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://cc.hnjuh.cn

PHP:  assert($x > 0);
来源：http://qo.nszjky.cn

JS:   console.assert(x > 0);
来源：http://tb.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://ug.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://kt.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nx.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vs.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://lb.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://pb.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://bq.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nh.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://ju.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qx.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://st.huanxung.cn

Go:   err.Error()
来源：http://uk.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://qd.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://gu.huixiangedu.cn

[H09] 带错误码的异常
来源：http://tu.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fi.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gi.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ys.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lq.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mr.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rv.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sf.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cu.nszjky.cn

[H10] 资源自动释放
来源：http://us.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lr.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pk.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qs.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hi.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mv.chemitech.net.cn

Go:   defer f.Close()
来源：http://uz.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://do.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vg.szxytkj.cn

================================================================================
来源：http://ss.haigaiapp.cn

I. 正则表达式
来源：http://bp.521024.cn

================================================================================
来源：http://ez.chemitech.net.cn

[I01] 判断是否匹配
来源：http://zo.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ib.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fp.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://ca.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://pk.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gl.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eg.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://hv.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pt.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ht.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://mf.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ix.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lh.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://wt.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://us.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://om.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://jv.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ki.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://un.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pv.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wz.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zl.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://he.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://op.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dw.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pb.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://un.9csxet.cn

[I04] 正则替换
来源：http://bm.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yu.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fy.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yt.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://th.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ee.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vy.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cs.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xb.shxzskj.cn

[I05] 按正则拆分
来源：http://vi.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ys.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bz.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://tq.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://ln.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://hx.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uh.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vi.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ja.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pn.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gv.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bl.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oh.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hm.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://we.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ge.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qm.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jc.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://qy.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nt.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yv.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dp.jctech888.com.cn

TS:   /error/gim
来源：http://fx.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hd.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dv.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://rb.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ir.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://jk.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wu.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hk.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cq.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tf.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wa.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://za.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xm.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://si.huanxung.cn

================================================================================
来源：http://hr.jianghongdianzi.cn

J. 日期与时间
来源：http://si.gzmigu.cn

================================================================================
来源：http://ov.nszjky.cn

[J01] 获取当前时间
来源：http://ev.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://an.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uu.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://mb.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://zk.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zv.huixinmuqiang.cn

Go:   time.Now()
来源：http://di.panjiajie.cn

Ruby: Time.now
来源：http://zn.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sc.yuntaijiaju.cn

[J02] 格式化输出
来源：http://gf.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tl.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cx.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dx.colortex.cn

TS:   d.toISOString()
来源：http://mi.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qk.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vt.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://le.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cg.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://ad.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://po.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uw.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://qi.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://wo.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tr.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jp.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://le.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dj.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://uf.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hu.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wk.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zj.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wy.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kt.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dl.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iu.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rp.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://of.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://rr.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dt.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tg.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bk.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://sd.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uk.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://ch.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://is.bjjhwx.cn

[J06] 计算两时间之差
来源：http://vv.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://bw.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://uf.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xj.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ok.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yr.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://vc.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://js.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://lw.muxihuayi.cn

[J07] 比较两个日期
来源：http://wy.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://hy.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dh.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fz.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jw.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bf.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jf.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oe.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://jz.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://gf.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://st.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xm.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gr.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vg.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fv.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ly.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hx.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wa.newstarts.cn

[J09] 时区处理
来源：http://ng.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pz.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ot.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zz.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zy.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pc.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://up.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ra.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ms.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://xs.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yz.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lp.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ws.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://as.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vn.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cf.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pa.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zy.nszjky.cn


<!-- 参考信息 -->