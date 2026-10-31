代发 wailian999

Java: interface Shape { double area(); }
来源：http://sb.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://ca.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mi.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://qz.wgjwhj.cn

[G10] 访问控制
来源：http://rz.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://yg.bjjhwx.cn

PHP:  public / protected / private
来源：http://wg.hahajie.cn

JS:   #private 字段；其余公开
来源：http://ci.panjiajie.cn

TS:   public / protected / private
来源：http://jf.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://or.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gy.bookmarksfly.cn

Ruby: public / protected / private
来源：http://td.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://hs.asd995.cn

[G11] getter / setter
来源：http://uq.521024.cn

Py:   @property 与 @x.setter
来源：http://vb.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ei.newstarts.cn

JS:   get name() { return this._name; }
来源：http://wf.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://gk.nicolike.cn

Java: public String getName() { return name; }
来源：http://vn.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hi.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://iw.huanxung.cn

C#:   public string Name { get; set; }
来源：http://wk.huanxung.cn

[G12] 对象转字符串
来源：http://nb.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://ul.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dy.nszjky.cn

JS:   toString() { return this.name; }
来源：http://ig.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://db.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://og.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kr.newstarts.cn

Ruby: def to_s; @name; end
来源：http://hz.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://im.szxytkj.cn

[G13] 判断对象类型
来源：http://wg.521024.cn

Py:   isinstance(u, User)
来源：http://sm.szsharing.cn

PHP:  $u instanceof User
来源：http://iv.huanxung.cn

JS:   u instanceof User
来源：http://kr.wgjwhj.cn

TS:   u instanceof User
来源：http://bm.huanxung.cn

Java: u instanceof User
来源：http://vs.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oh.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://bm.hahajie.cn

C#:   u is User
来源：http://za.shxzukj.cn

[G14] 数据类 / record
来源：http://xi.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jm.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://ey.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wv.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://rs.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://iw.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://oa.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ds.521024.cn

C#:   record User(string Name, int Age);
来源：http://bv.bjjhwx.cn

[G15] 枚举
来源：http://wl.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bh.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wq.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://la.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://td.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://oy.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hj.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://bo.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ts.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://js.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ao.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://wc.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://cx.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://mq.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iu.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gi.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://tz.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ya.hnjuh.cn

================================================================================
来源：http://kr.huanxung.cn

H. 异常与错误处理
来源：http://uy.jctech888.com.cn

================================================================================
来源：http://jp.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://xn.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eo.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sm.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ss.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ux.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ol.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qx.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xq.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mw.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://zq.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://co.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://id.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gl.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xk.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://iv.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zl.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gm.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ms.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://qj.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://qv.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ov.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://qr.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://lz.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bn.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zt.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wl.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lp.hahajie.cn

[H04] 自定义异常类型
来源：http://qn.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://gs.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qb.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://bi.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://dh.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://tx.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://we.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://qo.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://ts.szxytkj.cn

[H05] 捕获特定类型
来源：http://hl.huanxung.cn

Py:   except ValueError as e:
来源：http://cd.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oy.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://xd.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://je.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://kk.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nz.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://op.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gb.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://vo.521024.cn

Py:   value = d.get("k") or default
来源：http://bd.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://td.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fh.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iy.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xp.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dw.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://vx.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://mj.hnjuh.cn

[H07] 断言
来源：http://eg.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://ve.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://vn.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://ix.nszjky.cn

TS:   console.assert(x > 0);
来源：http://cy.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://lx.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eq.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gj.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://ao.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://ej.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ek.newstarts.cn

JS:   e.message;  e.stack
来源：http://rl.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zq.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nv.szsharing.cn

Go:   err.Error()
来源：http://rd.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://mf.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://cz.shxzukj.cn

[H09] 带错误码的异常
来源：http://ls.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ll.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ea.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ej.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ro.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://je.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kx.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tl.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://br.asd995.cn

[H10] 资源自动释放
来源：http://kf.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dk.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://da.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ti.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ia.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qm.panjiajie.cn

Go:   defer f.Close()
来源：http://wz.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gc.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dk.yuexingan06.cn

================================================================================
来源：http://ix.colortex.cn

I. 正则表达式
来源：http://tg.huixiangedu.cn

================================================================================
来源：http://cp.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://dt.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zk.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://py.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://ui.nszjky.cn

TS:   /\d+/.test(s)
来源：http://cn.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bn.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ri.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://ie.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cl.shxzskj.cn

[I02] 提取所有匹配
来源：http://al.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://ls.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ny.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wx.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://sp.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://us.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qe.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://fl.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ie.huixiangedu.cn

[I03] 提取捕获分组
来源：http://xi.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bl.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rk.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vm.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aw.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bv.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ja.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zi.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cq.bjjhwx.cn

[I04] 正则替换
来源：http://fn.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tz.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dq.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fx.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tb.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://av.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ai.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ri.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lf.hnjuh.cn

[I05] 按正则拆分
来源：http://zg.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fx.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rr.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://fg.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://yr.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://ap.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lh.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xd.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://je.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://od.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nl.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zs.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bc.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fh.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oi.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uf.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ot.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jf.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://bs.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qo.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ob.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xg.yuntaijiaju.cn

TS:   /error/gim
来源：http://cl.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://za.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ob.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://uo.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ps.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://oq.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sx.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ah.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ec.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jq.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xj.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jz.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wj.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lp.szsharing.cn

================================================================================
来源：http://gh.huixiangedu.cn

J. 日期与时间
来源：http://lq.wgjwhj.cn

================================================================================
来源：http://eh.muxihuayi.cn

[J01] 获取当前时间
来源：http://kp.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hm.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zn.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://kd.asd995.cn

TS:   new Date();  Date.now()
来源：http://uy.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ve.huixiangedu.cn

Go:   time.Now()
来源：http://ps.haigaiapp.cn

Ruby: Time.now
来源：http://hv.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ct.lnxyls.cn

[J02] 格式化输出
来源：http://sq.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://or.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lo.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qu.521024.cn

TS:   d.toISOString()
来源：http://vk.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cz.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yf.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hm.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xp.huanxung.cn

[J03] 字符串解析为日期
来源：http://vt.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://az.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aj.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://ko.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://df.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vc.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ch.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ed.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cy.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://we.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oc.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hx.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dt.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://py.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://th.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://km.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gn.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jn.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://ng.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://in.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ve.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bt.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oi.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://es.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vx.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://we.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yx.huanxung.cn

[J06] 计算两时间之差
来源：http://io.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://fi.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://de.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ik.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oz.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dg.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://fs.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://nu.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://pr.521024.cn

[J07] 比较两个日期
来源：http://oy.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://xw.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://so.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tf.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ek.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dm.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ml.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://md.shxzukj.cn


<!-- 参考信息 -->