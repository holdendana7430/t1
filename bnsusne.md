代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://ov.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ms.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sp.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://kl.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://ze.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://iu.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ya.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://xy.521024.cn

[G10] 访问控制
来源：http://lw.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://hc.muxihuayi.cn

PHP:  public / protected / private
来源：http://zk.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://gw.gzmigu.cn

TS:   public / protected / private
来源：http://xl.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://un.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qu.chemitech.net.cn

Ruby: public / protected / private
来源：http://ri.szxytkj.cn

C#:   public / protected / private / internal
来源：http://iq.shtwfgs.cn

[G11] getter / setter
来源：http://yg.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://rt.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dh.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://di.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://tm.hahajie.cn

Java: public String getName() { return name; }
来源：http://qn.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rd.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://fr.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://vq.hahajie.cn

[G12] 对象转字符串
来源：http://il.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://bz.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kd.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://px.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://og.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://tm.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uu.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://fb.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://uq.gzmigu.cn

[G13] 判断对象类型
来源：http://yo.nicolike.cn

Py:   isinstance(u, User)
来源：http://nk.shtwfgs.cn

PHP:  $u instanceof User
来源：http://bw.yuntaijiaju.cn

JS:   u instanceof User
来源：http://yl.yuntaijiaju.cn

TS:   u instanceof User
来源：http://fa.521024.cn

Java: u instanceof User
来源：http://jo.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ps.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://vb.9csxet.cn

C#:   u is User
来源：http://pi.9csxet.cn

[G14] 数据类 / record
来源：http://xg.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rs.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://cd.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://by.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://of.hahajie.cn

Java: record User(String name, int age) {}
来源：http://fm.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://io.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yp.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://cd.huanxung.cn

[G15] 枚举
来源：http://wb.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mh.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nu.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tk.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qo.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://su.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xy.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://zs.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://my.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://lv.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gq.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://ct.521024.cn

JS:   Object.entries(obj)
来源：http://ht.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://gj.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cn.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zg.nszjky.cn

Ruby: obj.instance_variables
来源：http://rn.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://lt.chemitech.net.cn

================================================================================
来源：http://mz.bjjhwx.cn

H. 异常与错误处理
来源：http://pa.chemitech.net.cn

================================================================================
来源：http://vi.shtwfgs.cn

[H01] try / catch 基础
来源：http://ml.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kp.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ud.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iy.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cr.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bv.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ah.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fm.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lx.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://vh.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yy.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://og.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://et.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nq.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://us.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vb.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bu.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pv.huanxung.cn

[H03] 主动抛出异常
来源：http://lg.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://ou.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://si.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://sc.521024.cn

TS:   throw new Error("错误信息");
来源：http://za.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://un.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nm.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tr.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ta.chemitech.net.cn

[H04] 自定义异常类型
来源：http://jz.521024.cn

Py:   class MyError(Exception): pass
来源：http://oe.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cr.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://mq.nicolike.cn

TS:   class MyError extends Error {}
来源：http://zz.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://kv.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mg.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://sd.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://pc.asd995.cn

[H05] 捕获特定类型
来源：http://gr.shxzskj.cn

Py:   except ValueError as e:
来源：http://zu.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yp.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://qo.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://jb.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://qy.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ya.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://ua.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ep.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://mu.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://dn.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gf.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zf.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xz.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gj.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ph.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://mx.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://kp.szsharing.cn

[H07] 断言
来源：http://il.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://sa.panjiajie.cn

PHP:  assert($x > 0);
来源：http://ip.nicolike.cn

JS:   console.assert(x > 0);
来源：http://ef.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://mf.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://gq.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wm.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uw.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://hn.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://db.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://ga.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://af.szsharing.cn

JS:   e.message;  e.stack
来源：http://rs.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zb.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://op.shxzskj.cn

Go:   err.Error()
来源：http://lh.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://cp.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://xw.asd995.cn

[H09] 带错误码的异常
来源：http://cs.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uq.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tg.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ai.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://en.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://le.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://co.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bx.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ef.newstarts.cn

[H10] 资源自动释放
来源：http://fb.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wm.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fj.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fn.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://si.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ty.nicolike.cn

Go:   defer f.Close()
来源：http://xa.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zq.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://my.lnxyls.cn

================================================================================
来源：http://wj.yuexingan06.cn

I. 正则表达式
来源：http://ny.shxzukj.cn

================================================================================
来源：http://nt.muxihuayi.cn

[I01] 判断是否匹配
来源：http://of.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qq.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ct.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://bb.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://qk.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vp.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qm.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://zk.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ez.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://mq.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://ct.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yb.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://av.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://yw.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fn.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kx.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://mw.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://en.yuexingan06.cn

[I03] 提取捕获分组
来源：http://lf.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hv.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rj.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ep.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xv.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nz.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xr.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bf.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cg.haigaiapp.cn

[I04] 正则替换
来源：http://dj.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://td.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ky.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jn.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dg.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zf.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zk.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vt.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ix.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://lh.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ok.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bc.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://fr.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://ti.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://zj.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ha.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cq.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://so.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ku.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ve.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jn.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cq.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dv.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fn.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ld.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mx.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hf.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://fq.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wx.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lk.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pn.muxihuayi.cn

TS:   /error/gim
来源：http://jn.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vt.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ew.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://gn.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lo.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://sh.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uz.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jp.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ws.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wa.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://br.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tm.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uc.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ts.shxzskj.cn

================================================================================
来源：http://lu.wgjwhj.cn

J. 日期与时间
来源：http://qt.nicolike.cn

================================================================================
来源：http://ft.9csxet.cn

[J01] 获取当前时间
来源：http://mq.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://je.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gd.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://gi.nszjky.cn

TS:   new Date();  Date.now()
来源：http://as.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zg.panjiajie.cn

Go:   time.Now()
来源：http://wj.huixiangedu.cn

Ruby: Time.now
来源：http://xn.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zy.9csxet.cn

[J02] 格式化输出
来源：http://tz.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://av.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ss.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cy.gzmigu.cn

TS:   d.toISOString()
来源：http://wf.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xn.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jy.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nl.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cm.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://qr.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hh.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zc.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://xs.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://pw.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vy.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yx.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://be.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ob.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://ze.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://og.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uo.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sp.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ot.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://en.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xi.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://el.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rx.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://jc.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://pd.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jw.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bf.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kx.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://vc.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://br.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://gx.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rm.521024.cn

[J06] 计算两时间之差
来源：http://wf.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://xj.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://ol.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ke.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://od.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://th.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://ew.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://hc.521024.cn

C#:   (end - start).TotalSeconds
来源：http://gx.nicolike.cn

[J07] 比较两个日期
来源：http://cq.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://yo.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://br.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://il.lnxyls.cn


<!-- 参考信息 -->