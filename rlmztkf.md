代发 wailian999

Ruby: attr_accessor :name
来源：http://vk.huanxung.cn

C#:   public string Name { get; set; }
来源：http://jw.nicolike.cn

[G12] 对象转字符串
来源：http://nx.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://gh.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rq.521024.cn

JS:   toString() { return this.name; }
来源：http://yy.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://zm.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://cx.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cw.newstarts.cn

Ruby: def to_s; @name; end
来源：http://rr.asd995.cn

C#:   public override string ToString() => Name;
来源：http://qq.asd995.cn

[G13] 判断对象类型
来源：http://ui.szxytkj.cn

Py:   isinstance(u, User)
来源：http://gi.muxihuayi.cn

PHP:  $u instanceof User
来源：http://ml.jctech888.com.cn

JS:   u instanceof User
来源：http://ch.shxzukj.cn

TS:   u instanceof User
来源：http://fz.huanxung.cn

Java: u instanceof User
来源：http://mn.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hh.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://cz.gzmigu.cn

C#:   u is User
来源：http://ui.gzmigu.cn

[G14] 数据类 / record
来源：http://aw.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://in.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://xm.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sn.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://of.szsharing.cn

Java: record User(String name, int age) {}
来源：http://ni.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://ut.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bg.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://mr.hahajie.cn

[G15] 枚举
来源：http://vl.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ei.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://up.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ad.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oy.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://sj.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qz.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://kp.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qi.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://jp.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://km.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://rs.lnxyls.cn

JS:   Object.entries(obj)
来源：http://tq.lnxyls.cn

TS:   Object.entries(obj)
来源：http://ua.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sa.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pg.gzmigu.cn

Ruby: obj.instance_variables
来源：http://wh.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://zk.huanxung.cn

================================================================================
来源：http://pi.shtwfgs.cn

H. 异常与错误处理
来源：http://ew.521024.cn

================================================================================
来源：http://bj.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://mb.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tq.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fx.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ak.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ua.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ip.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://re.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gn.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ga.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://lh.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zk.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bz.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kf.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://so.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://af.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ea.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sx.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jg.shxzukj.cn

[H03] 主动抛出异常
来源：http://kh.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://sh.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rj.asd995.cn

JS:   throw new Error("错误信息");
来源：http://ub.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://sx.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rk.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gz.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xu.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fs.szsharing.cn

[H04] 自定义异常类型
来源：http://yo.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://em.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lm.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://ft.asd995.cn

TS:   class MyError extends Error {}
来源：http://uk.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://oo.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uj.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://hk.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://hz.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://rw.gzmigu.cn

Py:   except ValueError as e:
来源：http://ze.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vl.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://se.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://yc.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://hm.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ft.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://nz.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dd.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://jm.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://kp.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yq.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nk.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zi.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://li.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bn.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://uf.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://kz.szsharing.cn

[H07] 断言
来源：http://im.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://es.szxytkj.cn

PHP:  assert($x > 0);
来源：http://of.szsharing.cn

JS:   console.assert(x > 0);
来源：http://yt.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://yr.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://du.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gj.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://sj.521024.cn

[H08] 获取错误信息与堆栈
来源：http://ik.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ff.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ep.szsharing.cn

JS:   e.message;  e.stack
来源：http://zq.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tp.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xh.hahajie.cn

Go:   err.Error()
来源：http://rd.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://jy.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://xd.muxihuayi.cn

[H09] 带错误码的异常
来源：http://mz.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rx.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yh.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gx.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ny.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://se.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bv.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oi.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vt.asd995.cn

[H10] 资源自动释放
来源：http://tu.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uu.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wk.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iz.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lb.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gb.nicolike.cn

Go:   defer f.Close()
来源：http://tw.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mv.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hu.panjiajie.cn

================================================================================
来源：http://wc.muxihuayi.cn

I. 正则表达式
来源：http://wz.yuntaijiaju.cn

================================================================================
来源：http://tc.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://ad.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fr.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zt.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://wo.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://nr.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vn.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bo.521024.cn

Ruby: s.match?(/\d+/)
来源：http://bz.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ii.chemitech.net.cn

[I02] 提取所有匹配
来源：http://dv.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://uj.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fy.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qd.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://nh.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fu.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gv.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://de.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lf.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://nq.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xb.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sh.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://th.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vd.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ij.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zp.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://om.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://so.szxytkj.cn

[I04] 正则替换
来源：http://ws.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xv.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://io.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nw.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kx.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ps.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yk.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dh.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ja.muxihuayi.cn

[I05] 按正则拆分
来源：http://hp.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kv.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dg.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://tn.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://sk.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://wp.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hp.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bl.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uw.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ny.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kd.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tt.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yi.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xs.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zq.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zj.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ro.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tk.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://iy.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xh.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yd.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dt.muxihuayi.cn

TS:   /error/gim
来源：http://vx.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xu.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://to.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://vy.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mo.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://in.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bi.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yp.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yx.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oh.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sd.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xc.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ax.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nt.panjiajie.cn

================================================================================
来源：http://ql.yuexingan06.cn

J. 日期与时间
来源：http://yw.9csxet.cn

================================================================================
来源：http://gx.haigaiapp.cn

[J01] 获取当前时间
来源：http://mw.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cm.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uh.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://zw.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://wg.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uh.yuntaijiaju.cn

Go:   time.Now()
来源：http://wl.jianghongdianzi.cn

Ruby: Time.now
来源：http://wm.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eb.nicolike.cn

[J02] 格式化输出
来源：http://mk.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jj.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rn.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pc.chemitech.net.cn

TS:   d.toISOString()
来源：http://we.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xh.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xe.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ct.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ia.521024.cn

[J03] 字符串解析为日期
来源：http://gf.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ek.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jp.521024.cn

JS:   new Date("2024-01-02")
来源：http://te.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://bg.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vs.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://el.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://zr.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ox.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://gs.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zk.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vn.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eg.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yb.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jp.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ff.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uh.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ly.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://zx.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://zd.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qa.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://za.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bw.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://rm.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rt.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://bl.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yn.gzmigu.cn

[J06] 计算两时间之差
来源：http://bu.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://jt.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://hf.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iu.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uz.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wl.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://mw.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://mi.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://oc.shtwfgs.cn

[J07] 比较两个日期
来源：http://gd.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://wq.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://of.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vd.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pp.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sj.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://og.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jc.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://gw.lnxyls.cn

[J08] 提取年月日与星期
来源：http://zu.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ip.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gu.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sv.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hd.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://me.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ub.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oy.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fx.colortex.cn

[J09] 时区处理
来源：http://gc.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wo.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://np.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zk.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vz.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hw.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bb.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hv.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kx.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://vg.shtwfgs.cn


<!-- 参考信息 -->