代发 wailian999

Java: interface Shape { double area(); }
来源：http://sl.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://nk.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ah.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://nd.hnjuh.cn

[G10] 访问控制
来源：http://co.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://li.bookmarksfly.cn

PHP:  public / protected / private
来源：http://bt.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://tk.shtwfgs.cn

TS:   public / protected / private
来源：http://zt.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://ua.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tj.lnxyls.cn

Ruby: public / protected / private
来源：http://kg.gzmigu.cn

C#:   public / protected / private / internal
来源：http://bo.panjiajie.cn

[G11] getter / setter
来源：http://yk.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://kn.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iy.521024.cn

JS:   get name() { return this._name; }
来源：http://mu.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://kl.hahajie.cn

Java: public String getName() { return name; }
来源：http://qt.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tl.panjiajie.cn

Ruby: attr_accessor :name
来源：http://yn.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://xg.nszjky.cn

[G12] 对象转字符串
来源：http://bo.asd995.cn

Py:   def __str__(self): return self.name
来源：http://vp.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cn.nicolike.cn

JS:   toString() { return this.name; }
来源：http://gs.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://wu.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://ge.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://de.nszjky.cn

Ruby: def to_s; @name; end
来源：http://ru.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://po.yuexingan06.cn

[G13] 判断对象类型
来源：http://jy.szxytkj.cn

Py:   isinstance(u, User)
来源：http://zv.panjiajie.cn

PHP:  $u instanceof User
来源：http://ug.lnxyls.cn

JS:   u instanceof User
来源：http://if.shtwfgs.cn

TS:   u instanceof User
来源：http://pk.9csxet.cn

Java: u instanceof User
来源：http://ze.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yg.9csxet.cn

Ruby: u.is_a?(User)
来源：http://ve.shxzskj.cn

C#:   u is User
来源：http://qw.jctech888.com.cn

[G14] 数据类 / record
来源：http://uu.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pe.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://ut.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ho.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://ou.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://ml.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://jy.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jr.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://ub.hahajie.cn

[G15] 枚举
来源：http://fl.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lv.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bo.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hb.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sb.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://vt.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gz.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://yc.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ob.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://ss.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://al.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://ki.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://db.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://rc.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yd.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://up.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://un.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://li.bjjhwx.cn

================================================================================
来源：http://fc.chemitech.net.cn

H. 异常与错误处理
来源：http://fh.shtwfgs.cn

================================================================================
来源：http://sl.szxytkj.cn

[H01] try / catch 基础
来源：http://tf.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nf.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ga.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ia.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wz.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hr.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ap.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hv.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qa.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://cn.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tp.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mm.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qw.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ma.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pt.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qz.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qv.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pe.huixiangedu.cn

[H03] 主动抛出异常
来源：http://ah.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://ax.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dg.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://pw.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://ri.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gi.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xy.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zp.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://so.muxihuayi.cn

[H04] 自定义异常类型
来源：http://ri.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://pr.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cx.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://fw.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://sv.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://fi.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fd.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://ft.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://wx.newstarts.cn

[H05] 捕获特定类型
来源：http://kl.newstarts.cn

Py:   except ValueError as e:
来源：http://ub.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bp.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://ka.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://pe.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://ce.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://du.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://xr.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xn.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://dr.colortex.cn

Py:   value = d.get("k") or default
来源：http://ig.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ao.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kk.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rl.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mn.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bp.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://dl.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://li.chemitech.net.cn

[H07] 断言
来源：http://wz.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://ix.szxytkj.cn

PHP:  assert($x > 0);
来源：http://wv.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://lo.hahajie.cn

TS:   console.assert(x > 0);
来源：http://hy.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://ke.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sf.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wc.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://rj.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://dq.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://zr.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://je.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://sj.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pn.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://np.huixiangedu.cn

Go:   err.Error()
来源：http://zn.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://ya.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://sq.shtwfgs.cn

[H09] 带错误码的异常
来源：http://qq.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ks.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yh.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bt.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hh.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xk.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uz.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vi.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ri.szxytkj.cn

[H10] 资源自动释放
来源：http://we.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hp.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ei.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tn.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sx.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fw.521024.cn

Go:   defer f.Close()
来源：http://ze.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ex.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ip.jianghongdianzi.cn

================================================================================
来源：http://dt.nicolike.cn

I. 正则表达式
来源：http://pa.9csxet.cn

================================================================================
来源：http://tj.haigaiapp.cn

[I01] 判断是否匹配
来源：http://cb.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vr.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xp.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://tc.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://ya.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qf.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bh.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://li.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://il.lnxyls.cn

[I02] 提取所有匹配
来源：http://wo.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://vk.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://or.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qa.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://wv.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zl.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kp.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://yz.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://es.newstarts.cn

[I03] 提取捕获分组
来源：http://du.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://af.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uu.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ux.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gx.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zt.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bu.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iq.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://os.hahajie.cn

[I04] 正则替换
来源：http://qa.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ik.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pf.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xu.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tl.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bw.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cg.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jn.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bd.colortex.cn

[I05] 按正则拆分
来源：http://ns.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pm.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dx.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ev.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://cc.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://bl.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ts.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uy.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xm.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wd.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tt.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wb.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xe.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ch.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mn.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bd.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ad.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cn.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://xf.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bf.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ue.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fh.lnxyls.cn

TS:   /error/gim
来源：http://cu.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pa.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xz.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://dr.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nm.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://ar.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://py.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ex.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sn.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mn.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fl.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vk.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uo.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://to.huixinmuqiang.cn

================================================================================
来源：http://kz.jianghongdianzi.cn

J. 日期与时间
来源：http://kq.muxihuayi.cn

================================================================================
来源：http://pw.szxytkj.cn

[J01] 获取当前时间
来源：http://sj.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lk.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ly.hahajie.cn

JS:   new Date();  Date.now()
来源：http://fy.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://lb.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oc.wgjwhj.cn

Go:   time.Now()
来源：http://ua.jctech888.com.cn

Ruby: Time.now
来源：http://do.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bu.chemitech.net.cn

[J02] 格式化输出
来源：http://xk.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://li.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yo.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://no.9csxet.cn

TS:   d.toISOString()
来源：http://us.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ti.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ez.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://us.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gr.huanxung.cn

[J03] 字符串解析为日期
来源：http://xn.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mh.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pf.521024.cn

JS:   new Date("2024-01-02")
来源：http://qb.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://sj.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uo.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oy.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://fy.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ip.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://cd.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gs.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://up.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jc.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tz.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rr.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://di.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rv.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pr.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://od.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://nt.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mc.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cs.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bj.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://xv.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ys.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://eh.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yt.yuexingan06.cn

[J06] 计算两时间之差
来源：http://ov.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://sc.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://cu.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xs.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rv.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ea.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://eg.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://tu.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://az.9csxet.cn

[J07] 比较两个日期
来源：http://di.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://fc.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mx.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zz.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rn.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yw.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hi.huixiangedu.cn


<!-- 参考信息 -->