代发 wailian999

JS:   get name() { return this._name; }
来源：http://nr.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://fx.colortex.cn

Java: public String getName() { return name; }
来源：http://pe.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tz.hahajie.cn

Ruby: attr_accessor :name
来源：http://wv.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://br.9csxet.cn

[G12] 对象转字符串
来源：http://be.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://ct.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ym.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://ed.521024.cn

TS:   toString(): string { return this.name; }
来源：http://rn.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://jw.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jg.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://gk.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://ql.chemitech.net.cn

[G13] 判断对象类型
来源：http://ve.colortex.cn

Py:   isinstance(u, User)
来源：http://bh.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://xv.yuntaijiaju.cn

JS:   u instanceof User
来源：http://ye.521024.cn

TS:   u instanceof User
来源：http://az.lnxyls.cn

Java: u instanceof User
来源：http://xu.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pc.asd995.cn

Ruby: u.is_a?(User)
来源：http://vh.wgjwhj.cn

C#:   u is User
来源：http://nb.colortex.cn

[G14] 数据类 / record
来源：http://be.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bu.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://pe.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hn.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://tc.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://gr.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://qq.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kp.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://jv.huanxung.cn

[G15] 枚举
来源：http://cp.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fo.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jm.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qt.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sr.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://ny.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xa.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://ye.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vw.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://hr.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ak.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://fk.nicolike.cn

JS:   Object.entries(obj)
来源：http://yb.hnjuh.cn

TS:   Object.entries(obj)
来源：http://rx.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ps.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pv.hahajie.cn

Ruby: obj.instance_variables
来源：http://ne.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://gr.wgjwhj.cn

================================================================================
来源：http://ft.huixinmuqiang.cn

H. 异常与错误处理
来源：http://dm.haigaiapp.cn

================================================================================
来源：http://gq.muxihuayi.cn

[H01] try / catch 基础
来源：http://xs.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://or.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uz.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qe.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vl.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jm.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fw.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rb.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://et.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://xh.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ws.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dj.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yx.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gy.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fh.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cf.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://df.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fz.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://zr.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://xr.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hw.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://na.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://dk.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://si.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sy.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aw.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://za.szxytkj.cn

[H04] 自定义异常类型
来源：http://ol.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://tj.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zo.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://co.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://yq.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://fa.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wx.521024.cn

Ruby: class MyError < StandardError; end
来源：http://ag.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://cl.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://mx.newstarts.cn

Py:   except ValueError as e:
来源：http://hv.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ee.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://od.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://au.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://lv.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ay.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://qx.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vb.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://oo.9csxet.cn

Py:   value = d.get("k") or default
来源：http://cz.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ui.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://et.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ks.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xo.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vx.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://zv.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://wl.huanxung.cn

[H07] 断言
来源：http://os.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://va.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://uo.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://aq.colortex.cn

TS:   console.assert(x > 0);
来源：http://qf.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://ez.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ei.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vy.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://bf.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://ax.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://fp.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uk.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://pc.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yy.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://le.lnxyls.cn

Go:   err.Error()
来源：http://dw.521024.cn

Ruby: e.message;  e.backtrace
来源：http://pq.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://bo.shtwfgs.cn

[H09] 带错误码的异常
来源：http://lc.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jb.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yo.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://te.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jq.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hh.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kg.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nk.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jo.szxytkj.cn

[H10] 资源自动释放
来源：http://jf.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kh.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oi.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://si.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yv.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mm.jctech888.com.cn

Go:   defer f.Close()
来源：http://uz.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gm.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uf.huixinmuqiang.cn

================================================================================
来源：http://ga.huixinmuqiang.cn

I. 正则表达式
来源：http://yq.gzmigu.cn

================================================================================
来源：http://bc.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://zq.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hw.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fk.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://ng.521024.cn

TS:   /\d+/.test(s)
来源：http://yo.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sc.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nj.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://ei.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sj.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://zx.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://qp.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rp.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fi.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://hf.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://on.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rj.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://eh.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vb.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://rb.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://np.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hx.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jo.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dx.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vp.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qb.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yh.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ty.bjjhwx.cn

[I04] 正则替换
来源：http://zl.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rh.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fo.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ur.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ju.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cz.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ik.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://er.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://it.shxzskj.cn

[I05] 按正则拆分
来源：http://uh.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sv.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://av.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://nf.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://mu.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://ux.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ih.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gp.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rm.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://za.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bi.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dy.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nh.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://su.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gj.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mo.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hr.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xg.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://sz.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zj.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iz.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wk.huixinmuqiang.cn

TS:   /error/gim
来源：http://tr.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xl.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mw.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://xc.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pt.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://ld.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iq.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ju.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ws.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yq.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gg.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gz.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fb.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fy.huanxung.cn

================================================================================
来源：http://kq.newstarts.cn

J. 日期与时间
来源：http://yq.panjiajie.cn

================================================================================
来源：http://gp.nicolike.cn

[J01] 获取当前时间
来源：http://rd.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bs.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://io.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://et.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://cy.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mc.wgjwhj.cn

Go:   time.Now()
来源：http://ox.newstarts.cn

Ruby: Time.now
来源：http://mo.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mz.haigaiapp.cn

[J02] 格式化输出
来源：http://oh.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vy.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://li.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lq.bookmarksfly.cn

TS:   d.toISOString()
来源：http://ix.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yo.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ab.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vs.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wr.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://xu.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ok.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ii.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://sk.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://dy.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cy.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://li.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://me.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sw.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://pq.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bd.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ot.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qu.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oz.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ay.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jc.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tk.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yd.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://tw.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://go.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hm.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://av.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ld.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://gc.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cf.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://nv.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vm.huanxung.cn

[J06] 计算两时间之差
来源：http://ji.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://ul.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://ul.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yh.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wr.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nb.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://cu.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://xw.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://gq.shtwfgs.cn

[J07] 比较两个日期
来源：http://rv.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://ew.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://je.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vv.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iw.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iz.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hx.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nl.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://uz.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://pp.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tq.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://to.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mc.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ea.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gx.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fx.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://of.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://en.newstarts.cn

[J09] 时区处理
来源：http://fz.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lg.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rd.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yj.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qr.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mi.muxihuayi.cn


<!-- 参考信息 -->