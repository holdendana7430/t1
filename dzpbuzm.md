代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://nj.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wn.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xu.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://ak.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://fg.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://by.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gm.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://hy.shxzukj.cn

[G10] 访问控制
来源：http://pa.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://fu.newstarts.cn

PHP:  public / protected / private
来源：http://el.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://je.shxzskj.cn

TS:   public / protected / private
来源：http://ke.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://jm.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qc.nicolike.cn

Ruby: public / protected / private
来源：http://sc.nszjky.cn

C#:   public / protected / private / internal
来源：http://vq.gzmigu.cn

[G11] getter / setter
来源：http://xr.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://xg.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yy.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://qa.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://qm.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://qs.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://db.asd995.cn

Ruby: attr_accessor :name
来源：http://tg.521024.cn

C#:   public string Name { get; set; }
来源：http://lv.nicolike.cn

[G12] 对象转字符串
来源：http://ys.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://wi.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://km.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://un.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://cd.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://jk.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wp.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://yx.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://kk.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://tq.hnjuh.cn

Py:   isinstance(u, User)
来源：http://xi.shtwfgs.cn

PHP:  $u instanceof User
来源：http://qm.jctech888.com.cn

JS:   u instanceof User
来源：http://xp.colortex.cn

TS:   u instanceof User
来源：http://oi.bookmarksfly.cn

Java: u instanceof User
来源：http://qb.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ik.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://vf.szsharing.cn

C#:   u is User
来源：http://dt.jctech888.com.cn

[G14] 数据类 / record
来源：http://xo.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ub.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://fy.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cm.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://hc.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://xl.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://ak.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://li.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://rq.yuexingan06.cn

[G15] 枚举
来源：http://gd.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gj.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://px.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ya.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oq.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://ev.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bv.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://bo.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ch.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://vp.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xs.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://yg.9csxet.cn

JS:   Object.entries(obj)
来源：http://pb.huanxung.cn

TS:   Object.entries(obj)
来源：http://lj.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iu.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uy.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://tf.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ri.shxzukj.cn

================================================================================
来源：http://iu.szsharing.cn

H. 异常与错误处理
来源：http://of.shxzukj.cn

================================================================================
来源：http://rm.hnjuh.cn

[H01] try / catch 基础
来源：http://ty.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gt.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ww.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jj.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zr.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aj.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fa.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://du.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ki.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://ic.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iq.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ri.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mz.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kz.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dr.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bp.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ih.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ol.haigaiapp.cn

[H03] 主动抛出异常
来源：http://if.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://em.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yz.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://sx.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://xl.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://py.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://us.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kt.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uw.haigaiapp.cn

[H04] 自定义异常类型
来源：http://nf.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://ia.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dj.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://vz.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://yk.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://iv.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nb.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://yi.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://oj.shxzskj.cn

[H05] 捕获特定类型
来源：http://er.521024.cn

Py:   except ValueError as e:
来源：http://em.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fs.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://rg.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://lv.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://gc.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bg.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://dq.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hf.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://mz.nicolike.cn

Py:   value = d.get("k") or default
来源：http://gb.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bg.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fq.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ve.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jn.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fm.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://gk.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://fv.nszjky.cn

[H07] 断言
来源：http://rv.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://oi.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://lw.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://lo.colortex.cn

TS:   console.assert(x > 0);
来源：http://la.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://th.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ye.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yi.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://aq.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://gp.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://sa.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sr.huanxung.cn

JS:   e.message;  e.stack
来源：http://qc.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kp.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qj.huixiangedu.cn

Go:   err.Error()
来源：http://qi.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://ek.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://va.jctech888.com.cn

[H09] 带错误码的异常
来源：http://gf.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gi.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ia.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ko.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tu.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://py.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dj.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://co.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://un.jctech888.com.cn

[H10] 资源自动释放
来源：http://qq.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bi.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qk.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bc.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://or.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sl.szxytkj.cn

Go:   defer f.Close()
来源：http://zv.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qg.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cu.shxzukj.cn

================================================================================
来源：http://yv.yuntaijiaju.cn

I. 正则表达式
来源：http://yv.shxzskj.cn

================================================================================
来源：http://rc.chemitech.net.cn

[I01] 判断是否匹配
来源：http://np.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gj.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ue.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://im.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://wu.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qi.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ao.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://cx.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bj.nszjky.cn

[I02] 提取所有匹配
来源：http://vn.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://ln.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hq.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xa.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://mj.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sp.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nb.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://yk.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zk.huixiangedu.cn

[I03] 提取捕获分组
来源：http://uj.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vl.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ms.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://as.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://al.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cb.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kp.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tu.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tp.huixinmuqiang.cn

[I04] 正则替换
来源：http://ia.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wt.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ts.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pv.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ks.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://aa.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sf.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uc.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ry.newstarts.cn

[I05] 按正则拆分
来源：http://ug.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pu.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lb.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://ui.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://if.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://nq.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rl.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gy.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dk.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ue.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yy.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cl.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ef.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zu.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wr.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xt.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rs.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dm.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://eb.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ej.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xu.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sx.jctech888.com.cn

TS:   /error/gim
来源：http://ya.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zt.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pz.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://wa.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jc.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://gi.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uy.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lg.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ko.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ya.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wo.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cq.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gq.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tm.hahajie.cn

================================================================================
来源：http://ip.muxihuayi.cn

J. 日期与时间
来源：http://re.chemitech.net.cn

================================================================================
来源：http://fd.colortex.cn

[J01] 获取当前时间
来源：http://rg.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kq.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://up.9csxet.cn

JS:   new Date();  Date.now()
来源：http://im.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://tp.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kk.521024.cn

Go:   time.Now()
来源：http://pp.huanxung.cn

Ruby: Time.now
来源：http://ck.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oo.shxzskj.cn

[J02] 格式化输出
来源：http://kb.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bb.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hp.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://as.hahajie.cn

TS:   d.toISOString()
来源：http://tr.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ca.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ht.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://al.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gt.newstarts.cn

[J03] 字符串解析为日期
来源：http://om.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tl.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eg.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://dp.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://lj.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pu.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ds.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://zc.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zv.521024.cn

[J04] 时间戳与日期互转
来源：http://hn.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dw.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://op.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hs.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cj.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zv.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qj.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vh.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jq.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://jx.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://vv.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uy.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ca.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ef.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://qu.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jm.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://zl.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ld.9csxet.cn

[J06] 计算两时间之差
来源：http://yt.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://bi.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://qh.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cr.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yz.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ey.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://ky.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://zq.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://lh.asd995.cn

[J07] 比较两个日期
来源：http://nv.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://wl.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ky.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mg.nszjky.cn


<!-- 参考信息 -->