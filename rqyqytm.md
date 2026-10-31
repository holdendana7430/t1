代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://fi.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vg.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qs.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://gn.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://ix.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://bm.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hf.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://jp.bjjhwx.cn

[G10] 访问控制
来源：http://bf.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://jt.gzmigu.cn

PHP:  public / protected / private
来源：http://fz.nszjky.cn

JS:   #private 字段；其余公开
来源：http://ep.jctech888.com.cn

TS:   public / protected / private
来源：http://bg.asd995.cn

Java: public / protected / private / 默认包级
来源：http://lp.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qn.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://gg.colortex.cn

C#:   public / protected / private / internal
来源：http://ae.jianghongdianzi.cn

[G11] getter / setter
来源：http://fj.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://qj.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://db.9csxet.cn

JS:   get name() { return this._name; }
来源：http://ab.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://sx.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://wm.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cx.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://kd.huanxung.cn

C#:   public string Name { get; set; }
来源：http://mo.muxihuayi.cn

[G12] 对象转字符串
来源：http://zs.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://nj.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gz.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://bt.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://hq.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://fp.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jx.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://vw.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://eo.colortex.cn

[G13] 判断对象类型
来源：http://sg.huanxung.cn

Py:   isinstance(u, User)
来源：http://yz.haigaiapp.cn

PHP:  $u instanceof User
来源：http://qf.yuntaijiaju.cn

JS:   u instanceof User
来源：http://dz.jctech888.com.cn

TS:   u instanceof User
来源：http://bk.asd995.cn

Java: u instanceof User
来源：http://gf.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uf.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://ll.bookmarksfly.cn

C#:   u is User
来源：http://qa.521024.cn

[G14] 数据类 / record
来源：http://am.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ii.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://tv.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://io.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://ru.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://xq.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://xy.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://is.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://sa.panjiajie.cn

[G15] 枚举
来源：http://zr.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fn.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bg.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sq.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jz.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://qv.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ln.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://dh.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lj.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://zl.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hg.521024.cn

PHP:  get_object_vars($obj);
来源：http://ku.gzmigu.cn

JS:   Object.entries(obj)
来源：http://ad.colortex.cn

TS:   Object.entries(obj)
来源：http://tq.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ng.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bo.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://av.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://rl.asd995.cn

================================================================================
来源：http://jf.nicolike.cn

H. 异常与错误处理
来源：http://jt.asd995.cn

================================================================================
来源：http://vh.shxzukj.cn

[H01] try / catch 基础
来源：http://qu.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lk.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rf.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tj.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lw.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dd.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cx.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xe.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hm.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://cx.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xk.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kw.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ic.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rz.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://os.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ra.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://to.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lk.szxytkj.cn

[H03] 主动抛出异常
来源：http://dx.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://of.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gk.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://ur.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://dl.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zu.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sw.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xf.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kh.521024.cn

[H04] 自定义异常类型
来源：http://mj.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://fq.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ce.newstarts.cn

JS:   class MyError extends Error {}
来源：http://ur.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://js.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://sg.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ha.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://nd.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://rq.szsharing.cn

[H05] 捕获特定类型
来源：http://rq.lnxyls.cn

Py:   except ValueError as e:
来源：http://rv.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sx.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://kz.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://lf.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://ot.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kv.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://xd.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cb.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://sp.szsharing.cn

Py:   value = d.get("k") or default
来源：http://ts.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wl.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zb.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://im.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jl.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ff.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://xr.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://id.haigaiapp.cn

[H07] 断言
来源：http://dj.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://il.shxzskj.cn

PHP:  assert($x > 0);
来源：http://uo.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://uu.colortex.cn

TS:   console.assert(x > 0);
来源：http://ml.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://lq.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gn.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fv.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://vi.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://xt.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://uk.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gy.hahajie.cn

JS:   e.message;  e.stack
来源：http://nx.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lt.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zx.huanxung.cn

Go:   err.Error()
来源：http://si.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://ld.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://pq.szxytkj.cn

[H09] 带错误码的异常
来源：http://zq.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lg.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ft.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ph.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tv.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bz.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sj.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fo.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yr.bookmarksfly.cn

[H10] 资源自动释放
来源：http://nl.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tk.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hh.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xy.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lx.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://io.asd995.cn

Go:   defer f.Close()
来源：http://xz.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ea.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ll.9csxet.cn

================================================================================
来源：http://tt.huixiangedu.cn

I. 正则表达式
来源：http://ml.wgjwhj.cn

================================================================================
来源：http://nn.shxzukj.cn

[I01] 判断是否匹配
来源：http://mz.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qk.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vk.colortex.cn

JS:   /\d+/.test(s)
来源：http://mu.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://cc.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mq.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qg.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://vt.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rm.huanxung.cn

[I02] 提取所有匹配
来源：http://qp.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://bb.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bq.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xc.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://bo.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jn.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://do.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://rh.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://va.gzmigu.cn

[I03] 提取捕获分组
来源：http://ay.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ks.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ow.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zn.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ya.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ie.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ex.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://so.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zh.szsharing.cn

[I04] 正则替换
来源：http://so.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://da.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ei.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yj.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ci.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://db.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gl.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sa.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://px.gzmigu.cn

[I05] 按正则拆分
来源：http://qv.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mv.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wf.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://sh.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://mc.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://cc.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ld.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qb.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cj.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jx.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dw.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yf.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bx.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nt.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rl.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sv.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cw.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ne.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://sg.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xg.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sv.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lr.huixiangedu.cn

TS:   /error/gim
来源：http://dp.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://if.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wq.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://bp.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bz.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://yl.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://la.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ne.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bw.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lf.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oo.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ue.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zg.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bm.shtwfgs.cn

================================================================================
来源：http://vl.lnxyls.cn

J. 日期与时间
来源：http://ex.colortex.cn

================================================================================
来源：http://ue.colortex.cn

[J01] 获取当前时间
来源：http://jz.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://om.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wz.asd995.cn

JS:   new Date();  Date.now()
来源：http://gw.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://mn.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rp.jianghongdianzi.cn

Go:   time.Now()
来源：http://lb.hnjuh.cn

Ruby: Time.now
来源：http://xs.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wx.shxzskj.cn

[J02] 格式化输出
来源：http://zy.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dv.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://du.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rl.asd995.cn

TS:   d.toISOString()
来源：http://mz.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ic.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://az.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mg.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://px.colortex.cn

[J03] 字符串解析为日期
来源：http://bd.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ni.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tr.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://dj.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://oz.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ay.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ld.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://ii.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yc.nicolike.cn

[J04] 时间戳与日期互转
来源：http://tn.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://at.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oe.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zf.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oz.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yh.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ka.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ag.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pp.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://zv.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://wp.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ad.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rx.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://na.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://uu.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mg.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://it.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bs.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://zm.521024.cn

Py:   (end - start).total_seconds()
来源：http://be.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://uv.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hm.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pi.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uv.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://bo.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://tk.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://lk.hnjuh.cn

[J07] 比较两个日期
来源：http://hs.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://bt.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ks.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ux.hahajie.cn


<!-- 参考信息 -->