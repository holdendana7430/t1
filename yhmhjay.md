代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://tr.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rh.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vp.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://st.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://sh.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://gc.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zm.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://rm.shxzukj.cn

[G10] 访问控制
来源：http://nz.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://le.nicolike.cn

PHP:  public / protected / private
来源：http://we.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://zl.chemitech.net.cn

TS:   public / protected / private
来源：http://se.521024.cn

Java: public / protected / private / 默认包级
来源：http://iw.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vf.newstarts.cn

Ruby: public / protected / private
来源：http://wq.shxzskj.cn

C#:   public / protected / private / internal
来源：http://mz.huixiangedu.cn

[G11] getter / setter
来源：http://yq.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://kk.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jq.521024.cn

JS:   get name() { return this._name; }
来源：http://ci.521024.cn

TS:   get name(): string { return this._name; }
来源：http://rm.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://pv.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ox.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://gs.huanxung.cn

C#:   public string Name { get; set; }
来源：http://cp.shxzukj.cn

[G12] 对象转字符串
来源：http://jf.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://sg.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ls.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://ee.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://la.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://dm.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jn.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://ko.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://or.colortex.cn

[G13] 判断对象类型
来源：http://fa.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://no.521024.cn

PHP:  $u instanceof User
来源：http://cy.bookmarksfly.cn

JS:   u instanceof User
来源：http://cn.nszjky.cn

TS:   u instanceof User
来源：http://xl.lnxyls.cn

Java: u instanceof User
来源：http://ap.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mn.huanxung.cn

Ruby: u.is_a?(User)
来源：http://mc.521024.cn

C#:   u is User
来源：http://as.wgjwhj.cn

[G14] 数据类 / record
来源：http://vz.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wj.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://dg.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://za.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://jx.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://hb.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://aq.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rc.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://aq.bookmarksfly.cn

[G15] 枚举
来源：http://ty.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cp.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://up.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qe.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dl.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://af.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bt.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://fq.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eb.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://on.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://if.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://jf.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://ik.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://zl.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rg.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xp.9csxet.cn

Ruby: obj.instance_variables
来源：http://qd.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://xd.yuexingan06.cn

================================================================================
来源：http://vy.521024.cn

H. 异常与错误处理
来源：http://qn.nszjky.cn

================================================================================
来源：http://jf.bookmarksfly.cn

[H01] try / catch 基础
来源：http://xd.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ef.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yu.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://me.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zf.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://df.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hs.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qd.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wn.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://mj.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cm.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ox.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qh.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gl.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://es.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ca.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ep.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xo.szsharing.cn

[H03] 主动抛出异常
来源：http://jz.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://wx.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gc.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://el.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://bb.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ia.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ld.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ig.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jh.asd995.cn

[H04] 自定义异常类型
来源：http://zv.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://sg.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://st.nicolike.cn

JS:   class MyError extends Error {}
来源：http://kr.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://pb.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://mm.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sl.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://vk.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://gw.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://rr.hahajie.cn

Py:   except ValueError as e:
来源：http://pw.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oo.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://wr.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://rd.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://ne.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://im.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://ui.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cw.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://mp.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://ha.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yx.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yp.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vo.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://na.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ic.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://vq.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://du.huixiangedu.cn

[H07] 断言
来源：http://sm.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://os.newstarts.cn

PHP:  assert($x > 0);
来源：http://ra.huanxung.cn

JS:   console.assert(x > 0);
来源：http://ic.hahajie.cn

TS:   console.assert(x > 0);
来源：http://sw.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://vb.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eo.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://we.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ln.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://nl.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://vq.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ue.szsharing.cn

JS:   e.message;  e.stack
来源：http://nw.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://du.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aa.panjiajie.cn

Go:   err.Error()
来源：http://rc.521024.cn

Ruby: e.message;  e.backtrace
来源：http://dy.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://mw.huixiangedu.cn

[H09] 带错误码的异常
来源：http://zw.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gx.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ox.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ei.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zs.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nm.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wk.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bs.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://es.9csxet.cn

[H10] 资源自动释放
来源：http://ac.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://an.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rt.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gk.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mc.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nu.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://hn.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kl.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://op.nicolike.cn

================================================================================
来源：http://rf.521024.cn

I. 正则表达式
来源：http://lb.colortex.cn

================================================================================
来源：http://ga.panjiajie.cn

[I01] 判断是否匹配
来源：http://mi.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uo.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nk.szsharing.cn

JS:   /\d+/.test(s)
来源：http://zq.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://mk.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dg.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mc.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://uw.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ho.hahajie.cn

[I02] 提取所有匹配
来源：http://xo.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://ao.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sx.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nr.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://qz.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qp.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bl.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://tb.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mo.9csxet.cn

[I03] 提取捕获分组
来源：http://kd.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pv.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xk.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cy.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vg.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://if.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yg.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iq.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://li.wgjwhj.cn

[I04] 正则替换
来源：http://ha.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ft.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qt.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dr.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rh.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ve.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zq.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eo.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aa.shtwfgs.cn

[I05] 按正则拆分
来源：http://yv.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qj.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://do.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://dm.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://np.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://xf.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ym.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sc.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qh.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://de.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tn.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://us.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yw.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uw.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mc.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xm.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xy.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://my.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://fl.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cg.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jf.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rs.huixinmuqiang.cn

TS:   /error/gim
来源：http://wx.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ph.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ta.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://ag.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qd.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://bz.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wm.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://us.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nl.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nv.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tt.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ql.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mj.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nt.nicolike.cn

================================================================================
来源：http://lr.panjiajie.cn

J. 日期与时间
来源：http://ip.chemitech.net.cn

================================================================================
来源：http://be.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://hz.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dh.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://js.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://mv.521024.cn

TS:   new Date();  Date.now()
来源：http://oi.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fo.bjjhwx.cn

Go:   time.Now()
来源：http://zi.wgjwhj.cn

Ruby: Time.now
来源：http://pj.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kb.wgjwhj.cn

[J02] 格式化输出
来源：http://ve.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ow.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ny.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dq.panjiajie.cn

TS:   d.toISOString()
来源：http://xn.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://li.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bs.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bh.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gs.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://mk.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tf.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tq.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://dh.colortex.cn

TS:   new Date("2024-01-02")
来源：http://ha.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ce.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://za.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://nw.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://os.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://wa.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ge.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mf.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ko.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hc.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yn.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kq.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lr.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sr.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://kz.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://tf.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://za.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cy.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://by.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://wa.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://um.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://dz.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nu.lnxyls.cn

[J06] 计算两时间之差
来源：http://sg.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://wq.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://md.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://az.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eg.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bt.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://pi.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://hs.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://dg.colortex.cn

[J07] 比较两个日期
来源：http://ru.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://fg.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jl.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ze.wgjwhj.cn


<!-- 参考信息 -->