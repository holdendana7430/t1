代发 wailian999

Java: interface Shape { double area(); }
来源：http://zt.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://ej.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ms.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://ok.huanxung.cn

[G10] 访问控制
来源：http://wh.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://iy.shtwfgs.cn

PHP:  public / protected / private
来源：http://im.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://ci.huanxung.cn

TS:   public / protected / private
来源：http://ho.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://qy.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xu.lnxyls.cn

Ruby: public / protected / private
来源：http://ay.newstarts.cn

C#:   public / protected / private / internal
来源：http://qj.lnxyls.cn

[G11] getter / setter
来源：http://nk.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://qt.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bu.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://kc.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://zs.lnxyls.cn

Java: public String getName() { return name; }
来源：http://mf.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vo.shxzukj.cn

Ruby: attr_accessor :name
来源：http://mz.huanxung.cn

C#:   public string Name { get; set; }
来源：http://mm.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://pc.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://dj.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yp.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://ya.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://fs.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://ms.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nq.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://nn.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://st.jctech888.com.cn

[G13] 判断对象类型
来源：http://hl.nszjky.cn

Py:   isinstance(u, User)
来源：http://sm.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://qz.huanxung.cn

JS:   u instanceof User
来源：http://lq.wgjwhj.cn

TS:   u instanceof User
来源：http://mj.lnxyls.cn

Java: u instanceof User
来源：http://ci.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fe.521024.cn

Ruby: u.is_a?(User)
来源：http://sz.shtwfgs.cn

C#:   u is User
来源：http://lr.chemitech.net.cn

[G14] 数据类 / record
来源：http://yz.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mi.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://mz.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eb.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://jx.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://ya.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://ci.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rp.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://ux.hnjuh.cn

[G15] 枚举
来源：http://bj.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hj.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jt.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sc.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hi.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://wl.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gq.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://pt.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://de.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://pn.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eu.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://ea.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://jg.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://nc.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jk.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vm.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://ea.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://dh.newstarts.cn

================================================================================
来源：http://st.bookmarksfly.cn

H. 异常与错误处理
来源：http://ue.bookmarksfly.cn

================================================================================
来源：http://nw.huixiangedu.cn

[H01] try / catch 基础
来源：http://fa.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oy.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qk.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rc.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fy.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://az.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aj.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ml.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wb.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://xi.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ps.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ur.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bd.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bi.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://js.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sc.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oi.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qf.yuexingan06.cn

[H03] 主动抛出异常
来源：http://ov.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://zw.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lj.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://ct.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://qf.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rd.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kq.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zj.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fg.hahajie.cn

[H04] 自定义异常类型
来源：http://ye.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://xv.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jt.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://tr.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://id.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://ql.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zn.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://pe.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://wv.9csxet.cn

[H05] 捕获特定类型
来源：http://lk.shxzskj.cn

Py:   except ValueError as e:
来源：http://je.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vs.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://hw.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://qi.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://un.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fl.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://gn.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ad.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://qc.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://xb.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ng.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://us.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jz.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://if.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wa.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://rs.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://hk.gzmigu.cn

[H07] 断言
来源：http://wp.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://sj.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://ia.hahajie.cn

JS:   console.assert(x > 0);
来源：http://zr.asd995.cn

TS:   console.assert(x > 0);
来源：http://zu.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://ha.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zf.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zo.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://ox.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://zg.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://ki.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://im.521024.cn

JS:   e.message;  e.stack
来源：http://jb.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zw.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mr.lnxyls.cn

Go:   err.Error()
来源：http://yb.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://fh.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://js.panjiajie.cn

[H09] 带错误码的异常
来源：http://ej.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rd.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://od.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sb.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xw.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wp.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://be.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bq.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xi.9csxet.cn

[H10] 资源自动释放
来源：http://rf.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zj.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rt.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nf.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fr.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://az.shxzskj.cn

Go:   defer f.Close()
来源：http://gr.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hg.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wo.hnjuh.cn

================================================================================
来源：http://xk.szsharing.cn

I. 正则表达式
来源：http://uk.gzmigu.cn

================================================================================
来源：http://jm.szsharing.cn

[I01] 判断是否匹配
来源：http://ji.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vr.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vg.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://qs.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://vv.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ct.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://he.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://ws.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gv.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://gi.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://fx.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gv.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kj.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://ob.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rn.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rx.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://bi.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ri.hnjuh.cn

[I03] 提取捕获分组
来源：http://ju.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ob.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ek.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cz.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kf.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zg.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://il.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pf.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kr.haigaiapp.cn

[I04] 正则替换
来源：http://xl.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wm.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jv.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ja.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vm.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mk.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sw.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lu.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://si.nicolike.cn

[I05] 按正则拆分
来源：http://oj.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vi.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://of.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://it.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://eh.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://px.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ch.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cb.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fj.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rv.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kz.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wu.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yx.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kv.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ze.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dh.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kf.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pj.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://hu.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jf.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qj.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wl.muxihuayi.cn

TS:   /error/gim
来源：http://jy.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rc.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bw.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://zb.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dc.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://kf.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lx.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jc.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vf.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ls.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lc.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wi.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cu.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cu.shxzskj.cn

================================================================================
来源：http://gr.521024.cn

J. 日期与时间
来源：http://yp.chemitech.net.cn

================================================================================
来源：http://fn.asd995.cn

[J01] 获取当前时间
来源：http://yq.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xo.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tw.9csxet.cn

JS:   new Date();  Date.now()
来源：http://rl.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://kp.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oa.szsharing.cn

Go:   time.Now()
来源：http://yj.szxytkj.cn

Ruby: Time.now
来源：http://yt.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ua.nicolike.cn

[J02] 格式化输出
来源：http://kr.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cw.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vf.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hw.huixiangedu.cn

TS:   d.toISOString()
来源：http://mf.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jg.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sk.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://io.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cu.panjiajie.cn

[J03] 字符串解析为日期
来源：http://me.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tw.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wr.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://wp.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://kq.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lv.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tg.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ce.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uf.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://qt.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oh.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://av.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pn.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yc.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vn.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ys.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ww.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fh.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://nd.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://hv.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ga.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nt.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sw.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://wi.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qc.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ml.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zc.521024.cn

[J06] 计算两时间之差
来源：http://ab.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://rt.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://wn.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uu.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gk.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fs.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://lg.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://vh.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://sn.shxzukj.cn

[J07] 比较两个日期
来源：http://rw.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ax.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qc.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mm.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xn.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kv.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cu.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ov.newstarts.cn


<!-- 参考信息 -->