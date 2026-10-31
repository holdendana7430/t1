代发 wailian999

C#:   public / protected / private / internal
来源：http://ly.szxytkj.cn

[G11] getter / setter
来源：http://lu.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://gx.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gt.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://bd.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://cf.newstarts.cn

Java: public String getName() { return name; }
来源：http://jx.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jw.newstarts.cn

Ruby: attr_accessor :name
来源：http://pb.szsharing.cn

C#:   public string Name { get; set; }
来源：http://tm.huanxung.cn

[G12] 对象转字符串
来源：http://yu.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://gv.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vv.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://uc.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://me.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://mq.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://va.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://jq.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://zk.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://ij.nicolike.cn

Py:   isinstance(u, User)
来源：http://qj.panjiajie.cn

PHP:  $u instanceof User
来源：http://yp.panjiajie.cn

JS:   u instanceof User
来源：http://xe.newstarts.cn

TS:   u instanceof User
来源：http://ah.nicolike.cn

Java: u instanceof User
来源：http://eq.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ab.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://pj.muxihuayi.cn

C#:   u is User
来源：http://th.nicolike.cn

[G14] 数据类 / record
来源：http://bk.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dn.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://bt.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rx.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://gg.521024.cn

Java: record User(String name, int age) {}
来源：http://nt.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://ho.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hq.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://pv.huanxung.cn

[G15] 枚举
来源：http://zb.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://of.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://id.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vn.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wx.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://bs.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aj.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://yt.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nc.521024.cn

[G16] 对象转数组 / 字典
来源：http://xz.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jg.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://lz.szsharing.cn

JS:   Object.entries(obj)
来源：http://sc.9csxet.cn

TS:   Object.entries(obj)
来源：http://vc.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nb.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://am.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://wc.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://dt.chemitech.net.cn

================================================================================
来源：http://no.asd995.cn

H. 异常与错误处理
来源：http://jl.521024.cn

================================================================================
来源：http://sk.shxzukj.cn

[H01] try / catch 基础
来源：http://vd.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bv.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qh.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jp.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lq.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qs.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fo.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pt.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uv.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://xq.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ub.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vw.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sw.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vb.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yd.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dg.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cy.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mu.haigaiapp.cn

[H03] 主动抛出异常
来源：http://kz.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://bi.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yw.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://rq.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://sk.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uv.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iu.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xk.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jh.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://lt.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://zh.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rv.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://ti.szsharing.cn

TS:   class MyError extends Error {}
来源：http://zo.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ph.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tp.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://ui.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://ku.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://xj.hnjuh.cn

Py:   except ValueError as e:
来源：http://vr.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wu.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://ek.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://hf.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://sv.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zp.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://dk.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ir.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://vd.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://wl.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cw.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ke.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zm.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oc.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lc.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://jc.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://tx.shtwfgs.cn

[H07] 断言
来源：http://la.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://vn.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://by.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://nz.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://is.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://ul.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dy.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eu.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://td.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://ve.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://wk.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ee.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://bo.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ua.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ve.shxzukj.cn

Go:   err.Error()
来源：http://yu.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://mf.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://or.huixiangedu.cn

[H09] 带错误码的异常
来源：http://bd.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mp.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zv.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tr.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tq.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qh.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oj.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zh.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ck.colortex.cn

[H10] 资源自动释放
来源：http://gp.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lx.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dk.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dv.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ef.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tt.huixiangedu.cn

Go:   defer f.Close()
来源：http://aw.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pb.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gf.haigaiapp.cn

================================================================================
来源：http://gb.jctech888.com.cn

I. 正则表达式
来源：http://yf.hahajie.cn

================================================================================
来源：http://kx.asd995.cn

[I01] 判断是否匹配
来源：http://lm.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cf.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cd.huanxung.cn

JS:   /\d+/.test(s)
来源：http://pp.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://uk.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ah.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ul.521024.cn

Ruby: s.match?(/\d+/)
来源：http://yg.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ct.nszjky.cn

[I02] 提取所有匹配
来源：http://ig.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://zo.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ff.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://an.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://ka.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gl.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xb.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://if.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.newstarts.cn

[I03] 提取捕获分组
来源：http://xh.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yh.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ps.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wm.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ea.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fi.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bq.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lc.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uq.haigaiapp.cn

[I04] 正则替换
来源：http://la.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tf.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yn.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gb.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kn.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://un.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kt.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xk.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://of.shxzskj.cn

[I05] 按正则拆分
来源：http://af.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ys.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mv.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://ln.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://pi.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://sk.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nx.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bi.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ht.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cw.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ho.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://it.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sp.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dg.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kd.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://en.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://md.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yd.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://km.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fj.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://id.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://df.9csxet.cn

TS:   /error/gim
来源：http://ag.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://js.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xy.asd995.cn

Ruby: s.scan(/error/i)
来源：http://qq.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nw.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://ay.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fc.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pn.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eu.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uh.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hm.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cs.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ku.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ly.shtwfgs.cn

================================================================================
来源：http://hq.hnjuh.cn

J. 日期与时间
来源：http://dj.asd995.cn

================================================================================
来源：http://jl.shxzukj.cn

[J01] 获取当前时间
来源：http://ud.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://za.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wf.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://lw.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://yf.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mt.hnjuh.cn

Go:   time.Now()
来源：http://tl.shxzskj.cn

Ruby: Time.now
来源：http://ji.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tx.jctech888.com.cn

[J02] 格式化输出
来源：http://gp.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oh.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ep.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pm.hnjuh.cn

TS:   d.toISOString()
来源：http://ma.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cd.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qz.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ir.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lv.newstarts.cn

[J03] 字符串解析为日期
来源：http://cf.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://az.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cy.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://tk.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://uv.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://od.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yn.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://kh.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qy.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://im.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ie.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bj.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yu.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ip.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qb.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ru.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tt.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qs.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://un.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://ve.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dv.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lz.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zt.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://ux.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ik.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://qi.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://au.hahajie.cn

[J06] 计算两时间之差
来源：http://es.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://pi.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://il.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zm.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fp.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eh.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://ta.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://dt.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://eu.shxzukj.cn

[J07] 比较两个日期
来源：http://mk.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://bn.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zh.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ox.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://et.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qg.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yz.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xq.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://sc.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://nb.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nn.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bo.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dz.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://um.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kz.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rq.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wz.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mw.szsharing.cn

[J09] 时区处理
来源：http://zd.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ur.wgjwhj.cn


<!-- 参考信息 -->