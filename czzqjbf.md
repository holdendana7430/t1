代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://yk.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://pi.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://ur.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://fw.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gq.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://cw.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://yy.panjiajie.cn

[G13] 判断对象类型
来源：http://da.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://uj.nicolike.cn

PHP:  $u instanceof User
来源：http://xg.nicolike.cn

JS:   u instanceof User
来源：http://ve.hnjuh.cn

TS:   u instanceof User
来源：http://ep.wgjwhj.cn

Java: u instanceof User
来源：http://cr.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://li.colortex.cn

Ruby: u.is_a?(User)
来源：http://cg.hahajie.cn

C#:   u is User
来源：http://pa.shxzskj.cn

[G14] 数据类 / record
来源：http://ia.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dz.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://ms.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kp.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://mt.9csxet.cn

Java: record User(String name, int age) {}
来源：http://mh.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://ms.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ob.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://tr.szxytkj.cn

[G15] 枚举
来源：http://cm.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hy.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://er.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ll.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ae.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://hz.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uh.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://mg.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hl.521024.cn

[G16] 对象转数组 / 字典
来源：http://xp.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cg.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://xj.colortex.cn

JS:   Object.entries(obj)
来源：http://co.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://xn.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fl.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ss.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://iz.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://jh.asd995.cn

================================================================================
来源：http://rb.muxihuayi.cn

H. 异常与错误处理
来源：http://st.hnjuh.cn

================================================================================
来源：http://pd.nicolike.cn

[H01] try / catch 基础
来源：http://nq.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fb.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://df.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iv.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jh.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qv.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fv.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hu.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ih.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://iq.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lf.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ms.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kr.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jy.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://iv.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kd.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yz.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vr.shxzskj.cn

[H03] 主动抛出异常
来源：http://ti.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://bp.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hn.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://ce.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://ut.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dw.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ab.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fu.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ra.panjiajie.cn

[H04] 自定义异常类型
来源：http://ru.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://wf.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wa.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://wn.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://gb.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://gy.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eo.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://dl.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://ho.jctech888.com.cn

[H05] 捕获特定类型
来源：http://oc.panjiajie.cn

Py:   except ValueError as e:
来源：http://ns.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nv.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://tb.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://ob.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://hn.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gq.521024.cn

Ruby: rescue ArgumentError => e
来源：http://sj.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nd.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://qm.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://ni.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vf.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iw.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zi.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://li.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ys.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://eu.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://je.yuexingan06.cn

[H07] 断言
来源：http://ud.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://py.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://wc.asd995.cn

JS:   console.assert(x > 0);
来源：http://cj.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://av.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://ko.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nh.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nq.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://dn.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://le.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://gb.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qo.gzmigu.cn

JS:   e.message;  e.stack
来源：http://hg.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ih.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gx.hnjuh.cn

Go:   err.Error()
来源：http://go.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://tq.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://ct.huanxung.cn

[H09] 带错误码的异常
来源：http://xz.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bg.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ps.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yn.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wj.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qz.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ak.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wa.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ls.gzmigu.cn

[H10] 资源自动释放
来源：http://al.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://em.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lz.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fp.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bz.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gu.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://rl.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uo.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hq.asd995.cn

================================================================================
来源：http://hm.lnxyls.cn

I. 正则表达式
来源：http://qd.gzmigu.cn

================================================================================
来源：http://bb.shxzskj.cn

[I01] 判断是否匹配
来源：http://ib.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bl.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mg.9csxet.cn

JS:   /\d+/.test(s)
来源：http://py.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://gi.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://di.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ss.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://uc.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zv.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://fi.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://qu.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ac.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ig.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://wp.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qw.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kd.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://yj.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lo.colortex.cn

[I03] 提取捕获分组
来源：http://he.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://li.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ir.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wj.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dm.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bq.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ky.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nw.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ea.huixiangedu.cn

[I04] 正则替换
来源：http://gm.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bn.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ly.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tk.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tp.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ln.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xz.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nl.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fx.newstarts.cn

[I05] 按正则拆分
来源：http://pg.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nz.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vb.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://we.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://ui.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://di.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cp.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yy.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ul.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ti.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kp.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ms.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://if.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://py.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://om.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rw.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://po.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ox.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://fm.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mh.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://si.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fv.bjjhwx.cn

TS:   /error/gim
来源：http://ax.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tm.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xk.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://qp.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ut.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://zj.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rc.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wr.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cq.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ps.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kb.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yr.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://or.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qk.jianghongdianzi.cn

================================================================================
来源：http://au.521024.cn

J. 日期与时间
来源：http://nc.muxihuayi.cn

================================================================================
来源：http://vz.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://et.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iq.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hv.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://mz.szsharing.cn

TS:   new Date();  Date.now()
来源：http://ww.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pv.hnjuh.cn

Go:   time.Now()
来源：http://ze.newstarts.cn

Ruby: Time.now
来源：http://jn.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sy.asd995.cn

[J02] 格式化输出
来源：http://wu.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lz.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cw.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://he.haigaiapp.cn

TS:   d.toISOString()
来源：http://yx.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yq.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vj.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mz.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oe.nszjky.cn

[J03] 字符串解析为日期
来源：http://vw.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ff.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://il.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://vi.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://xd.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qd.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gc.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://mv.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qx.521024.cn

[J04] 时间戳与日期互转
来源：http://kx.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mp.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uq.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://js.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://az.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zf.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://th.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://al.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cf.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://bo.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://il.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xr.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://is.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vt.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://tl.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ms.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://bf.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wc.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://iy.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://li.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://xp.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wq.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://my.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vz.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://ku.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://yk.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://ip.newstarts.cn

[J07] 比较两个日期
来源：http://rc.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://cx.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bp.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lw.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ve.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eq.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ki.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gx.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://aa.shxzukj.cn

[J08] 提取年月日与星期
来源：http://xd.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dr.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://px.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jc.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ar.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qb.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ic.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ea.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://af.521024.cn

[J09] 时区处理
来源：http://dl.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zu.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kl.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yo.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sq.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ig.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kp.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://id.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rm.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://gj.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gk.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cs.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wj.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ju.shtwfgs.cn


<!-- 参考信息 -->