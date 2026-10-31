代发 wailian999

JS:   get name() { return this._name; }
来源：http://rt.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://sv.hnjuh.cn

Java: public String getName() { return name; }
来源：http://fe.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gn.shxzukj.cn

Ruby: attr_accessor :name
来源：http://ir.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://rp.shtwfgs.cn

[G12] 对象转字符串
来源：http://du.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://qh.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rp.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://oi.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://zk.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://il.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ur.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://pd.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://cx.asd995.cn

[G13] 判断对象类型
来源：http://uv.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://yc.muxihuayi.cn

PHP:  $u instanceof User
来源：http://fc.nicolike.cn

JS:   u instanceof User
来源：http://hb.panjiajie.cn

TS:   u instanceof User
来源：http://af.wgjwhj.cn

Java: u instanceof User
来源：http://vo.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hb.521024.cn

Ruby: u.is_a?(User)
来源：http://ib.gzmigu.cn

C#:   u is User
来源：http://ds.hnjuh.cn

[G14] 数据类 / record
来源：http://ji.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bb.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://qe.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lv.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://ry.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://wu.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://vb.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lk.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://oe.yuexingan06.cn

[G15] 枚举
来源：http://om.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nz.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gg.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mc.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jn.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://fm.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ro.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://mp.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zf.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://nm.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ph.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://pj.hnjuh.cn

JS:   Object.entries(obj)
来源：http://bk.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://bd.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pg.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://de.gzmigu.cn

Ruby: obj.instance_variables
来源：http://el.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://nh.shxzukj.cn

================================================================================
来源：http://rc.521024.cn

H. 异常与错误处理
来源：http://hu.lnxyls.cn

================================================================================
来源：http://na.lnxyls.cn

[H01] try / catch 基础
来源：http://sn.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kx.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bm.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aa.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ho.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bn.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rm.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ye.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ri.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://ko.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ua.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pn.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bq.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qn.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jw.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eh.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fi.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ww.panjiajie.cn

[H03] 主动抛出异常
来源：http://ua.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://jy.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rg.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://yk.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://he.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dj.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bp.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fq.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ab.panjiajie.cn

[H04] 自定义异常类型
来源：http://xj.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://io.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bi.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://nf.szsharing.cn

TS:   class MyError extends Error {}
来源：http://qq.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://mk.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pr.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://ea.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://yq.szxytkj.cn

[H05] 捕获特定类型
来源：http://tk.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://hs.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vz.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://pf.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://gm.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://ek.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zp.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://yb.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gm.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://zh.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://mv.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dw.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ap.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fs.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yg.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ik.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://ge.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://cj.yuexingan06.cn

[H07] 断言
来源：http://xk.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://zu.colortex.cn

PHP:  assert($x > 0);
来源：http://hi.szsharing.cn

JS:   console.assert(x > 0);
来源：http://as.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://kt.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://jz.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mc.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zr.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://wq.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://th.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://fe.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mr.szsharing.cn

JS:   e.message;  e.stack
来源：http://ec.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sa.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ei.huixinmuqiang.cn

Go:   err.Error()
来源：http://ec.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://kh.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://ta.huanxung.cn

[H09] 带错误码的异常
来源：http://ke.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bk.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ls.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ug.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nc.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hn.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bf.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pt.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rd.hnjuh.cn

[H10] 资源自动释放
来源：http://xy.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ek.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yb.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ep.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ra.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ef.wgjwhj.cn

Go:   defer f.Close()
来源：http://dg.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://et.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nb.9csxet.cn

================================================================================
来源：http://cb.jctech888.com.cn

I. 正则表达式
来源：http://rs.newstarts.cn

================================================================================
来源：http://ay.wgjwhj.cn

[I01] 判断是否匹配
来源：http://ox.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://he.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yw.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://ip.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://jf.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wl.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://re.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://bv.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://el.hnjuh.cn

[I02] 提取所有匹配
来源：http://lb.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://sg.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ad.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://in.colortex.cn

TS:   s.match(/\d+/g)
来源：http://fj.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ov.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wt.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://ch.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ps.panjiajie.cn

[I03] 提取捕获分组
来源：http://yq.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ks.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cq.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wo.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mi.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bf.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lv.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ib.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kq.panjiajie.cn

[I04] 正则替换
来源：http://wm.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xp.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eq.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rt.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xx.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ru.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wm.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qv.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vy.huanxung.cn

[I05] 按正则拆分
来源：http://kq.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dj.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://pl.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://ze.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://mh.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hq.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yl.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ij.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mg.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ng.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ok.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xy.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qq.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lp.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uq.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://od.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kq.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://pa.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ag.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qq.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wa.nicolike.cn

TS:   /error/gim
来源：http://qp.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gm.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sg.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://rl.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rb.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://zl.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yy.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qw.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rg.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kc.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mh.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bb.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://el.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fo.9csxet.cn

================================================================================
来源：http://jc.chemitech.net.cn

J. 日期与时间
来源：http://sl.wgjwhj.cn

================================================================================
来源：http://dc.colortex.cn

[J01] 获取当前时间
来源：http://dq.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rd.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vq.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://eo.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://cx.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dy.shxzskj.cn

Go:   time.Now()
来源：http://fd.yuexingan06.cn

Ruby: Time.now
来源：http://py.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bg.yuexingan06.cn

[J02] 格式化输出
来源：http://cm.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dx.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ox.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://it.huixiangedu.cn

TS:   d.toISOString()
来源：http://ws.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yj.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://li.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vk.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vy.9csxet.cn

[J03] 字符串解析为日期
来源：http://iv.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ik.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mx.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://vq.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://wl.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xa.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ot.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://dj.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ro.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://vf.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lc.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xc.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bv.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wf.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zr.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ge.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pr.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ig.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://xz.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://ei.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ce.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wq.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tc.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://up.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xj.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://lq.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ke.panjiajie.cn

[J06] 计算两时间之差
来源：http://vr.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://my.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://my.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ka.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ny.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uh.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://ev.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://tr.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://jm.shtwfgs.cn

[J07] 比较两个日期
来源：http://ub.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://zl.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jp.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xz.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rz.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dv.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ji.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lj.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://pa.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://yh.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ib.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ks.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ct.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kk.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pq.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rq.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gn.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jf.bjjhwx.cn

[J09] 时区处理
来源：http://dw.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yw.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sp.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ea.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ns.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ix.hahajie.cn


<!-- 参考信息 -->