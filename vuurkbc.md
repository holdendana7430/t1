代发 wailian999

Ruby: attr_accessor :name
来源：http://ga.521024.cn

C#:   public string Name { get; set; }
来源：http://js.haigaiapp.cn

[G12] 对象转字符串
来源：http://nd.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://vj.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bs.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://wd.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://vr.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://yr.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qc.huanxung.cn

Ruby: def to_s; @name; end
来源：http://oh.colortex.cn

C#:   public override string ToString() => Name;
来源：http://ud.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://xa.521024.cn

Py:   isinstance(u, User)
来源：http://kx.szsharing.cn

PHP:  $u instanceof User
来源：http://df.szxytkj.cn

JS:   u instanceof User
来源：http://zr.521024.cn

TS:   u instanceof User
来源：http://ru.asd995.cn

Java: u instanceof User
来源：http://pd.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vh.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://kj.panjiajie.cn

C#:   u is User
来源：http://jf.shtwfgs.cn

[G14] 数据类 / record
来源：http://pp.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fx.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://ot.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ij.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://tc.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://vl.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://rk.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://on.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://ld.nszjky.cn

[G15] 枚举
来源：http://hr.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ix.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rn.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wj.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zd.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://ml.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cz.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://qr.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lc.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://yc.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qu.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://dk.nszjky.cn

JS:   Object.entries(obj)
来源：http://yj.9csxet.cn

TS:   Object.entries(obj)
来源：http://gy.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vt.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://io.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://yb.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://gz.szsharing.cn

================================================================================
来源：http://ta.hnjuh.cn

H. 异常与错误处理
来源：http://vk.yuntaijiaju.cn

================================================================================
来源：http://rl.chemitech.net.cn

[H01] try / catch 基础
来源：http://pz.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rz.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zk.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ka.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yu.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cx.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wa.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uy.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ja.nicolike.cn

[H02] finally / ensure 收尾
来源：http://du.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mh.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rd.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lq.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yg.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ml.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lv.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zc.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gt.yuexingan06.cn

[H03] 主动抛出异常
来源：http://gn.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://ws.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cu.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://ym.colortex.cn

TS:   throw new Error("错误信息");
来源：http://ul.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ez.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bu.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hk.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qo.gzmigu.cn

[H04] 自定义异常类型
来源：http://ix.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://pg.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://li.newstarts.cn

JS:   class MyError extends Error {}
来源：http://iv.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://ac.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://gj.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cg.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://bg.9csxet.cn

C#:   class MyException : Exception {}
来源：http://vx.nicolike.cn

[H05] 捕获特定类型
来源：http://rl.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://ag.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wc.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://hp.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://dd.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://xy.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uz.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://ii.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sf.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://xl.nszjky.cn

Py:   value = d.get("k") or default
来源：http://jr.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ub.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ol.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://op.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gq.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xc.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://ab.521024.cn

C#:   obj?.A?.B ?? default
来源：http://ze.szsharing.cn

[H07] 断言
来源：http://xr.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://rk.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://qy.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://nw.nszjky.cn

TS:   console.assert(x > 0);
来源：http://lc.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://vy.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gr.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mi.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://fs.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://mg.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://wp.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dy.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://ob.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ar.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bz.shxzskj.cn

Go:   err.Error()
来源：http://qz.521024.cn

Ruby: e.message;  e.backtrace
来源：http://pd.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://eh.bjjhwx.cn

[H09] 带错误码的异常
来源：http://kt.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pi.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://um.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fo.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zr.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ge.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://un.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zk.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cu.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://em.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vz.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sz.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iv.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ee.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fw.shxzukj.cn

Go:   defer f.Close()
来源：http://vq.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zo.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rs.colortex.cn

================================================================================
来源：http://wo.panjiajie.cn

I. 正则表达式
来源：http://kw.huanxung.cn

================================================================================
来源：http://jy.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://sg.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hl.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oz.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://vg.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://ja.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uf.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gn.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://wy.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hl.newstarts.cn

[I02] 提取所有匹配
来源：http://ys.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://bi.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ic.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sm.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://xu.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xo.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tb.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://xx.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qe.lnxyls.cn

[I03] 提取捕获分组
来源：http://em.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ii.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dn.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xt.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://em.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ey.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ya.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jn.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ac.lnxyls.cn

[I04] 正则替换
来源：http://ey.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ca.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fx.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://su.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wi.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rq.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tr.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cr.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fb.bjjhwx.cn

[I05] 按正则拆分
来源：http://cs.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://re.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ql.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://yq.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ei.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://cv.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ha.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wx.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://li.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ty.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://it.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sw.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tl.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jp.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://az.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fg.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kf.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tn.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://qb.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ib.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qh.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ch.bookmarksfly.cn

TS:   /error/gim
来源：http://hw.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vv.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zl.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://dz.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ns.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://cq.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pu.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ei.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nf.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ce.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jd.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gi.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gy.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kw.chemitech.net.cn

================================================================================
来源：http://vd.asd995.cn

J. 日期与时间
来源：http://nj.gzmigu.cn

================================================================================
来源：http://ls.521024.cn

[J01] 获取当前时间
来源：http://zi.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bm.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ud.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://sj.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://lx.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://za.szxytkj.cn

Go:   time.Now()
来源：http://ut.jctech888.com.cn

Ruby: Time.now
来源：http://pg.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ck.shxzskj.cn

[J02] 格式化输出
来源：http://er.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cb.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tn.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ss.wgjwhj.cn

TS:   d.toISOString()
来源：http://cy.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rg.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wz.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mq.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wy.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://xr.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kq.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xb.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://du.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://sy.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ld.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ij.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://nx.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xr.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://sy.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wi.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ht.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gk.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ea.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lr.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vp.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xl.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hf.521024.cn

[J05] 时间加减（加 7 天）
来源：http://ac.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://yw.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kb.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xn.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wa.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://vl.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bw.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://me.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bw.huixiangedu.cn

[J06] 计算两时间之差
来源：http://yd.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://lb.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://an.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yt.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ft.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ps.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://yx.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://cl.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://gl.9csxet.cn

[J07] 比较两个日期
来源：http://kf.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://by.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ur.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wm.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yi.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ie.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gj.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cm.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://fd.gzmigu.cn

[J08] 提取年月日与星期
来源：http://hy.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hp.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rt.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pb.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ud.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tg.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jv.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gi.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://py.lnxyls.cn

[J09] 时区处理
来源：http://vx.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ph.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://so.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rf.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tj.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dm.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ee.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xh.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hi.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://px.huanxung.cn


<!-- 参考信息 -->