代发 wailian999

JS:   get name() { return this._name; }
来源：http://pq.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://ni.gzmigu.cn

Java: public String getName() { return name; }
来源：http://qb.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zm.shxzukj.cn

Ruby: attr_accessor :name
来源：http://tg.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://gk.9csxet.cn

[G12] 对象转字符串
来源：http://ya.asd995.cn

Py:   def __str__(self): return self.name
来源：http://vc.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kv.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://zm.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://gb.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://rp.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cd.colortex.cn

Ruby: def to_s; @name; end
来源：http://ka.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://xr.huanxung.cn

[G13] 判断对象类型
来源：http://yu.hnjuh.cn

Py:   isinstance(u, User)
来源：http://ih.szsharing.cn

PHP:  $u instanceof User
来源：http://lt.nszjky.cn

JS:   u instanceof User
来源：http://aw.jctech888.com.cn

TS:   u instanceof User
来源：http://iq.newstarts.cn

Java: u instanceof User
来源：http://gr.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://af.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://jo.9csxet.cn

C#:   u is User
来源：http://he.bookmarksfly.cn

[G14] 数据类 / record
来源：http://db.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zd.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://xx.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://el.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://ls.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://hx.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://hc.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gd.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://wd.gzmigu.cn

[G15] 枚举
来源：http://um.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lw.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jl.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kb.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://la.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://yb.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vp.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://rl.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://az.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://uf.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mo.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://ib.shxzukj.cn

JS:   Object.entries(obj)
来源：http://nk.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://as.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xy.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ss.newstarts.cn

Ruby: obj.instance_variables
来源：http://cv.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://dy.asd995.cn

================================================================================
来源：http://vz.shxzukj.cn

H. 异常与错误处理
来源：http://ok.gzmigu.cn

================================================================================
来源：http://cy.wgjwhj.cn

[H01] try / catch 基础
来源：http://ca.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xu.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zt.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wf.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pz.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yg.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mr.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ds.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mr.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://mh.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tp.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jr.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ws.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xj.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ty.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gk.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vi.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ci.shtwfgs.cn

[H03] 主动抛出异常
来源：http://iq.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://to.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rg.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://bg.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://cv.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ay.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://es.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cr.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lr.521024.cn

[H04] 自定义异常类型
来源：http://hj.521024.cn

Py:   class MyError(Exception): pass
来源：http://ya.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rp.521024.cn

JS:   class MyError extends Error {}
来源：http://mo.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://ou.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://qd.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://co.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://oz.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://mx.szxytkj.cn

[H05] 捕获特定类型
来源：http://mv.yuexingan06.cn

Py:   except ValueError as e:
来源：http://xe.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ak.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://rh.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://bh.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://ur.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pn.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://mp.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lb.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://ue.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://iy.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://we.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qw.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tk.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ke.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qs.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://fb.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://mt.hnjuh.cn

[H07] 断言
来源：http://fm.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://jk.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://wq.hahajie.cn

JS:   console.assert(x > 0);
来源：http://qg.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://ml.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://wy.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bp.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cu.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://me.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://vy.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://fr.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ej.gzmigu.cn

JS:   e.message;  e.stack
来源：http://ri.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cr.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hj.hnjuh.cn

Go:   err.Error()
来源：http://ff.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://cs.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://bo.panjiajie.cn

[H09] 带错误码的异常
来源：http://ra.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hq.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ti.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ug.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://as.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ou.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dk.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nr.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vb.521024.cn

[H10] 资源自动释放
来源：http://wz.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zh.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hh.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cn.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://al.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://re.asd995.cn

Go:   defer f.Close()
来源：http://us.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wz.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mo.jianghongdianzi.cn

================================================================================
来源：http://ib.shxzukj.cn

I. 正则表达式
来源：http://wm.haigaiapp.cn

================================================================================
来源：http://cm.shtwfgs.cn

[I01] 判断是否匹配
来源：http://wt.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nm.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vd.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://fo.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://ie.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ng.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bf.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://yq.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wv.szxytkj.cn

[I02] 提取所有匹配
来源：http://fn.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://xr.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cw.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kl.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://sm.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cs.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ft.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://jp.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ji.9csxet.cn

[I03] 提取捕获分组
来源：http://wt.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lg.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ns.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yg.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://by.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aw.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qu.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hf.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xi.yuntaijiaju.cn

[I04] 正则替换
来源：http://bt.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vc.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://or.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kv.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dj.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bf.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oi.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xp.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gp.shxzskj.cn

[I05] 按正则拆分
来源：http://jv.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sc.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kx.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://hi.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://yo.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://qn.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ta.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ao.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rf.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://na.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ms.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nu.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vv.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wp.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gb.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zg.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xx.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jf.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://sb.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yd.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rq.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iu.shxzskj.cn

TS:   /error/gim
来源：http://jb.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ts.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yg.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://lh.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rb.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://yx.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wm.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sp.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://di.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://la.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://br.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ng.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kr.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://he.gzmigu.cn

================================================================================
来源：http://wb.shxzukj.cn

J. 日期与时间
来源：http://bw.jctech888.com.cn

================================================================================
来源：http://xz.nszjky.cn

[J01] 获取当前时间
来源：http://nt.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://va.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jz.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://pi.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://di.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://og.szsharing.cn

Go:   time.Now()
来源：http://yu.yuntaijiaju.cn

Ruby: Time.now
来源：http://tu.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qk.gzmigu.cn

[J02] 格式化输出
来源：http://ve.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jk.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ap.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qr.bookmarksfly.cn

TS:   d.toISOString()
来源：http://gm.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zs.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cz.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bz.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hp.nicolike.cn

[J03] 字符串解析为日期
来源：http://pj.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xq.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://in.colortex.cn

JS:   new Date("2024-01-02")
来源：http://vr.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://ai.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vt.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cl.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://nd.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mh.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://co.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iu.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dj.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vh.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fm.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ur.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yp.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yw.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wk.521024.cn

[J05] 时间加减（加 7 天）
来源：http://nm.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://ng.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yv.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bz.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lq.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://tw.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://az.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://pb.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ax.lnxyls.cn

[J06] 计算两时间之差
来源：http://cx.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://ot.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://xx.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nd.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ce.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://it.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://sv.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://wz.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://be.muxihuayi.cn

[J07] 比较两个日期
来源：http://dt.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://fh.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://md.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vb.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ib.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qd.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tc.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vx.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://ag.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://dp.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tp.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wv.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ah.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ln.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gc.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ja.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zf.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yd.colortex.cn

[J09] 时区处理
来源：http://uq.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yn.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wk.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ay.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fi.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ab.521024.cn


<!-- 参考信息 -->