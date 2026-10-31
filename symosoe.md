代发 wailian999

[G10] 访问控制
来源：http://ap.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://fe.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://gv.521024.cn

JS:   #private 字段；其余公开
来源：http://uy.yuexingan06.cn

TS:   public / protected / private
来源：http://pj.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://ex.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gh.panjiajie.cn

Ruby: public / protected / private
来源：http://qs.gzmigu.cn

C#:   public / protected / private / internal
来源：http://wn.nicolike.cn

[G11] getter / setter
来源：http://pr.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://dh.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iw.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://lg.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://mw.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://qq.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qw.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://jh.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://au.lnxyls.cn

[G12] 对象转字符串
来源：http://yh.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://ye.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jv.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://tb.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://cc.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://mj.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ri.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://wu.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://jk.521024.cn

[G13] 判断对象类型
来源：http://ip.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://yx.bjjhwx.cn

PHP:  $u instanceof User
来源：http://wy.jctech888.com.cn

JS:   u instanceof User
来源：http://jr.jctech888.com.cn

TS:   u instanceof User
来源：http://of.hahajie.cn

Java: u instanceof User
来源：http://ir.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://co.hahajie.cn

Ruby: u.is_a?(User)
来源：http://ah.nicolike.cn

C#:   u is User
来源：http://cf.jctech888.com.cn

[G14] 数据类 / record
来源：http://zm.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rw.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://za.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uq.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://yj.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://ac.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://fo.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xd.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://wc.asd995.cn

[G15] 枚举
来源：http://my.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mb.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sj.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yi.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gp.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://mn.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://og.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://ty.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fx.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://xd.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mg.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://oa.asd995.cn

JS:   Object.entries(obj)
来源：http://zl.shxzskj.cn

TS:   Object.entries(obj)
来源：http://ke.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ub.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oy.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://hs.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://bd.muxihuayi.cn

================================================================================
来源：http://ca.muxihuayi.cn

H. 异常与错误处理
来源：http://pl.jctech888.com.cn

================================================================================
来源：http://qh.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://wz.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oa.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zt.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lz.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hb.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zb.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mc.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tb.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://su.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://cn.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xn.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://et.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gj.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ds.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yv.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eu.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dc.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zw.hnjuh.cn

[H03] 主动抛出异常
来源：http://hp.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://pw.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pf.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://uv.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://jr.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://va.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gy.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jc.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yc.chemitech.net.cn

[H04] 自定义异常类型
来源：http://uf.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://xv.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ys.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://ia.521024.cn

TS:   class MyError extends Error {}
来源：http://pp.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://uk.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ui.521024.cn

Ruby: class MyError < StandardError; end
来源：http://jb.9csxet.cn

C#:   class MyException : Exception {}
来源：http://sg.shxzukj.cn

[H05] 捕获特定类型
来源：http://ml.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://vt.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mp.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://lz.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ln.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://ti.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zu.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://jh.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lc.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://og.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://ag.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pj.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kj.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://at.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tk.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fi.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://eq.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://ag.wgjwhj.cn

[H07] 断言
来源：http://ci.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://us.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://ns.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://ic.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://iv.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://tn.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gz.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sd.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://ow.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://bn.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://kz.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wl.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://lu.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kz.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xn.shxzskj.cn

Go:   err.Error()
来源：http://ot.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://wh.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://qj.hnjuh.cn

[H09] 带错误码的异常
来源：http://ap.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yz.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dv.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sq.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xs.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tk.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wu.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ta.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://og.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://oq.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pa.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qv.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mu.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xf.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ui.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://vg.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xf.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ue.nicolike.cn

================================================================================
来源：http://av.huanxung.cn

I. 正则表达式
来源：http://kc.yuexingan06.cn

================================================================================
来源：http://xv.521024.cn

[I01] 判断是否匹配
来源：http://kn.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://te.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://km.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://wj.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://ah.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cx.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://il.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://xj.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mq.haigaiapp.cn

[I02] 提取所有匹配
来源：http://hg.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://ep.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hc.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cy.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://ss.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bq.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://to.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://yp.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mk.chemitech.net.cn

[I03] 提取捕获分组
来源：http://dv.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wk.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pa.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ze.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bf.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fy.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iz.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ly.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://km.nicolike.cn

[I04] 正则替换
来源：http://gv.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uq.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xw.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kj.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bq.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://as.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uo.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ml.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aw.nicolike.cn

[I05] 按正则拆分
来源：http://po.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zu.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kk.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://hk.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://mc.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://lu.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cw.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bv.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qy.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dp.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ih.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zo.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jt.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jf.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tm.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yi.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wt.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kc.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://sq.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fn.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kx.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jt.hahajie.cn

TS:   /error/gim
来源：http://em.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://at.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ku.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://dw.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://db.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://lp.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wp.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xk.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jb.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://du.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zn.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vf.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ju.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tu.nszjky.cn

================================================================================
来源：http://mc.szsharing.cn

J. 日期与时间
来源：http://jx.nszjky.cn

================================================================================
来源：http://rf.bookmarksfly.cn

[J01] 获取当前时间
来源：http://tg.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pm.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pt.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://hw.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://fx.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lj.szsharing.cn

Go:   time.Now()
来源：http://fd.hahajie.cn

Ruby: Time.now
来源：http://xd.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ui.jianghongdianzi.cn

[J02] 格式化输出
来源：http://rw.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://we.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pu.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qe.haigaiapp.cn

TS:   d.toISOString()
来源：http://fd.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ad.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rg.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bn.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gb.hahajie.cn

[J03] 字符串解析为日期
来源：http://sd.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wt.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gu.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://ou.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://pv.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uq.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ai.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://wb.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ll.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://pu.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://th.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bh.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kj.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ou.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ea.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hc.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://po.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ep.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://tl.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://wi.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fe.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zp.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gx.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://qk.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://go.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://mv.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cd.huixiangedu.cn

[J06] 计算两时间之差
来源：http://dw.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://jo.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://ij.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mc.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lo.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ub.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://lv.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://kr.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://uq.haigaiapp.cn

[J07] 比较两个日期
来源：http://nm.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://nr.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dy.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ho.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rv.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cx.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fy.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pc.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://xe.colortex.cn

[J08] 提取年月日与星期
来源：http://bi.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rh.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ur.chemitech.net.cn


<!-- 参考信息 -->