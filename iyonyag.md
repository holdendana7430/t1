代发 wailian999

PHP:  public static function f() {}
来源：http://rl.bookmarksfly.cn

JS:   static f() {}
来源：http://ut.nszjky.cn

TS:   static f(): void {}
来源：http://vf.chemitech.net.cn

Java: static void f() {}
来源：http://rf.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cb.gzmigu.cn

Ruby: def self.f; end
来源：http://lu.nicolike.cn

C#:   public static void F() {}
来源：http://zc.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://dy.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://bv.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mu.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://po.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://ru.nszjky.cn

Java: interface Shape { double area(); }
来源：http://wd.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://am.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://og.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://lq.chemitech.net.cn

[G10] 访问控制
来源：http://ie.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://yl.gzmigu.cn

PHP:  public / protected / private
来源：http://ap.nicolike.cn

JS:   #private 字段；其余公开
来源：http://ru.colortex.cn

TS:   public / protected / private
来源：http://dj.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://lt.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mq.haigaiapp.cn

Ruby: public / protected / private
来源：http://vv.panjiajie.cn

C#:   public / protected / private / internal
来源：http://qx.colortex.cn

[G11] getter / setter
来源：http://bn.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://iv.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pm.9csxet.cn

JS:   get name() { return this._name; }
来源：http://xf.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://mn.asd995.cn

Java: public String getName() { return name; }
来源：http://pu.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yk.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://lj.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ht.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://nc.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://sk.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rz.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://ey.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://wg.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://ze.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wf.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://kk.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://zi.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://ki.hnjuh.cn

Py:   isinstance(u, User)
来源：http://il.shxzukj.cn

PHP:  $u instanceof User
来源：http://uv.521024.cn

JS:   u instanceof User
来源：http://ls.hnjuh.cn

TS:   u instanceof User
来源：http://eb.hahajie.cn

Java: u instanceof User
来源：http://bo.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://td.nicolike.cn

Ruby: u.is_a?(User)
来源：http://oz.nicolike.cn

C#:   u is User
来源：http://aw.9csxet.cn

[G14] 数据类 / record
来源：http://tj.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wf.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://ds.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jx.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://ig.szsharing.cn

Java: record User(String name, int age) {}
来源：http://sm.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://tl.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xn.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://zj.colortex.cn

[G15] 枚举
来源：http://ix.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ll.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://km.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rx.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nt.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://ir.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xr.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://dh.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mx.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://br.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vq.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://ql.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://kp.9csxet.cn

TS:   Object.entries(obj)
来源：http://yd.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sc.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ku.lnxyls.cn

Ruby: obj.instance_variables
来源：http://sw.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://ll.huixinmuqiang.cn

================================================================================
来源：http://us.yuntaijiaju.cn

H. 异常与错误处理
来源：http://ef.jianghongdianzi.cn

================================================================================
来源：http://rn.hnjuh.cn

[H01] try / catch 基础
来源：http://ws.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tp.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jp.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lv.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xg.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zd.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vk.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gr.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fx.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://vb.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nc.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ru.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://az.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nq.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yz.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://me.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pk.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://af.szxytkj.cn

[H03] 主动抛出异常
来源：http://dc.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://vm.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bt.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://wn.521024.cn

TS:   throw new Error("错误信息");
来源：http://ik.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wd.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://us.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xn.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bv.521024.cn

[H04] 自定义异常类型
来源：http://ys.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://dq.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oj.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://zo.newstarts.cn

TS:   class MyError extends Error {}
来源：http://ug.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://ta.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pd.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://vc.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://ru.lnxyls.cn

[H05] 捕获特定类型
来源：http://xw.asd995.cn

Py:   except ValueError as e:
来源：http://kh.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iz.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ma.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://qb.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://zi.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pb.521024.cn

Ruby: rescue ArgumentError => e
来源：http://rj.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ja.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://ha.szsharing.cn

Py:   value = d.get("k") or default
来源：http://ez.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fa.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ed.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nm.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ld.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jx.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://vl.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://vt.panjiajie.cn

[H07] 断言
来源：http://fx.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://yo.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://iv.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://za.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://zs.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://ef.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pi.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ca.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://om.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ip.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://nm.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vs.nicolike.cn

JS:   e.message;  e.stack
来源：http://gm.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://de.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rz.lnxyls.cn

Go:   err.Error()
来源：http://cz.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://ae.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://le.521024.cn

[H09] 带错误码的异常
来源：http://xq.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ol.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xf.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xz.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vf.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lo.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jk.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ub.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://op.haigaiapp.cn

[H10] 资源自动释放
来源：http://ro.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gs.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dd.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ox.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ot.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vh.wgjwhj.cn

Go:   defer f.Close()
来源：http://vb.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ue.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jt.jctech888.com.cn

================================================================================
来源：http://bi.nszjky.cn

I. 正则表达式
来源：http://jr.gzmigu.cn

================================================================================
来源：http://jx.asd995.cn

[I01] 判断是否匹配
来源：http://sv.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ur.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qc.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://vt.521024.cn

TS:   /\d+/.test(s)
来源：http://vl.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ve.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cd.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://sf.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://me.hahajie.cn

[I02] 提取所有匹配
来源：http://ba.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://vp.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xo.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mw.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://yz.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://az.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pb.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://jp.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lk.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://nm.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wj.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mh.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fi.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ma.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oq.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qi.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ul.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qn.colortex.cn

[I04] 正则替换
来源：http://gb.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://os.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ou.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oz.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mh.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ua.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wp.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sr.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ac.szsharing.cn

[I05] 按正则拆分
来源：http://om.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wg.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ol.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://iu.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://ft.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://tg.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yw.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ag.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yr.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rb.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ja.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jj.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pt.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yt.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hk.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://an.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rv.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://by.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://ht.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ft.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hb.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fx.haigaiapp.cn

TS:   /error/gim
来源：http://ox.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ht.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uk.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://oe.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ma.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://qs.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lx.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ul.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uz.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fp.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yt.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qh.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ay.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fp.asd995.cn

================================================================================
来源：http://jh.shxzskj.cn

J. 日期与时间
来源：http://vj.newstarts.cn

================================================================================
来源：http://zi.muxihuayi.cn

[J01] 获取当前时间
来源：http://kp.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wl.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ut.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://ig.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://we.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tt.newstarts.cn

Go:   time.Now()
来源：http://zp.jctech888.com.cn

Ruby: Time.now
来源：http://km.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ws.bookmarksfly.cn

[J02] 格式化输出
来源：http://yd.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tg.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fo.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ns.jctech888.com.cn

TS:   d.toISOString()
来源：http://us.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://js.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hq.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zv.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tb.nicolike.cn

[J03] 字符串解析为日期
来源：http://sx.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ks.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bg.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://rd.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://uh.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yh.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zx.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://la.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bz.521024.cn

[J04] 时间戳与日期互转
来源：http://ue.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kk.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wa.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wp.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ah.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rz.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://no.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oj.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mr.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://nl.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://ba.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hg.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vj.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ek.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://yw.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gq.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://tz.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nh.shxzskj.cn

[J06] 计算两时间之差
来源：http://bw.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://gs.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://zz.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://po.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://on.chemitech.net.cn


<!-- 参考信息 -->