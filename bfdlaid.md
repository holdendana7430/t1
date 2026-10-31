代发 wailian999

Java: interface Shape { double area(); }
来源：http://wb.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://lu.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wm.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://lx.yuexingan06.cn

[G10] 访问控制
来源：http://on.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://es.lnxyls.cn

PHP:  public / protected / private
来源：http://uu.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://fm.huixinmuqiang.cn

TS:   public / protected / private
来源：http://xm.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://ry.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nt.gzmigu.cn

Ruby: public / protected / private
来源：http://pw.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://ji.yuexingan06.cn

[G11] getter / setter
来源：http://gb.hahajie.cn

Py:   @property 与 @x.setter
来源：http://ku.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tk.hahajie.cn

JS:   get name() { return this._name; }
来源：http://hx.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://fy.nicolike.cn

Java: public String getName() { return name; }
来源：http://jm.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uh.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://ti.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://wm.newstarts.cn

[G12] 对象转字符串
来源：http://zo.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://df.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mw.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://wj.521024.cn

TS:   toString(): string { return this.name; }
来源：http://mj.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://bd.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ew.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ly.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://ri.szxytkj.cn

[G13] 判断对象类型
来源：http://qs.9csxet.cn

Py:   isinstance(u, User)
来源：http://ah.shtwfgs.cn

PHP:  $u instanceof User
来源：http://hs.nicolike.cn

JS:   u instanceof User
来源：http://kn.bookmarksfly.cn

TS:   u instanceof User
来源：http://pm.panjiajie.cn

Java: u instanceof User
来源：http://nu.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ui.szsharing.cn

Ruby: u.is_a?(User)
来源：http://pz.muxihuayi.cn

C#:   u is User
来源：http://cy.chemitech.net.cn

[G14] 数据类 / record
来源：http://ww.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kr.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ui.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vk.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://xv.szsharing.cn

Java: record User(String name, int age) {}
来源：http://zw.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://wj.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ux.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://ow.huixiangedu.cn

[G15] 枚举
来源：http://kn.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sg.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ni.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kj.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://am.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://sq.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fv.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://yw.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ok.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://zm.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qs.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://cv.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://ti.gzmigu.cn

TS:   Object.entries(obj)
来源：http://un.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fh.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://we.huanxung.cn

Ruby: obj.instance_variables
来源：http://bm.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://fr.bjjhwx.cn

================================================================================
来源：http://ul.jctech888.com.cn

H. 异常与错误处理
来源：http://py.jctech888.com.cn

================================================================================
来源：http://fb.chemitech.net.cn

[H01] try / catch 基础
来源：http://yz.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nd.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hp.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://at.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://my.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wk.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ih.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pr.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yb.hahajie.cn

[H02] finally / ensure 收尾
来源：http://fe.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pq.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pp.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bh.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hn.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://df.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zd.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rg.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rc.colortex.cn

[H03] 主动抛出异常
来源：http://ki.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://zf.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rc.colortex.cn

JS:   throw new Error("错误信息");
来源：http://zf.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://fn.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xh.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ka.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hp.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vk.wgjwhj.cn

[H04] 自定义异常类型
来源：http://ox.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://en.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vp.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://lt.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://ov.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://oo.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dv.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://bw.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://dp.jctech888.com.cn

[H05] 捕获特定类型
来源：http://dq.hahajie.cn

Py:   except ValueError as e:
来源：http://qv.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://by.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://oc.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://pf.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://hp.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uq.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://xi.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qj.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://xv.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://mt.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ev.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xs.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cw.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zb.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gf.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://tf.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://yg.jianghongdianzi.cn

[H07] 断言
来源：http://ec.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://aq.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://oa.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://tw.huanxung.cn

TS:   console.assert(x > 0);
来源：http://gi.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://ny.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vg.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cz.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://kx.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://ed.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ky.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yz.shxzskj.cn

JS:   e.message;  e.stack
来源：http://ov.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://or.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pv.9csxet.cn

Go:   err.Error()
来源：http://rg.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://uo.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://wz.chemitech.net.cn

[H09] 带错误码的异常
来源：http://oo.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zx.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dz.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yl.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qb.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yr.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wy.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wh.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gw.huanxung.cn

[H10] 资源自动释放
来源：http://bm.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://au.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iz.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qq.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tb.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ye.bookmarksfly.cn

Go:   defer f.Close()
来源：http://li.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pr.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cl.wgjwhj.cn

================================================================================
来源：http://kq.hnjuh.cn

I. 正则表达式
来源：http://ft.szxytkj.cn

================================================================================
来源：http://nv.szsharing.cn

[I01] 判断是否匹配
来源：http://aw.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pf.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fx.nicolike.cn

JS:   /\d+/.test(s)
来源：http://ni.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://lj.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ml.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pn.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://bh.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jb.yuexingan06.cn

[I02] 提取所有匹配
来源：http://as.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://xq.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iw.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yr.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://ro.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ne.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qc.521024.cn

Ruby: s.scan(/\d+/)
来源：http://yk.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ss.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://hw.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qh.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zx.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oa.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zh.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vj.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mj.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zh.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://si.colortex.cn

[I04] 正则替换
来源：http://xd.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wi.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pq.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ty.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rf.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wf.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xf.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vl.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mt.521024.cn

[I05] 按正则拆分
来源：http://oh.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bc.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rc.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://di.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://dl.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ew.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yk.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kq.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lr.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fn.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://js.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vm.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fi.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ve.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dl.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xp.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fu.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hm.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://ft.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ls.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qi.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xv.chemitech.net.cn

TS:   /error/gim
来源：http://ac.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xe.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wm.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://eb.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sv.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://xn.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mz.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ry.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ko.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vi.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bo.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ho.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vy.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pe.nszjky.cn

================================================================================
来源：http://wa.jianghongdianzi.cn

J. 日期与时间
来源：http://sz.jctech888.com.cn

================================================================================
来源：http://il.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://it.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yp.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sw.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://gz.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://jy.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://we.bookmarksfly.cn

Go:   time.Now()
来源：http://gu.521024.cn

Ruby: Time.now
来源：http://sj.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dz.nicolike.cn

[J02] 格式化输出
来源：http://rk.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jh.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dv.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jo.jctech888.com.cn

TS:   d.toISOString()
来源：http://bh.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qm.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zz.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://za.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qv.szsharing.cn

[J03] 字符串解析为日期
来源：http://js.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ku.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xu.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://vw.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://xt.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qq.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sa.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://mf.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yi.nszjky.cn

[J04] 时间戳与日期互转
来源：http://ri.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nz.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://us.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ux.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ay.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ls.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://af.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://td.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zj.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://ua.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://ze.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ur.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tw.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ul.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://la.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pl.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://ip.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hi.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://hg.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://nx.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://pj.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ct.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zf.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aq.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://qv.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://zy.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://ji.colortex.cn

[J07] 比较两个日期
来源：http://eh.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://ci.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gq.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://br.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vz.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zn.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eu.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ev.muxihuayi.cn


<!-- 参考信息 -->