代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://kx.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mp.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oq.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://xl.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://xa.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://df.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yo.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://et.jianghongdianzi.cn

[G10] 访问控制
来源：http://ua.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://oz.nicolike.cn

PHP:  public / protected / private
来源：http://zh.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://dn.szsharing.cn

TS:   public / protected / private
来源：http://nt.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://ws.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jt.colortex.cn

Ruby: public / protected / private
来源：http://kr.newstarts.cn

C#:   public / protected / private / internal
来源：http://eh.9csxet.cn

[G11] getter / setter
来源：http://vp.nszjky.cn

Py:   @property 与 @x.setter
来源：http://eu.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ah.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://zu.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://yf.newstarts.cn

Java: public String getName() { return name; }
来源：http://ot.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ra.nicolike.cn

Ruby: attr_accessor :name
来源：http://rh.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://nm.jctech888.com.cn

[G12] 对象转字符串
来源：http://zy.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://jj.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pf.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://cw.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://hf.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://ua.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kw.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://bo.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://oz.haigaiapp.cn

[G13] 判断对象类型
来源：http://nk.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://xw.nicolike.cn

PHP:  $u instanceof User
来源：http://ku.shxzukj.cn

JS:   u instanceof User
来源：http://rv.lnxyls.cn

TS:   u instanceof User
来源：http://qf.huixinmuqiang.cn

Java: u instanceof User
来源：http://jz.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qm.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://du.asd995.cn

C#:   u is User
来源：http://lk.muxihuayi.cn

[G14] 数据类 / record
来源：http://hc.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tj.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://gp.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iq.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://cm.colortex.cn

Java: record User(String name, int age) {}
来源：http://pc.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://cc.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://su.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://ln.bookmarksfly.cn

[G15] 枚举
来源：http://ac.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lc.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ig.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bi.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ki.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://st.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oq.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://wa.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sx.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://fc.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://of.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://ml.shxzskj.cn

JS:   Object.entries(obj)
来源：http://ru.shxzukj.cn

TS:   Object.entries(obj)
来源：http://bd.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fo.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sk.shxzskj.cn

Ruby: obj.instance_variables
来源：http://ft.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://sw.shxzskj.cn

================================================================================
来源：http://fp.asd995.cn

H. 异常与错误处理
来源：http://ks.lnxyls.cn

================================================================================
来源：http://jb.yuexingan06.cn

[H01] try / catch 基础
来源：http://kv.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yo.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pw.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ah.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aj.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ft.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gi.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uk.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nu.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://vf.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qf.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://er.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://it.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zu.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bf.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ig.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wb.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jy.shtwfgs.cn

[H03] 主动抛出异常
来源：http://ik.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://st.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bb.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://lw.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://wv.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ve.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hx.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jb.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ud.shxzukj.cn

[H04] 自定义异常类型
来源：http://iu.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://hk.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nk.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://px.asd995.cn

TS:   class MyError extends Error {}
来源：http://mg.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://pr.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uy.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://bl.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://fk.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://pp.szxytkj.cn

Py:   except ValueError as e:
来源：http://ro.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bh.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://am.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://nt.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://ev.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zz.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://df.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vm.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://ex.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://ax.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qd.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nj.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gx.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xm.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ds.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://gv.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://dh.yuexingan06.cn

[H07] 断言
来源：http://dg.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://ax.hahajie.cn

PHP:  assert($x > 0);
来源：http://wy.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://xk.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://ky.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://lp.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dm.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fz.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://dc.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://qt.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://yb.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ii.szsharing.cn

JS:   e.message;  e.stack
来源：http://iq.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ff.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://la.szxytkj.cn

Go:   err.Error()
来源：http://lo.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://dc.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://wa.haigaiapp.cn

[H09] 带错误码的异常
来源：http://dl.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tv.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ay.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ec.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nh.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jo.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ww.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zv.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zo.nszjky.cn

[H10] 资源自动释放
来源：http://me.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ah.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gf.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xg.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yj.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ea.panjiajie.cn

Go:   defer f.Close()
来源：http://rl.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cg.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ug.shxzukj.cn

================================================================================
来源：http://gx.huanxung.cn

I. 正则表达式
来源：http://ek.nicolike.cn

================================================================================
来源：http://xg.hahajie.cn

[I01] 判断是否匹配
来源：http://af.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kp.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vh.colortex.cn

JS:   /\d+/.test(s)
来源：http://hj.nicolike.cn

TS:   /\d+/.test(s)
来源：http://rg.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fn.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ud.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://in.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://he.shtwfgs.cn

[I02] 提取所有匹配
来源：http://ij.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://vv.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://in.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ab.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://ez.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cj.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rn.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://gk.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ji.shxzskj.cn

[I03] 提取捕获分组
来源：http://in.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ef.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mc.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ax.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tv.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kg.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jf.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wz.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://px.bookmarksfly.cn

[I04] 正则替换
来源：http://ng.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eg.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pl.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://di.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gp.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ni.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gl.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rn.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vo.szsharing.cn

[I05] 按正则拆分
来源：http://lr.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ya.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wb.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://zs.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://jr.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://vq.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yk.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tv.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fz.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rj.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qg.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vb.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aq.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vj.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wu.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kk.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cw.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ku.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://el.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qj.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mn.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eo.jianghongdianzi.cn

TS:   /error/gim
来源：http://ey.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dr.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ic.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://gh.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kx.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://bf.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yw.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dd.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ji.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://km.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xu.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tr.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fv.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jw.szsharing.cn

================================================================================
来源：http://em.yuexingan06.cn

J. 日期与时间
来源：http://er.shxzukj.cn

================================================================================
来源：http://zo.lnxyls.cn

[J01] 获取当前时间
来源：http://zi.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zs.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ir.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://ah.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://kj.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rb.chemitech.net.cn

Go:   time.Now()
来源：http://tr.haigaiapp.cn

Ruby: Time.now
来源：http://jf.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xl.gzmigu.cn

[J02] 格式化输出
来源：http://lo.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bg.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ut.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bv.newstarts.cn

TS:   d.toISOString()
来源：http://pm.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://en.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vc.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bw.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jz.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://lo.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gs.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gc.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://hq.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://qb.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://oe.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sl.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://xg.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tj.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://nc.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fd.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ht.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rh.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dx.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bq.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hx.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ws.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yf.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://rc.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://ci.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vx.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hl.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qc.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://fu.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ay.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://go.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gy.shxzskj.cn

[J06] 计算两时间之差
来源：http://fl.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://ie.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://eq.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sd.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://et.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bu.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://dd.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://fd.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://ny.nszjky.cn

[J07] 比较两个日期
来源：http://tz.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://qn.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eg.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ky.shxzukj.cn


<!-- 参考信息 -->