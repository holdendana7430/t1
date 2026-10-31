代发 wailian999

TS:   public / protected / private
来源：http://ib.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://be.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vg.asd995.cn

Ruby: public / protected / private
来源：http://ho.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://bs.huixinmuqiang.cn

[G11] getter / setter
来源：http://zv.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://ho.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://td.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://wd.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://jl.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://ic.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://py.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://kw.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://vx.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://nk.colortex.cn

Py:   def __str__(self): return self.name
来源：http://la.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qy.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://co.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://qi.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://gv.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ht.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://jr.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://gh.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://gk.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://eg.shtwfgs.cn

PHP:  $u instanceof User
来源：http://tp.asd995.cn

JS:   u instanceof User
来源：http://lh.nicolike.cn

TS:   u instanceof User
来源：http://ru.shtwfgs.cn

Java: u instanceof User
来源：http://yv.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nf.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://se.nszjky.cn

C#:   u is User
来源：http://kt.huixiangedu.cn

[G14] 数据类 / record
来源：http://fq.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ma.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://jf.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ys.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://rm.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://bs.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://hb.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gw.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://yf.panjiajie.cn

[G15] 枚举
来源：http://vr.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zo.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oy.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zz.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://co.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://zj.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jn.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://py.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ng.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://pl.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hs.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://sv.521024.cn

JS:   Object.entries(obj)
来源：http://bj.szxytkj.cn

TS:   Object.entries(obj)
来源：http://ot.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bw.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gz.nicolike.cn

Ruby: obj.instance_variables
来源：http://jz.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://nl.panjiajie.cn

================================================================================
来源：http://md.jctech888.com.cn

H. 异常与错误处理
来源：http://ea.panjiajie.cn

================================================================================
来源：http://am.chemitech.net.cn

[H01] try / catch 基础
来源：http://va.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pl.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bd.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fu.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cu.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uz.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vo.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uc.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bx.9csxet.cn

[H02] finally / ensure 收尾
来源：http://li.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mb.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lr.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://df.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ou.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zh.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ml.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ay.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dv.jctech888.com.cn

[H03] 主动抛出异常
来源：http://wt.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://mg.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ij.colortex.cn

JS:   throw new Error("错误信息");
来源：http://hz.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://fn.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cw.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gm.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bf.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://va.chemitech.net.cn

[H04] 自定义异常类型
来源：http://sv.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://qk.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yr.nicolike.cn

JS:   class MyError extends Error {}
来源：http://fv.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://uu.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://jx.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ji.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://an.asd995.cn

C#:   class MyException : Exception {}
来源：http://hv.521024.cn

[H05] 捕获特定类型
来源：http://iq.hnjuh.cn

Py:   except ValueError as e:
来源：http://ld.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lp.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://jb.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://zy.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://ka.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ge.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://tn.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ij.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://te.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://qs.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://da.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wu.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oy.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://am.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dt.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://qu.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://xv.asd995.cn

[H07] 断言
来源：http://np.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://di.nicolike.cn

PHP:  assert($x > 0);
来源：http://mg.nszjky.cn

JS:   console.assert(x > 0);
来源：http://op.521024.cn

TS:   console.assert(x > 0);
来源：http://en.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://rv.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cl.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ko.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://uu.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://tn.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://si.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ph.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://ft.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ga.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oz.gzmigu.cn

Go:   err.Error()
来源：http://ba.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://ry.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://hx.nicolike.cn

[H09] 带错误码的异常
来源：http://dg.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wq.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ro.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kb.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ec.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ww.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fx.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xi.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yw.huanxung.cn

[H10] 资源自动释放
来源：http://le.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://py.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ix.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mm.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jj.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lg.huanxung.cn

Go:   defer f.Close()
来源：http://px.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fb.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ho.nicolike.cn

================================================================================
来源：http://th.yuntaijiaju.cn

I. 正则表达式
来源：http://wu.asd995.cn

================================================================================
来源：http://qc.lnxyls.cn

[I01] 判断是否匹配
来源：http://sf.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jo.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gj.nicolike.cn

JS:   /\d+/.test(s)
来源：http://zy.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://xy.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nr.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://em.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://re.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aj.hnjuh.cn

[I02] 提取所有匹配
来源：http://rk.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://bt.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zy.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fr.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://mu.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dr.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zi.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://iv.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rt.asd995.cn

[I03] 提取捕获分组
来源：http://hd.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kf.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sq.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gy.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://le.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oo.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ke.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ef.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rk.shtwfgs.cn

[I04] 正则替换
来源：http://hm.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fg.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wb.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wt.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://po.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hg.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rw.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://im.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wk.shtwfgs.cn

[I05] 按正则拆分
来源：http://oz.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ls.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eu.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://db.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://zh.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://fx.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ex.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ky.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rx.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ij.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nu.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yy.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ml.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fu.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://br.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ra.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fg.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://al.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://mk.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fp.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ns.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bn.521024.cn

TS:   /error/gim
来源：http://me.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ts.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tn.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://qy.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hh.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://cx.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ep.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ax.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://df.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rx.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ot.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fj.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uz.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tl.huixiangedu.cn

================================================================================
来源：http://pt.huixinmuqiang.cn

J. 日期与时间
来源：http://ca.bjjhwx.cn

================================================================================
来源：http://cq.521024.cn

[J01] 获取当前时间
来源：http://sd.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ot.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lt.521024.cn

JS:   new Date();  Date.now()
来源：http://vn.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://jh.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ry.huixinmuqiang.cn

Go:   time.Now()
来源：http://ny.szxytkj.cn

Ruby: Time.now
来源：http://vq.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yf.huixiangedu.cn

[J02] 格式化输出
来源：http://lf.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mg.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fb.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wo.bjjhwx.cn

TS:   d.toISOString()
来源：http://ct.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ye.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tg.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ok.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://te.nicolike.cn

[J03] 字符串解析为日期
来源：http://di.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aa.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ex.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://ko.521024.cn

TS:   new Date("2024-01-02")
来源：http://su.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qb.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gb.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://ei.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ms.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://fg.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tb.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oj.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aj.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oy.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iy.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sq.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jl.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fa.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://vp.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://sp.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ee.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jh.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ob.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://rx.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sm.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://db.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://om.shxzskj.cn

[J06] 计算两时间之差
来源：http://ks.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://vs.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://tw.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ul.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://da.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uj.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://hj.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://qk.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://vq.gzmigu.cn

[J07] 比较两个日期
来源：http://ue.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://qn.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://za.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kk.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zo.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uu.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xy.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ts.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://ct.szsharing.cn

[J08] 提取年月日与星期
来源：http://yf.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gg.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vy.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pv.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ce.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cv.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ht.yuntaijiaju.cn


<!-- 参考信息 -->