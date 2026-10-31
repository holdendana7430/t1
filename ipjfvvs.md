代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hj.9csxet.cn

Ruby: def self.f; end
来源：http://xl.huanxung.cn

C#:   public static void F() {}
来源：http://fl.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://yn.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://gz.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ia.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://he.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://kt.nszjky.cn

Java: interface Shape { double area(); }
来源：http://oj.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://pr.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mo.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://tx.lnxyls.cn

[G10] 访问控制
来源：http://mt.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://wo.bjjhwx.cn

PHP:  public / protected / private
来源：http://ht.newstarts.cn

JS:   #private 字段；其余公开
来源：http://we.shtwfgs.cn

TS:   public / protected / private
来源：http://hp.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://db.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rd.asd995.cn

Ruby: public / protected / private
来源：http://lw.colortex.cn

C#:   public / protected / private / internal
来源：http://hb.szxytkj.cn

[G11] getter / setter
来源：http://dp.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://qt.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eq.szsharing.cn

JS:   get name() { return this._name; }
来源：http://tu.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://tq.nszjky.cn

Java: public String getName() { return name; }
来源：http://vx.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wi.9csxet.cn

Ruby: attr_accessor :name
来源：http://gs.newstarts.cn

C#:   public string Name { get; set; }
来源：http://fd.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://mg.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://wy.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gy.nicolike.cn

JS:   toString() { return this.name; }
来源：http://fc.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://zv.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://bw.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ja.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://dy.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://wp.hahajie.cn

[G13] 判断对象类型
来源：http://on.shxzukj.cn

Py:   isinstance(u, User)
来源：http://xy.panjiajie.cn

PHP:  $u instanceof User
来源：http://fg.huixiangedu.cn

JS:   u instanceof User
来源：http://ro.shxzukj.cn

TS:   u instanceof User
来源：http://lj.shxzukj.cn

Java: u instanceof User
来源：http://nt.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mb.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://sf.colortex.cn

C#:   u is User
来源：http://ik.lnxyls.cn

[G14] 数据类 / record
来源：http://uf.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vq.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://yq.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qx.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://sj.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://ls.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://bk.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ce.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://pq.jianghongdianzi.cn

[G15] 枚举
来源：http://fg.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fw.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gs.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dd.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vo.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://vs.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kx.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://tc.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uj.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://om.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ds.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://yw.gzmigu.cn

JS:   Object.entries(obj)
来源：http://it.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://vb.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wp.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yi.hnjuh.cn

Ruby: obj.instance_variables
来源：http://to.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ic.huixinmuqiang.cn

================================================================================
来源：http://qh.yuexingan06.cn

H. 异常与错误处理
来源：http://rv.gzmigu.cn

================================================================================
来源：http://tj.hnjuh.cn

[H01] try / catch 基础
来源：http://yv.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xc.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ph.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://an.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ad.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xg.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qv.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mn.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lb.newstarts.cn

[H02] finally / ensure 收尾
来源：http://vb.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://su.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xi.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rz.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ch.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vr.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://of.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uu.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ri.yuexingan06.cn

[H03] 主动抛出异常
来源：http://bn.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://aa.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ia.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://gx.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://bv.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jv.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yr.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://di.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rh.shxzskj.cn

[H04] 自定义异常类型
来源：http://yu.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://yq.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wi.szsharing.cn

JS:   class MyError extends Error {}
来源：http://cs.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://ss.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://bk.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ym.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://hs.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://fi.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://zr.521024.cn

Py:   except ValueError as e:
来源：http://uw.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jd.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://vm.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://zn.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://ev.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jx.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://to.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fv.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://pc.521024.cn

Py:   value = d.get("k") or default
来源：http://hy.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dh.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bl.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ue.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lo.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fn.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://nz.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://eq.colortex.cn

[H07] 断言
来源：http://vv.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://fh.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://ni.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://ha.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://eo.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://ie.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ey.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dx.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://zd.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://bc.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://zr.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xv.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://ti.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bi.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vx.nicolike.cn

Go:   err.Error()
来源：http://em.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://gr.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://am.shxzukj.cn

[H09] 带错误码的异常
来源：http://bm.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://am.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ts.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kp.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ji.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qe.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://om.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dk.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ci.bjjhwx.cn

[H10] 资源自动释放
来源：http://yz.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ny.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ch.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ez.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kt.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bp.chemitech.net.cn

Go:   defer f.Close()
来源：http://hu.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://el.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fq.newstarts.cn

================================================================================
来源：http://vh.szxytkj.cn

I. 正则表达式
来源：http://fo.hahajie.cn

================================================================================
来源：http://gt.gzmigu.cn

[I01] 判断是否匹配
来源：http://xx.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oa.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kh.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://np.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://sl.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://st.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ao.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://su.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zp.muxihuayi.cn

[I02] 提取所有匹配
来源：http://rj.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://on.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xc.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bz.colortex.cn

TS:   s.match(/\d+/g)
来源：http://ad.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gj.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mw.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://xq.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tx.hnjuh.cn

[I03] 提取捕获分组
来源：http://al.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ir.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ba.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wq.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pe.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ac.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ud.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mt.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kk.muxihuayi.cn

[I04] 正则替换
来源：http://bg.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hg.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ww.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rf.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lb.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mp.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nr.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://de.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gc.szsharing.cn

[I05] 按正则拆分
来源：http://uc.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ln.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://la.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://il.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://bm.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://wj.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pa.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ak.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gu.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ux.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yu.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jv.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fu.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://af.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gr.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pj.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vn.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bo.521024.cn

[I07] 忽略大小写与多行模式
来源：http://lw.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ca.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ef.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nq.hnjuh.cn

TS:   /error/gim
来源：http://dd.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lm.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jp.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://ec.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lp.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://wl.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://am.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ms.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://se.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zf.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cz.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pp.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ko.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jc.newstarts.cn

================================================================================
来源：http://xo.jctech888.com.cn

J. 日期与时间
来源：http://oj.nicolike.cn

================================================================================
来源：http://yr.colortex.cn

[J01] 获取当前时间
来源：http://om.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ta.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ei.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://oj.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://cn.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nl.yuntaijiaju.cn

Go:   time.Now()
来源：http://ck.jctech888.com.cn

Ruby: Time.now
来源：http://rs.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ca.jctech888.com.cn

[J02] 格式化输出
来源：http://wz.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sw.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kz.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://av.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://vr.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kn.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://do.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zg.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ex.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://te.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ln.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ph.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://on.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://cc.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zn.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kj.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://tp.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ko.szsharing.cn

[J04] 时间戳与日期互转
来源：http://ot.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xs.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rg.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dk.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eg.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ca.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sf.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ly.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cu.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://yp.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://nm.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wq.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tf.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://er.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://sy.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ey.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://ns.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pr.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://zg.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://tb.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://xq.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pq.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gc.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ma.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://nd.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://cm.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://bn.huixiangedu.cn


<!-- 参考信息 -->