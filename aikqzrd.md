代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://xj.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://hb.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://rt.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://rx.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jo.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://yg.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://us.wgjwhj.cn

[G13] 判断对象类型
来源：http://vo.asd995.cn

Py:   isinstance(u, User)
来源：http://mj.wgjwhj.cn

PHP:  $u instanceof User
来源：http://pd.gzmigu.cn

JS:   u instanceof User
来源：http://dv.9csxet.cn

TS:   u instanceof User
来源：http://gd.shxzskj.cn

Java: u instanceof User
来源：http://wn.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://af.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://ya.haigaiapp.cn

C#:   u is User
来源：http://uf.hnjuh.cn

[G14] 数据类 / record
来源：http://dr.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oy.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://oo.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bg.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://ff.521024.cn

Java: record User(String name, int age) {}
来源：http://tn.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://tu.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wb.asd995.cn

C#:   record User(string Name, int Age);
来源：http://ru.jianghongdianzi.cn

[G15] 枚举
来源：http://la.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zh.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://eq.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aj.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gj.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://qe.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ih.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://rn.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bn.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://ts.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bi.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://pv.asd995.cn

JS:   Object.entries(obj)
来源：http://zg.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://ow.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hj.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qj.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://sg.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://ze.shxzskj.cn

================================================================================
来源：http://de.chemitech.net.cn

H. 异常与错误处理
来源：http://mz.gzmigu.cn

================================================================================
来源：http://qb.szxytkj.cn

[H01] try / catch 基础
来源：http://hp.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tm.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sy.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vh.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pc.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pf.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ub.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gl.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fv.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://qe.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dh.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vd.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ol.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vt.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tx.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sa.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qw.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ie.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://nv.521024.cn

Py:   raise ValueError("错误信息")
来源：http://ji.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fb.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://de.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://fh.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xw.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xn.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ar.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ia.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://np.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://tu.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nh.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://dy.asd995.cn

TS:   class MyError extends Error {}
来源：http://vy.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://sm.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xo.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://nf.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://kt.shtwfgs.cn

[H05] 捕获特定类型
来源：http://hf.chemitech.net.cn

Py:   except ValueError as e:
来源：http://pi.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aj.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://eo.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://hy.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://gp.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yq.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://wh.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tz.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://vh.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://ez.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ch.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wq.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://th.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ty.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dw.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://cv.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://tb.bookmarksfly.cn

[H07] 断言
来源：http://wi.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://pk.hnjuh.cn

PHP:  assert($x > 0);
来源：http://pg.nszjky.cn

JS:   console.assert(x > 0);
来源：http://lw.huanxung.cn

TS:   console.assert(x > 0);
来源：http://de.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://xk.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uv.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sn.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://jk.521024.cn

[H08] 获取错误信息与堆栈
来源：http://fj.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://fo.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nz.lnxyls.cn

JS:   e.message;  e.stack
来源：http://kh.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ya.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bj.shxzskj.cn

Go:   err.Error()
来源：http://xh.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://rf.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://kh.huixiangedu.cn

[H09] 带错误码的异常
来源：http://mj.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eh.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pd.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lf.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://we.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ig.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ne.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ob.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xs.huanxung.cn

[H10] 资源自动释放
来源：http://il.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fm.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oy.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fv.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://re.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pt.hnjuh.cn

Go:   defer f.Close()
来源：http://rh.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jm.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qd.colortex.cn

================================================================================
来源：http://ha.9csxet.cn

I. 正则表达式
来源：http://if.shxzukj.cn

================================================================================
来源：http://ox.huixiangedu.cn

[I01] 判断是否匹配
来源：http://kf.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pa.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ka.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://mb.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://xy.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hw.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yx.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://dj.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ir.gzmigu.cn

[I02] 提取所有匹配
来源：http://my.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://yq.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ji.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kv.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://ny.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rn.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://an.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://uh.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ep.gzmigu.cn

[I03] 提取捕获分组
来源：http://ie.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iu.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://os.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ay.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ut.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dk.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rx.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bh.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vc.shxzskj.cn

[I04] 正则替换
来源：http://lz.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pe.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mb.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ij.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ow.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://th.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tq.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zt.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ee.shxzskj.cn

[I05] 按正则拆分
来源：http://ss.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ke.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sn.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://hw.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://lv.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://bv.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://to.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pr.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tm.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wv.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jj.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qm.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ng.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xy.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xi.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bf.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ng.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qo.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://wm.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oh.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://th.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ut.asd995.cn

TS:   /error/gim
来源：http://sz.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rz.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zg.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://rj.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://az.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://gr.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lj.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cp.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tw.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ho.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bb.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vq.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gu.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bq.jianghongdianzi.cn

================================================================================
来源：http://pi.lnxyls.cn

J. 日期与时间
来源：http://sy.gzmigu.cn

================================================================================
来源：http://pq.bookmarksfly.cn

[J01] 获取当前时间
来源：http://fy.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ir.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mz.hahajie.cn

JS:   new Date();  Date.now()
来源：http://mt.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://ag.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vw.asd995.cn

Go:   time.Now()
来源：http://cj.yuntaijiaju.cn

Ruby: Time.now
来源：http://da.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mg.yuexingan06.cn

[J02] 格式化输出
来源：http://rb.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ex.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eu.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uc.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://st.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://df.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kv.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dv.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lz.gzmigu.cn

[J03] 字符串解析为日期
来源：http://nw.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eh.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eh.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://pk.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://pv.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://my.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://by.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://rh.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ft.asd995.cn

[J04] 时间戳与日期互转
来源：http://gy.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pi.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ri.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tm.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rv.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vt.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zp.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nx.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pa.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://sz.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://st.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aq.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xr.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qb.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://tg.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qv.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://ay.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vw.chemitech.net.cn

[J06] 计算两时间之差
来源：http://um.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://hz.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://tr.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tw.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mk.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yg.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://nc.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://th.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://xi.huixiangedu.cn

[J07] 比较两个日期
来源：http://mz.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://xc.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bi.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ul.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aq.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ji.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ss.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pi.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://db.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://xn.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uw.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://md.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wm.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nw.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fe.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cs.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yh.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yp.nicolike.cn

[J09] 时区处理
来源：http://vj.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bx.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pg.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qc.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nv.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yp.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lv.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sf.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lv.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://ea.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fy.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wc.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rd.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xq.haigaiapp.cn


<!-- 参考信息 -->