代发 wailian999

JS:   get name() { return this._name; }
来源：http://mo.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://xi.nicolike.cn

Java: public String getName() { return name; }
来源：http://jy.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mp.shxzukj.cn

Ruby: attr_accessor :name
来源：http://ss.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://gn.hahajie.cn

[G12] 对象转字符串
来源：http://la.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://bl.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ht.szsharing.cn

JS:   toString() { return this.name; }
来源：http://vt.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://xr.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://jk.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pl.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://qq.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://sh.nszjky.cn

[G13] 判断对象类型
来源：http://zc.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://eo.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://gi.huixiangedu.cn

JS:   u instanceof User
来源：http://pc.chemitech.net.cn

TS:   u instanceof User
来源：http://xq.shtwfgs.cn

Java: u instanceof User
来源：http://ve.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iu.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://nd.lnxyls.cn

C#:   u is User
来源：http://qz.9csxet.cn

[G14] 数据类 / record
来源：http://tb.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://se.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://aq.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ih.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://pb.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://og.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://lo.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lw.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://yj.wgjwhj.cn

[G15] 枚举
来源：http://ui.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cm.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dc.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qx.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://en.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://xs.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yb.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://rf.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vq.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://mp.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uz.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://bc.asd995.cn

JS:   Object.entries(obj)
来源：http://tc.asd995.cn

TS:   Object.entries(obj)
来源：http://kq.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sq.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mu.shxzskj.cn

Ruby: obj.instance_variables
来源：http://id.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://bk.jianghongdianzi.cn

================================================================================
来源：http://qf.colortex.cn

H. 异常与错误处理
来源：http://ej.jctech888.com.cn

================================================================================
来源：http://qf.hnjuh.cn

[H01] try / catch 基础
来源：http://fk.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tn.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mp.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xm.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mf.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fi.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ai.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ay.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://an.521024.cn

[H02] finally / ensure 收尾
来源：http://mb.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xe.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zf.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cg.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oz.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qd.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yw.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tr.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dx.newstarts.cn

[H03] 主动抛出异常
来源：http://zi.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://wg.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vv.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://dk.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://vy.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ae.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rj.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lr.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zg.hahajie.cn

[H04] 自定义异常类型
来源：http://cp.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://oz.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tz.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://by.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://su.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://xg.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qe.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://wj.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://hj.panjiajie.cn

[H05] 捕获特定类型
来源：http://ui.colortex.cn

Py:   except ValueError as e:
来源：http://zg.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ge.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://hn.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://fl.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://dw.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ed.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://ch.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hh.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://od.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://fz.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zp.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tc.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://px.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tl.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ct.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://mv.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://qg.yuexingan06.cn

[H07] 断言
来源：http://gd.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://so.szsharing.cn

PHP:  assert($x > 0);
来源：http://sr.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://sj.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://kp.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://sv.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bt.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ko.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://zo.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://fo.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://tb.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ly.panjiajie.cn

JS:   e.message;  e.stack
来源：http://sd.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://by.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ig.szxytkj.cn

Go:   err.Error()
来源：http://cb.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://el.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://yn.lnxyls.cn

[H09] 带错误码的异常
来源：http://mr.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nt.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mc.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jc.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rm.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cx.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pa.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sj.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://af.lnxyls.cn

[H10] 资源自动释放
来源：http://xu.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lw.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xk.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dg.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mf.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yl.jctech888.com.cn

Go:   defer f.Close()
来源：http://gj.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ei.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yn.hahajie.cn

================================================================================
来源：http://qj.yuexingan06.cn

I. 正则表达式
来源：http://xr.jianghongdianzi.cn

================================================================================
来源：http://nr.asd995.cn

[I01] 判断是否匹配
来源：http://ks.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://so.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ck.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://sw.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://eo.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kh.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gk.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://qc.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nq.szsharing.cn

[I02] 提取所有匹配
来源：http://ub.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://dg.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xl.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gy.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://ub.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fq.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pz.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://be.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cp.shtwfgs.cn

[I03] 提取捕获分组
来源：http://ii.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yz.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ub.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bb.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hi.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kk.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ci.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cz.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eg.shxzskj.cn

[I04] 正则替换
来源：http://ei.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aa.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gf.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oy.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eb.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yb.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hl.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rr.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ji.haigaiapp.cn

[I05] 按正则拆分
来源：http://no.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yx.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dq.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://mw.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://se.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://tc.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cc.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ec.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rr.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bk.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tc.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ek.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wm.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ov.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ta.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hd.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fv.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ao.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://sk.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qk.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://be.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://at.muxihuayi.cn

TS:   /error/gim
来源：http://li.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sg.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ga.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://ws.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pu.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://km.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hy.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jk.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ve.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://on.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ji.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dh.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ip.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mt.lnxyls.cn

================================================================================
来源：http://aa.521024.cn

J. 日期与时间
来源：http://um.shxzukj.cn

================================================================================
来源：http://qf.szxytkj.cn

[J01] 获取当前时间
来源：http://jl.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cv.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ve.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://kx.huanxung.cn

TS:   new Date();  Date.now()
来源：http://du.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ci.panjiajie.cn

Go:   time.Now()
来源：http://vo.huixinmuqiang.cn

Ruby: Time.now
来源：http://hq.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tl.asd995.cn

[J02] 格式化输出
来源：http://kg.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cf.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fj.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aw.lnxyls.cn

TS:   d.toISOString()
来源：http://vj.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wo.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vo.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ir.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lw.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://pl.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lm.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hf.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://zd.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://le.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jm.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ve.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://wg.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wp.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://ys.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bw.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jy.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://if.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pt.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uj.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ja.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fp.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vx.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://ci.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://py.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gm.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yt.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xo.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://qt.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vq.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://rt.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pe.shtwfgs.cn

[J06] 计算两时间之差
来源：http://jz.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://wc.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://yl.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bq.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://po.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jh.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://wp.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://ih.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://gz.jctech888.com.cn

[J07] 比较两个日期
来源：http://hm.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://wg.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lu.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uh.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xm.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vm.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gv.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ep.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://mw.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://qt.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ow.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ve.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hr.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ti.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rj.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pp.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ci.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://am.521024.cn

[J09] 时区处理
来源：http://qc.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sa.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sh.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yp.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tq.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nv.huanxung.cn


<!-- 参考信息 -->