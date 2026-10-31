代发 wailian999

Java: interface Shape { double area(); }
来源：http://ot.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://cd.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cc.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://eg.nszjky.cn

[G10] 访问控制
来源：http://df.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://uq.hnjuh.cn

PHP:  public / protected / private
来源：http://zn.nszjky.cn

JS:   #private 字段；其余公开
来源：http://vz.jianghongdianzi.cn

TS:   public / protected / private
来源：http://dc.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://xq.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uf.wgjwhj.cn

Ruby: public / protected / private
来源：http://pw.9csxet.cn

C#:   public / protected / private / internal
来源：http://yh.asd995.cn

[G11] getter / setter
来源：http://mo.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://oj.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bo.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://hz.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://fj.szsharing.cn

Java: public String getName() { return name; }
来源：http://qa.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yx.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://tt.9csxet.cn

C#:   public string Name { get; set; }
来源：http://yl.shtwfgs.cn

[G12] 对象转字符串
来源：http://yc.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://of.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://er.9csxet.cn

JS:   toString() { return this.name; }
来源：http://vz.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://ku.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://sc.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tr.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://bx.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://vb.lnxyls.cn

[G13] 判断对象类型
来源：http://nu.gzmigu.cn

Py:   isinstance(u, User)
来源：http://wl.lnxyls.cn

PHP:  $u instanceof User
来源：http://gp.panjiajie.cn

JS:   u instanceof User
来源：http://yq.bookmarksfly.cn

TS:   u instanceof User
来源：http://mr.haigaiapp.cn

Java: u instanceof User
来源：http://vy.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qi.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://ov.hahajie.cn

C#:   u is User
来源：http://wr.haigaiapp.cn

[G14] 数据类 / record
来源：http://ca.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qg.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://mh.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bm.521024.cn

TS:   type User = { name: string; age: number };
来源：http://ah.asd995.cn

Java: record User(String name, int age) {}
来源：http://de.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://vi.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kq.521024.cn

C#:   record User(string Name, int Age);
来源：http://fs.nszjky.cn

[G15] 枚举
来源：http://hy.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pj.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ij.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cv.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zr.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://ey.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tq.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://bx.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nk.521024.cn

[G16] 对象转数组 / 字典
来源：http://ru.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://va.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://ww.shxzskj.cn

JS:   Object.entries(obj)
来源：http://qs.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://sg.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xo.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mw.9csxet.cn

Ruby: obj.instance_variables
来源：http://fm.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://fk.yuntaijiaju.cn

================================================================================
来源：http://wh.haigaiapp.cn

H. 异常与错误处理
来源：http://eb.bjjhwx.cn

================================================================================
来源：http://au.newstarts.cn

[H01] try / catch 基础
来源：http://xf.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nm.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://of.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nz.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ix.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kf.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hh.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lm.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://is.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://fo.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tj.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yf.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zj.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wh.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ep.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ve.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hf.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ty.muxihuayi.cn

[H03] 主动抛出异常
来源：http://sj.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://fx.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yd.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://fz.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://mm.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yq.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dd.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://us.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zv.hnjuh.cn

[H04] 自定义异常类型
来源：http://sn.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://zj.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://up.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://yl.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://fm.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://ss.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pp.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://xs.9csxet.cn

C#:   class MyException : Exception {}
来源：http://tk.wgjwhj.cn

[H05] 捕获特定类型
来源：http://mj.newstarts.cn

Py:   except ValueError as e:
来源：http://uc.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mr.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://sw.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ww.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://av.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fx.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://vg.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cf.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://hp.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://fm.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ev.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oj.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cr.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ec.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dg.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://da.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://og.jctech888.com.cn

[H07] 断言
来源：http://au.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://gh.gzmigu.cn

PHP:  assert($x > 0);
来源：http://hi.521024.cn

JS:   console.assert(x > 0);
来源：http://bo.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://fi.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://uf.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ad.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ug.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://mi.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://qi.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://tk.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nm.szxytkj.cn

JS:   e.message;  e.stack
来源：http://jd.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cz.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ge.muxihuayi.cn

Go:   err.Error()
来源：http://hz.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://zt.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://pt.haigaiapp.cn

[H09] 带错误码的异常
来源：http://dj.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sz.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qb.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rp.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jj.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uk.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bu.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bx.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iv.shxzukj.cn

[H10] 资源自动释放
来源：http://vk.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://as.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://af.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ne.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vp.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kp.szxytkj.cn

Go:   defer f.Close()
来源：http://xz.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wi.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nv.shtwfgs.cn

================================================================================
来源：http://hf.newstarts.cn

I. 正则表达式
来源：http://jt.lnxyls.cn

================================================================================
来源：http://pm.jctech888.com.cn

[I01] 判断是否匹配
来源：http://yb.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ip.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hc.huanxung.cn

JS:   /\d+/.test(s)
来源：http://kk.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://br.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ja.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jw.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://hj.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ch.muxihuayi.cn

[I02] 提取所有匹配
来源：http://we.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://lo.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ck.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sw.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://if.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://en.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ri.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://ak.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zz.hnjuh.cn

[I03] 提取捕获分组
来源：http://wa.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fl.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tr.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vr.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vg.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://df.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ng.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hp.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iy.521024.cn

[I04] 正则替换
来源：http://th.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rz.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lm.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ti.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ng.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tx.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sm.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ga.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://df.panjiajie.cn

[I05] 按正则拆分
来源：http://po.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sj.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://om.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://tm.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://et.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://he.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://az.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sa.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aa.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kg.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wb.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qy.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cx.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gm.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ck.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rs.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jz.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ff.521024.cn

[I07] 忽略大小写与多行模式
来源：http://vz.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://in.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ja.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rz.asd995.cn

TS:   /error/gim
来源：http://ln.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mr.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rj.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://qo.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qa.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://wl.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tm.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sg.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ps.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yw.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ni.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jm.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ql.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uc.nszjky.cn

================================================================================
来源：http://nt.nicolike.cn

J. 日期与时间
来源：http://jd.panjiajie.cn

================================================================================
来源：http://ps.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://tt.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yr.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nz.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://vs.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://tn.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ta.yuexingan06.cn

Go:   time.Now()
来源：http://kb.bookmarksfly.cn

Ruby: Time.now
来源：http://ln.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://if.yuntaijiaju.cn

[J02] 格式化输出
来源：http://mm.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://di.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mx.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://td.gzmigu.cn

TS:   d.toISOString()
来源：http://lv.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ix.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iy.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mo.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ng.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://ue.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xf.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vk.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://fs.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://kj.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mn.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ya.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://pl.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zz.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://ji.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lq.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pe.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ev.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zk.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kx.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oy.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pk.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ru.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://lf.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://wh.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ay.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yy.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nd.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://dj.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dh.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://nb.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zf.szsharing.cn

[J06] 计算两时间之差
来源：http://dx.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://vm.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://lx.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yu.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xn.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hr.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://pi.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://lw.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://ed.jctech888.com.cn

[J07] 比较两个日期
来源：http://oo.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://zv.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mk.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ob.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uj.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aw.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pf.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gl.huixinmuqiang.cn


<!-- 参考信息 -->