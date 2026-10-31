代发 wailian999

Java: interface Shape { double area(); }
来源：http://kf.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ym.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fv.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://hl.huanxung.cn

[G10] 访问控制
来源：http://oz.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://es.gzmigu.cn

PHP:  public / protected / private
来源：http://tv.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://st.panjiajie.cn

TS:   public / protected / private
来源：http://qx.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://pp.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mi.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://aa.shxzukj.cn

C#:   public / protected / private / internal
来源：http://pa.huixiangedu.cn

[G11] getter / setter
来源：http://ew.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://ha.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://re.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://yq.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://zk.hnjuh.cn

Java: public String getName() { return name; }
来源：http://iq.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sl.hnjuh.cn

Ruby: attr_accessor :name
来源：http://pn.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://ow.9csxet.cn

[G12] 对象转字符串
来源：http://fh.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://uy.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mw.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://ti.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://fp.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://ut.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ym.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://jk.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://fw.muxihuayi.cn

[G13] 判断对象类型
来源：http://if.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://pb.szxytkj.cn

PHP:  $u instanceof User
来源：http://jc.yuntaijiaju.cn

JS:   u instanceof User
来源：http://py.shxzskj.cn

TS:   u instanceof User
来源：http://rl.asd995.cn

Java: u instanceof User
来源：http://io.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rn.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://wc.newstarts.cn

C#:   u is User
来源：http://va.haigaiapp.cn

[G14] 数据类 / record
来源：http://lr.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ss.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://ie.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dx.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://rw.9csxet.cn

Java: record User(String name, int age) {}
来源：http://ze.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://if.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oh.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://aq.521024.cn

[G15] 枚举
来源：http://lm.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vy.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qi.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qi.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ci.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://fh.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ux.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://bv.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fp.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://fx.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sw.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://ek.hnjuh.cn

JS:   Object.entries(obj)
来源：http://nf.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://tq.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yv.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://co.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://qn.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://rl.gzmigu.cn

================================================================================
来源：http://bw.muxihuayi.cn

H. 异常与错误处理
来源：http://wg.chemitech.net.cn

================================================================================
来源：http://nt.shxzukj.cn

[H01] try / catch 基础
来源：http://gd.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ko.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://po.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://km.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yk.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://by.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mb.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://je.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vj.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://fq.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jp.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dz.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xx.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zu.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lq.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pl.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ux.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zx.yuexingan06.cn

[H03] 主动抛出异常
来源：http://qt.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://sv.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jh.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://sd.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://cv.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lv.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://do.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://re.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://js.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://sr.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://qh.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dy.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://mn.nszjky.cn

TS:   class MyError extends Error {}
来源：http://sx.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://ws.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kt.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://pl.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://nb.shxzskj.cn

[H05] 捕获特定类型
来源：http://mq.asd995.cn

Py:   except ValueError as e:
来源：http://bs.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yk.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://dj.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://sy.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://pf.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ww.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://tf.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://re.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://pu.9csxet.cn

Py:   value = d.get("k") or default
来源：http://bk.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kf.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xu.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fe.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://on.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://za.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://cf.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://kr.shxzskj.cn

[H07] 断言
来源：http://yp.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://zg.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://xd.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://zj.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://rl.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://dm.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://du.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lh.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://po.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://fk.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ck.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ao.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://lf.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ml.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yz.szsharing.cn

Go:   err.Error()
来源：http://or.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://wa.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://wg.szxytkj.cn

[H09] 带错误码的异常
来源：http://zu.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kc.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cv.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wc.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jm.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hv.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wa.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gp.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ro.lnxyls.cn

[H10] 资源自动释放
来源：http://yn.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mu.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://br.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gd.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rp.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ge.9csxet.cn

Go:   defer f.Close()
来源：http://wj.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ou.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yf.huixinmuqiang.cn

================================================================================
来源：http://yy.huanxung.cn

I. 正则表达式
来源：http://qs.colortex.cn

================================================================================
来源：http://yv.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://qm.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vv.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pd.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://zj.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://ps.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://as.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xt.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://oh.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zl.szxytkj.cn

[I02] 提取所有匹配
来源：http://mf.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://cf.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://av.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://at.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://nw.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vr.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ex.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://ah.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pv.wgjwhj.cn

[I03] 提取捕获分组
来源：http://aw.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sx.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ey.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fp.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ze.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tj.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mt.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dd.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vu.chemitech.net.cn

[I04] 正则替换
来源：http://ve.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oo.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://du.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bi.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ly.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kb.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://od.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rd.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://er.shxzskj.cn

[I05] 按正则拆分
来源：http://mb.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wc.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://au.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://wp.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://sa.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://cg.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://st.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zb.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pf.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wf.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ol.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bi.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zj.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gx.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wk.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tr.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gf.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zk.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://xu.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hg.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://en.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mc.huanxung.cn

TS:   /error/gim
来源：http://mu.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rt.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zx.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://ny.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tg.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://xk.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fz.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zu.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gk.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pf.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sv.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iq.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aw.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qs.gzmigu.cn

================================================================================
来源：http://qx.gzmigu.cn

J. 日期与时间
来源：http://rm.nszjky.cn

================================================================================
来源：http://ju.lnxyls.cn

[J01] 获取当前时间
来源：http://fi.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ae.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kk.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://ks.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://bb.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fl.hahajie.cn

Go:   time.Now()
来源：http://xf.wgjwhj.cn

Ruby: Time.now
来源：http://el.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qm.bjjhwx.cn

[J02] 格式化输出
来源：http://gz.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hl.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uo.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xc.chemitech.net.cn

TS:   d.toISOString()
来源：http://bq.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://le.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hw.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vr.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qe.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://jp.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jp.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tv.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://np.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://lq.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://at.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fo.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://uf.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gc.newstarts.cn

[J04] 时间戳与日期互转
来源：http://ju.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zy.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ip.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sb.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cl.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ov.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ka.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://js.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nn.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://du.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://jr.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hq.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tx.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nd.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://pc.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uo.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://lc.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iw.newstarts.cn

[J06] 计算两时间之差
来源：http://bq.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://gq.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://sv.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mb.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://up.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zs.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://ev.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://fc.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://ur.huanxung.cn

[J07] 比较两个日期
来源：http://na.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://pu.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ld.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ns.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bq.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oo.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://de.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mv.newstarts.cn


<!-- 参考信息 -->