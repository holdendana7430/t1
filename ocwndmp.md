代发 wailian999

[G10] 访问控制
来源：http://qn.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://it.muxihuayi.cn

PHP:  public / protected / private
来源：http://qs.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://dk.yuexingan06.cn

TS:   public / protected / private
来源：http://oj.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://kf.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kn.muxihuayi.cn

Ruby: public / protected / private
来源：http://ly.nicolike.cn

C#:   public / protected / private / internal
来源：http://vh.yuexingan06.cn

[G11] getter / setter
来源：http://cv.nszjky.cn

Py:   @property 与 @x.setter
来源：http://nq.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uk.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://gz.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://qx.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://bx.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ln.nszjky.cn

Ruby: attr_accessor :name
来源：http://ik.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://nr.colortex.cn

[G12] 对象转字符串
来源：http://ff.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://es.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lg.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://qp.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://dx.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://ym.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bv.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://nj.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://er.szxytkj.cn

[G13] 判断对象类型
来源：http://rt.colortex.cn

Py:   isinstance(u, User)
来源：http://rx.wgjwhj.cn

PHP:  $u instanceof User
来源：http://ye.szxytkj.cn

JS:   u instanceof User
来源：http://yl.yuexingan06.cn

TS:   u instanceof User
来源：http://nu.bjjhwx.cn

Java: u instanceof User
来源：http://fz.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bv.szsharing.cn

Ruby: u.is_a?(User)
来源：http://pp.lnxyls.cn

C#:   u is User
来源：http://tu.nszjky.cn

[G14] 数据类 / record
来源：http://lm.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tr.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://ir.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mo.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://so.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://im.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://kz.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iv.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://fh.huixiangedu.cn

[G15] 枚举
来源：http://qu.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://my.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bn.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ge.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://xp.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sx.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://nx.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vb.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://wv.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ny.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://hs.shxzukj.cn

JS:   Object.entries(obj)
来源：http://kw.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://lu.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xc.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iv.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://xq.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://wz.hnjuh.cn

================================================================================
来源：http://gr.shxzukj.cn

H. 异常与错误处理
来源：http://qg.hahajie.cn

================================================================================
来源：http://is.nicolike.cn

[H01] try / catch 基础
来源：http://lj.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rw.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oj.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rz.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xs.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ae.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ha.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xw.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jx.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://rx.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fj.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sq.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gd.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ri.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ub.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jl.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ox.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://li.huanxung.cn

[H03] 主动抛出异常
来源：http://td.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://xx.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gj.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://xq.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://hd.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xi.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ty.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yw.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wv.gzmigu.cn

[H04] 自定义异常类型
来源：http://wd.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://uc.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://at.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://dw.521024.cn

TS:   class MyError extends Error {}
来源：http://zd.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://gm.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ff.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://na.nicolike.cn

C#:   class MyException : Exception {}
来源：http://vf.wgjwhj.cn

[H05] 捕获特定类型
来源：http://xx.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://ah.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hm.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://az.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://vd.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://dq.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wo.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://hz.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vn.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://bn.colortex.cn

Py:   value = d.get("k") or default
来源：http://zf.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ci.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wm.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xa.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://to.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hl.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://ym.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://gf.szsharing.cn

[H07] 断言
来源：http://ym.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://fr.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://bn.nszjky.cn

JS:   console.assert(x > 0);
来源：http://cz.nszjky.cn

TS:   console.assert(x > 0);
来源：http://nm.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://fi.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uh.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vf.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://xc.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://pb.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://lk.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ph.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://zf.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pq.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hm.haigaiapp.cn

Go:   err.Error()
来源：http://if.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://hz.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://bu.newstarts.cn

[H09] 带错误码的异常
来源：http://hd.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://im.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zq.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qi.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mf.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hq.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xd.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qk.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ef.muxihuayi.cn

[H10] 资源自动释放
来源：http://xk.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fc.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://no.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://is.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gv.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dc.szsharing.cn

Go:   defer f.Close()
来源：http://xt.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eu.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://is.yuntaijiaju.cn

================================================================================
来源：http://jk.huixiangedu.cn

I. 正则表达式
来源：http://ry.hahajie.cn

================================================================================
来源：http://wy.panjiajie.cn

[I01] 判断是否匹配
来源：http://hu.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zq.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ca.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://jk.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://ux.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wv.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ej.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://ws.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kd.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://oc.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://ga.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uz.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hq.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://zv.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dp.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://py.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://lg.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bt.nicolike.cn

[I03] 提取捕获分组
来源：http://zy.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vt.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cu.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oe.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nd.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://op.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://er.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tc.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://je.panjiajie.cn

[I04] 正则替换
来源：http://oz.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://at.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nr.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ze.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jm.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vf.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://in.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ij.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xw.jctech888.com.cn

[I05] 按正则拆分
来源：http://ik.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://je.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lu.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://ln.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://eh.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://wi.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xn.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pq.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://za.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ya.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qq.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kc.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sj.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uk.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zj.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vq.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ii.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wu.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://yl.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://am.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://df.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zx.muxihuayi.cn

TS:   /error/gim
来源：http://cr.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hn.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mh.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://hb.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://id.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ih.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pd.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wk.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dh.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ic.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bv.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aw.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://va.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lp.nszjky.cn

================================================================================
来源：http://hx.shxzskj.cn

J. 日期与时间
来源：http://gp.szsharing.cn

================================================================================
来源：http://sr.hahajie.cn

[J01] 获取当前时间
来源：http://zb.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ty.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fg.newstarts.cn

JS:   new Date();  Date.now()
来源：http://vx.colortex.cn

TS:   new Date();  Date.now()
来源：http://lu.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jy.shtwfgs.cn

Go:   time.Now()
来源：http://cl.lnxyls.cn

Ruby: Time.now
来源：http://jk.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mk.huixinmuqiang.cn

[J02] 格式化输出
来源：http://nk.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ya.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dk.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://se.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://lx.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ig.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jm.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yd.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sb.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://pd.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wj.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nb.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://yl.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://su.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pa.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cg.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://ow.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ks.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://pj.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lq.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ki.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rm.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ou.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hw.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lf.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wt.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sw.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://by.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://jy.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bj.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ag.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://db.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://ew.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://us.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://tm.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ht.huanxung.cn

[J06] 计算两时间之差
来源：http://kt.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://lc.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://bf.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ms.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dm.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vw.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://xi.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://gl.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://re.9csxet.cn

[J07] 比较两个日期
来源：http://ep.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://qg.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xh.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rd.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hs.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sf.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fv.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://na.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://qz.shxzukj.cn

[J08] 提取年月日与星期
来源：http://xh.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nq.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nh.jctech888.com.cn


<!-- 参考信息 -->