代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://gz.newstarts.cn

JS:   toString() { return this.name; }
来源：http://gk.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://oi.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://mz.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gt.hahajie.cn

Ruby: def to_s; @name; end
来源：http://un.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://ts.hnjuh.cn

[G13] 判断对象类型
来源：http://mp.shxzskj.cn

Py:   isinstance(u, User)
来源：http://id.panjiajie.cn

PHP:  $u instanceof User
来源：http://py.shtwfgs.cn

JS:   u instanceof User
来源：http://jf.yuexingan06.cn

TS:   u instanceof User
来源：http://wh.yuexingan06.cn

Java: u instanceof User
来源：http://mr.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aj.9csxet.cn

Ruby: u.is_a?(User)
来源：http://ha.szxytkj.cn

C#:   u is User
来源：http://qt.yuexingan06.cn

[G14] 数据类 / record
来源：http://vi.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gy.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://bg.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qr.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://wc.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://mg.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://sz.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://il.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://kk.szsharing.cn

[G15] 枚举
来源：http://jt.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nz.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tt.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hr.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fk.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://zf.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://of.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://wv.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ml.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://sl.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vh.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://qq.lnxyls.cn

JS:   Object.entries(obj)
来源：http://xk.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://su.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wn.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kf.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://lp.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ia.lnxyls.cn

================================================================================
来源：http://js.yuntaijiaju.cn

H. 异常与错误处理
来源：http://gs.bookmarksfly.cn

================================================================================
来源：http://rx.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://pw.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jd.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oi.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uj.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://go.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nv.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sh.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qo.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jx.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://ob.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oh.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://su.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cb.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://on.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bw.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yi.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ik.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vf.shxzukj.cn

[H03] 主动抛出异常
来源：http://td.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://em.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kz.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://ow.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://vj.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gh.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jd.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ax.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rz.haigaiapp.cn

[H04] 自定义异常类型
来源：http://qm.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://ae.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nk.nszjky.cn

JS:   class MyError extends Error {}
来源：http://zx.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://qi.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://bn.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wx.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://nw.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://bc.hahajie.cn

[H05] 捕获特定类型
来源：http://nx.shxzukj.cn

Py:   except ValueError as e:
来源：http://tj.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yi.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://bb.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://sf.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://fo.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dy.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://dd.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pk.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://di.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://vs.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qk.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://un.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jr.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ol.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://qd.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://tn.9csxet.cn

[H07] 断言
来源：http://mq.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://gl.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://tz.huanxung.cn

JS:   console.assert(x > 0);
来源：http://ev.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://zb.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://yh.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mj.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mm.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://xz.521024.cn

[H08] 获取错误信息与堆栈
来源：http://iv.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://fc.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ay.9csxet.cn

JS:   e.message;  e.stack
来源：http://dd.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pq.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wm.bjjhwx.cn

Go:   err.Error()
来源：http://hi.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://yi.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://ar.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://uv.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vb.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tw.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ko.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kc.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zk.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pp.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rv.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xs.panjiajie.cn

[H10] 资源自动释放
来源：http://cu.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fv.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eq.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ej.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://at.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ra.shxzukj.cn

Go:   defer f.Close()
来源：http://ag.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ol.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cf.yuntaijiaju.cn

================================================================================
来源：http://oa.jianghongdianzi.cn

I. 正则表达式
来源：http://nf.521024.cn

================================================================================
来源：http://em.gzmigu.cn

[I01] 判断是否匹配
来源：http://yw.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qr.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gr.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://hd.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://tl.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uu.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iy.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://kn.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sc.muxihuayi.cn

[I02] 提取所有匹配
来源：http://ut.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ox.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bj.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cl.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://ob.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ty.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ah.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://jk.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wt.wgjwhj.cn

[I03] 提取捕获分组
来源：http://si.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://go.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qb.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jn.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eo.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tm.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://so.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://br.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ya.asd995.cn

[I04] 正则替换
来源：http://ll.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mo.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zp.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ln.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://px.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mj.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gy.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yk.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pu.huanxung.cn

[I05] 按正则拆分
来源：http://cl.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gv.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rx.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ib.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://tg.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://zf.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xz.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vi.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hu.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ri.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cz.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dd.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iz.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://al.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cm.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nt.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wz.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://os.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://gu.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oa.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hc.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ha.9csxet.cn

TS:   /error/gim
来源：http://en.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vv.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zt.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://kb.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rr.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://lf.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zt.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jz.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xe.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lx.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yl.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nn.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://so.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ve.nszjky.cn

================================================================================
来源：http://kq.gzmigu.cn

J. 日期与时间
来源：http://zl.bjjhwx.cn

================================================================================
来源：http://jb.panjiajie.cn

[J01] 获取当前时间
来源：http://be.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ac.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hn.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://it.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://pu.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xo.bookmarksfly.cn

Go:   time.Now()
来源：http://op.colortex.cn

Ruby: Time.now
来源：http://iq.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://on.yuntaijiaju.cn

[J02] 格式化输出
来源：http://yc.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hb.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ij.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wm.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://kk.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ah.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oa.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cx.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mw.gzmigu.cn

[J03] 字符串解析为日期
来源：http://lh.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sr.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://um.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://qq.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://nj.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wp.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hs.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://ud.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ex.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://tk.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sf.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eb.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nr.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xg.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://so.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qi.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rm.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://iy.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://gg.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kj.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yu.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ee.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://pc.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ii.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://qo.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sx.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://ip.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://ri.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://wy.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://go.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ob.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dz.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://zm.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://kb.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://sw.hnjuh.cn

[J07] 比较两个日期
来源：http://rd.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://pi.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ru.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kh.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vi.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wm.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pa.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ov.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://yn.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://th.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://se.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qn.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qk.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qc.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zs.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yl.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://md.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ah.panjiajie.cn

[J09] 时区处理
来源：http://np.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ob.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ue.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gc.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hk.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nt.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oa.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ll.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ve.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://gl.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gy.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pm.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ju.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xm.521024.cn


<!-- 参考信息 -->