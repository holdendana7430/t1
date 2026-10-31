代发 wailian999

Ruby: attr_accessor :name
来源：http://le.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://hr.wgjwhj.cn

[G12] 对象转字符串
来源：http://tb.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://fi.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://po.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://gh.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://bt.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://ls.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gn.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://vy.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://tu.szxytkj.cn

[G13] 判断对象类型
来源：http://im.shxzukj.cn

Py:   isinstance(u, User)
来源：http://hd.panjiajie.cn

PHP:  $u instanceof User
来源：http://ho.lnxyls.cn

JS:   u instanceof User
来源：http://ox.haigaiapp.cn

TS:   u instanceof User
来源：http://nl.shxzskj.cn

Java: u instanceof User
来源：http://nx.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zu.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://is.colortex.cn

C#:   u is User
来源：http://li.szxytkj.cn

[G14] 数据类 / record
来源：http://rx.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mh.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://il.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zq.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://xw.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://xj.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://ua.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hp.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://bl.yuntaijiaju.cn

[G15] 枚举
来源：http://er.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qq.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sq.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cf.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rv.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://ho.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vg.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://yv.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vk.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://tb.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://in.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://sv.gzmigu.cn

JS:   Object.entries(obj)
来源：http://zo.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://zf.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ii.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ob.newstarts.cn

Ruby: obj.instance_variables
来源：http://kf.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://yt.shtwfgs.cn

================================================================================
来源：http://xo.huanxung.cn

H. 异常与错误处理
来源：http://ql.jianghongdianzi.cn

================================================================================
来源：http://om.jctech888.com.cn

[H01] try / catch 基础
来源：http://ou.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ww.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gn.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ae.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gq.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ks.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jm.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vv.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qx.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://gz.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ur.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lh.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qs.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wd.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rs.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zz.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://km.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gm.hnjuh.cn

[H03] 主动抛出异常
来源：http://nl.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://qz.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ac.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://at.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://yp.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ir.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tb.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yx.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bx.nszjky.cn

[H04] 自定义异常类型
来源：http://em.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://bh.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xy.521024.cn

JS:   class MyError extends Error {}
来源：http://xj.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://gv.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://de.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dc.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ju.szsharing.cn

C#:   class MyException : Exception {}
来源：http://pu.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://av.szsharing.cn

Py:   except ValueError as e:
来源：http://uz.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ep.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://mt.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://yd.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://oi.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fg.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://zn.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://az.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://tu.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://tk.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ha.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vq.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ga.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ey.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jj.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ds.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://pd.haigaiapp.cn

[H07] 断言
来源：http://ey.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://bp.shxzskj.cn

PHP:  assert($x > 0);
来源：http://zx.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://xy.szsharing.cn

TS:   console.assert(x > 0);
来源：http://sg.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://ye.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uo.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vc.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://lz.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://xh.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://iq.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qi.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://wk.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ay.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nd.shtwfgs.cn

Go:   err.Error()
来源：http://kg.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://hx.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://is.wgjwhj.cn

[H09] 带错误码的异常
来源：http://jp.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://on.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://il.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lq.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wg.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://md.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zg.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://de.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vd.jctech888.com.cn

[H10] 资源自动释放
来源：http://lg.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ol.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dd.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hn.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xr.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jv.colortex.cn

Go:   defer f.Close()
来源：http://dj.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qp.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wy.lnxyls.cn

================================================================================
来源：http://rd.521024.cn

I. 正则表达式
来源：http://ak.bookmarksfly.cn

================================================================================
来源：http://ch.shxzukj.cn

[I01] 判断是否匹配
来源：http://ku.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fh.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://us.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://ck.szsharing.cn

TS:   /\d+/.test(s)
来源：http://ci.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jr.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hj.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://gz.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://us.hahajie.cn

[I02] 提取所有匹配
来源：http://iy.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://sm.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kc.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gc.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://ju.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bs.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vm.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://kj.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jh.nszjky.cn

[I03] 提取捕获分组
来源：http://we.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ug.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gf.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qg.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bl.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://th.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pw.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pb.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hb.bjjhwx.cn

[I04] 正则替换
来源：http://zs.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jd.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lx.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yu.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qd.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fo.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wl.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://el.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bt.lnxyls.cn

[I05] 按正则拆分
来源：http://kv.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dx.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ja.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://an.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://if.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://ba.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gb.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ax.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ys.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dk.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://et.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bu.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wy.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ld.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xa.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ae.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vz.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ki.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://du.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kc.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fd.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://em.wgjwhj.cn

TS:   /error/gim
来源：http://ao.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ob.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wc.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://df.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oc.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://up.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yt.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bi.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ux.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hy.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://go.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oh.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kh.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bj.muxihuayi.cn

================================================================================
来源：http://no.521024.cn

J. 日期与时间
来源：http://ko.szsharing.cn

================================================================================
来源：http://yx.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://ej.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kt.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uh.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://zk.huanxung.cn

TS:   new Date();  Date.now()
来源：http://gx.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pq.bookmarksfly.cn

Go:   time.Now()
来源：http://ah.lnxyls.cn

Ruby: Time.now
来源：http://za.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://je.chemitech.net.cn

[J02] 格式化输出
来源：http://zi.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bg.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wa.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xb.asd995.cn

TS:   d.toISOString()
来源：http://hb.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qc.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zo.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mt.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nz.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://fa.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tu.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lm.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://fc.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://as.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ra.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vj.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://wc.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gq.asd995.cn

[J04] 时间戳与日期互转
来源：http://mt.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ja.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zx.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zu.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ji.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lm.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oj.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jd.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wk.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://kz.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://fv.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nz.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ri.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ra.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://fh.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ow.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://mc.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lg.colortex.cn

[J06] 计算两时间之差
来源：http://wy.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://pt.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://uw.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qm.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qg.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zr.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://tk.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://py.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://sf.huixiangedu.cn

[J07] 比较两个日期
来源：http://gc.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://ak.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dd.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gc.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bu.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gq.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eg.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://no.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://ek.nszjky.cn

[J08] 提取年月日与星期
来源：http://ah.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pi.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ni.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pd.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pe.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ek.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qx.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lr.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gu.colortex.cn

[J09] 时区处理
来源：http://tn.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://st.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wu.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wr.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vo.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dv.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://in.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fv.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ok.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://tx.bjjhwx.cn


<!-- 参考信息 -->