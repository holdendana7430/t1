代发 wailian999

PHP:  public static function f() {}
来源：http://cz.huanxung.cn

JS:   static f() {}
来源：http://eq.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://iz.nicolike.cn

Java: static void f() {}
来源：http://ij.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cp.wgjwhj.cn

Ruby: def self.f; end
来源：http://fn.shxzskj.cn

C#:   public static void F() {}
来源：http://pk.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://gc.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://bw.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ue.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jn.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://zn.9csxet.cn

Java: interface Shape { double area(); }
来源：http://il.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://ix.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xc.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://qt.shtwfgs.cn

[G10] 访问控制
来源：http://ya.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://br.chemitech.net.cn

PHP:  public / protected / private
来源：http://zn.9csxet.cn

JS:   #private 字段；其余公开
来源：http://np.huixinmuqiang.cn

TS:   public / protected / private
来源：http://ws.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://ai.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://we.muxihuayi.cn

Ruby: public / protected / private
来源：http://db.shxzukj.cn

C#:   public / protected / private / internal
来源：http://by.szsharing.cn

[G11] getter / setter
来源：http://xk.asd995.cn

Py:   @property 与 @x.setter
来源：http://qb.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pi.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://lv.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://gx.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://jz.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qq.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://hw.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://va.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://ly.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://zb.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cc.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://db.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://fl.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://el.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vc.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://xn.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://kw.yuexingan06.cn

[G13] 判断对象类型
来源：http://ng.lnxyls.cn

Py:   isinstance(u, User)
来源：http://og.szsharing.cn

PHP:  $u instanceof User
来源：http://og.haigaiapp.cn

JS:   u instanceof User
来源：http://yv.szsharing.cn

TS:   u instanceof User
来源：http://pe.nszjky.cn

Java: u instanceof User
来源：http://br.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ii.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://mj.chemitech.net.cn

C#:   u is User
来源：http://il.panjiajie.cn

[G14] 数据类 / record
来源：http://fe.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sw.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://jf.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vg.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://nd.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://ga.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://rc.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://it.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://ga.yuexingan06.cn

[G15] 枚举
来源：http://uo.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://at.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bk.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://md.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://db.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://zm.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kx.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://ol.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gy.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://mg.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://al.asd995.cn

PHP:  get_object_vars($obj);
来源：http://yj.gzmigu.cn

JS:   Object.entries(obj)
来源：http://rp.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://vn.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://is.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zc.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://jv.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://cr.hnjuh.cn

================================================================================
来源：http://kt.yuntaijiaju.cn

H. 异常与错误处理
来源：http://oj.chemitech.net.cn

================================================================================
来源：http://ni.lnxyls.cn

[H01] try / catch 基础
来源：http://qj.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vs.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eh.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://am.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zb.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://es.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ts.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hc.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xp.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ba.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tp.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sa.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tf.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yc.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uf.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vz.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bt.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ag.9csxet.cn

[H03] 主动抛出异常
来源：http://gw.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://oo.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dd.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://lp.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://sb.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://af.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vz.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mu.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yj.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://hn.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://fn.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qa.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://bx.nicolike.cn

TS:   class MyError extends Error {}
来源：http://ev.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://ew.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dy.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://lx.nszjky.cn

C#:   class MyException : Exception {}
来源：http://zu.chemitech.net.cn

[H05] 捕获特定类型
来源：http://qu.haigaiapp.cn

Py:   except ValueError as e:
来源：http://tj.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dx.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://kd.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://bh.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://cx.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qh.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://fp.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cd.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://ki.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://mr.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kd.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rk.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uw.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yg.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tq.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://ax.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://br.yuntaijiaju.cn

[H07] 断言
来源：http://ha.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://yh.newstarts.cn

PHP:  assert($x > 0);
来源：http://ft.9csxet.cn

JS:   console.assert(x > 0);
来源：http://by.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://gy.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://ae.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://po.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://la.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://ii.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://uh.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ml.colortex.cn

JS:   e.message;  e.stack
来源：http://wb.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hp.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tu.huanxung.cn

Go:   err.Error()
来源：http://bf.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://hy.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://kd.colortex.cn

[H09] 带错误码的异常
来源：http://fk.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sl.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mn.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ok.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nx.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xh.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oa.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rl.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mr.chemitech.net.cn

[H10] 资源自动释放
来源：http://wl.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://of.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tx.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zh.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hq.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://er.hahajie.cn

Go:   defer f.Close()
来源：http://ml.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xt.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qf.asd995.cn

================================================================================
来源：http://jr.jctech888.com.cn

I. 正则表达式
来源：http://nt.huanxung.cn

================================================================================
来源：http://ui.colortex.cn

[I01] 判断是否匹配
来源：http://lp.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eh.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qf.szsharing.cn

JS:   /\d+/.test(s)
来源：http://du.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://hr.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ko.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uj.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://yr.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mj.nicolike.cn

[I02] 提取所有匹配
来源：http://lk.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://zf.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ja.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uj.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://fb.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://um.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oc.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://rr.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://af.jctech888.com.cn

[I03] 提取捕获分组
来源：http://mc.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qn.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ja.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://py.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zb.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ux.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cb.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qr.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uv.shxzukj.cn

[I04] 正则替换
来源：http://qq.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nk.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tj.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://au.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ym.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ly.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hm.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qz.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dd.wgjwhj.cn

[I05] 按正则拆分
来源：http://mf.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mi.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jf.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://ca.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://cp.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://ba.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zr.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sf.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uy.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mw.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oz.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bh.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ue.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vo.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vo.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ua.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jx.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://os.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://gd.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://al.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://px.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qs.nicolike.cn

TS:   /error/gim
来源：http://ui.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bi.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xc.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://bx.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oj.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://zv.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://by.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mz.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ji.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://co.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dp.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kw.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bc.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://us.nszjky.cn

================================================================================
来源：http://fz.wgjwhj.cn

J. 日期与时间
来源：http://au.jctech888.com.cn

================================================================================
来源：http://no.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://wa.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vs.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://gu.asd995.cn

TS:   new Date();  Date.now()
来源：http://oo.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zj.jianghongdianzi.cn

Go:   time.Now()
来源：http://re.panjiajie.cn

Ruby: Time.now
来源：http://cu.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tn.panjiajie.cn

[J02] 格式化输出
来源：http://vm.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qv.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://if.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://em.huixiangedu.cn

TS:   d.toISOString()
来源：http://os.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dx.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jr.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dq.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qp.szxytkj.cn

[J03] 字符串解析为日期
来源：http://fi.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ca.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ly.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://ny.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://dq.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://di.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ld.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://cq.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ge.colortex.cn

[J04] 时间戳与日期互转
来源：http://ez.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nj.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sk.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qe.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sz.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jj.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jx.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lf.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tm.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://mw.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://ia.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pl.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ok.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://op.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://aq.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qi.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://vd.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xb.haigaiapp.cn

[J06] 计算两时间之差
来源：http://vc.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://rf.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://cy.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nl.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rs.huixinmuqiang.cn


<!-- 参考信息 -->