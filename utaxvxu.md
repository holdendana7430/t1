代发 wailian999

Java: interface Shape { double area(); }
来源：http://ct.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://sl.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oz.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://nq.jctech888.com.cn

[G10] 访问控制
来源：http://aw.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://lo.nszjky.cn

PHP:  public / protected / private
来源：http://ux.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://js.yuexingan06.cn

TS:   public / protected / private
来源：http://ng.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://qn.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hy.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://gy.shxzskj.cn

C#:   public / protected / private / internal
来源：http://nm.haigaiapp.cn

[G11] getter / setter
来源：http://od.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://fn.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pg.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://gy.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://hr.newstarts.cn

Java: public String getName() { return name; }
来源：http://ji.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cx.521024.cn

Ruby: attr_accessor :name
来源：http://co.asd995.cn

C#:   public string Name { get; set; }
来源：http://qs.szxytkj.cn

[G12] 对象转字符串
来源：http://il.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://oa.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ai.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://ch.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://mr.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://yy.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qo.521024.cn

Ruby: def to_s; @name; end
来源：http://bi.521024.cn

C#:   public override string ToString() => Name;
来源：http://wv.521024.cn

[G13] 判断对象类型
来源：http://ua.shxzskj.cn

Py:   isinstance(u, User)
来源：http://tt.szsharing.cn

PHP:  $u instanceof User
来源：http://yj.asd995.cn

JS:   u instanceof User
来源：http://xb.haigaiapp.cn

TS:   u instanceof User
来源：http://zd.gzmigu.cn

Java: u instanceof User
来源：http://ik.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qn.szsharing.cn

Ruby: u.is_a?(User)
来源：http://za.huixiangedu.cn

C#:   u is User
来源：http://ez.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://qu.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ed.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://im.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://td.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://kl.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://xy.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://ed.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gr.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://hu.lnxyls.cn

[G15] 枚举
来源：http://jl.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fk.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kj.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ss.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hd.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://qn.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sz.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://sr.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ha.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://lw.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vx.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://zi.gzmigu.cn

JS:   Object.entries(obj)
来源：http://gx.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://vh.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://us.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dr.newstarts.cn

Ruby: obj.instance_variables
来源：http://pl.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://cv.9csxet.cn

================================================================================
来源：http://cn.colortex.cn

H. 异常与错误处理
来源：http://za.szxytkj.cn

================================================================================
来源：http://ip.lnxyls.cn

[H01] try / catch 基础
来源：http://pf.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ww.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ww.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cg.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gp.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sz.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ur.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jg.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://db.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://if.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cu.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pe.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hn.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yo.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://th.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bi.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ap.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bd.haigaiapp.cn

[H03] 主动抛出异常
来源：http://vs.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://zv.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wb.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://ys.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://lp.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pw.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dr.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://en.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cy.szsharing.cn

[H04] 自定义异常类型
来源：http://zb.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://gb.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kp.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://au.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://yy.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://jr.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sd.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://sv.nicolike.cn

C#:   class MyException : Exception {}
来源：http://md.9csxet.cn

[H05] 捕获特定类型
来源：http://lb.chemitech.net.cn

Py:   except ValueError as e:
来源：http://bw.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dd.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://cs.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://cn.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://tn.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rw.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://in.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dy.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://xc.nszjky.cn

Py:   value = d.get("k") or default
来源：http://ce.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nz.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ij.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://et.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rx.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ei.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://on.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://eu.huixinmuqiang.cn

[H07] 断言
来源：http://fn.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://im.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://fw.nicolike.cn

JS:   console.assert(x > 0);
来源：http://uf.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://wv.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://sc.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bi.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jx.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://wd.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://uv.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://wi.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nl.asd995.cn

JS:   e.message;  e.stack
来源：http://za.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nn.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ri.yuntaijiaju.cn

Go:   err.Error()
来源：http://mj.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://fr.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://ta.nicolike.cn

[H09] 带错误码的异常
来源：http://zu.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zf.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cj.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bt.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yc.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ql.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oi.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ic.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kt.bjjhwx.cn

[H10] 资源自动释放
来源：http://wg.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dd.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://md.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ty.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ua.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dq.asd995.cn

Go:   defer f.Close()
来源：http://vy.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zi.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fm.colortex.cn

================================================================================
来源：http://hb.colortex.cn

I. 正则表达式
来源：http://gd.shxzskj.cn

================================================================================
来源：http://cb.hahajie.cn

[I01] 判断是否匹配
来源：http://el.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ec.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fj.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://ge.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://ht.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gt.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wp.521024.cn

Ruby: s.match?(/\d+/)
来源：http://rn.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qv.nszjky.cn

[I02] 提取所有匹配
来源：http://vt.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://th.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hl.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zb.521024.cn

TS:   s.match(/\d+/g)
来源：http://av.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://va.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fl.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://dz.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jq.lnxyls.cn

[I03] 提取捕获分组
来源：http://st.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lw.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://he.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xl.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ry.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ln.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kk.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://um.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iz.szxytkj.cn

[I04] 正则替换
来源：http://xr.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hf.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://po.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sf.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bv.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bn.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xb.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ac.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gh.szsharing.cn

[I05] 按正则拆分
来源：http://al.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mi.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yj.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://dl.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://ox.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://ob.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cq.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ph.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bs.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sk.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gi.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vs.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qe.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eo.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rm.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ki.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jr.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://te.521024.cn

[I07] 忽略大小写与多行模式
来源：http://tx.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iv.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ks.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ti.521024.cn

TS:   /error/gim
来源：http://yb.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ww.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jm.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://ip.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uv.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://vk.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ji.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://th.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qc.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dg.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fd.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fc.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vn.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uj.shtwfgs.cn

================================================================================
来源：http://zj.muxihuayi.cn

J. 日期与时间
来源：http://wv.521024.cn

================================================================================
来源：http://zu.haigaiapp.cn

[J01] 获取当前时间
来源：http://za.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ro.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uw.521024.cn

JS:   new Date();  Date.now()
来源：http://jr.hahajie.cn

TS:   new Date();  Date.now()
来源：http://an.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dc.asd995.cn

Go:   time.Now()
来源：http://mx.yuexingan06.cn

Ruby: Time.now
来源：http://qz.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ct.colortex.cn

[J02] 格式化输出
来源：http://jo.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tk.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ux.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vp.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://uj.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pl.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nu.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tb.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sd.hahajie.cn

[J03] 字符串解析为日期
来源：http://mi.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://og.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ds.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://zi.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://lc.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yx.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sh.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://we.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ba.newstarts.cn

[J04] 时间戳与日期互转
来源：http://hr.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hp.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yu.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tx.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ko.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ms.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jr.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ee.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://to.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://as.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://av.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nm.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vs.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rh.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://cd.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rf.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://kw.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qo.hnjuh.cn

[J06] 计算两时间之差
来源：http://xb.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://tb.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://sh.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jf.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ul.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ik.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://fg.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://cj.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://uu.shxzukj.cn

[J07] 比较两个日期
来源：http://gh.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://sc.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fk.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ya.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://za.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ta.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bf.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oz.panjiajie.cn


<!-- 参考信息 -->