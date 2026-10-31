代发 wailian999

Java: class Admin extends User {}
来源：http://yy.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xt.lnxyls.cn

Ruby: class Admin < User; end
来源：http://di.shtwfgs.cn

C#:   class Admin : User {}
来源：http://bs.jctech888.com.cn

[G06] 重写方法
来源：http://zd.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://gt.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pm.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://fh.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://rt.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://dw.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kh.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://ny.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://bd.chemitech.net.cn

[G07] 调用父类方法
来源：http://es.bjjhwx.cn

Py:   super().greet()
来源：http://au.nicolike.cn

PHP:  parent::greet();
来源：http://la.haigaiapp.cn

JS:   super.greet();
来源：http://lr.hahajie.cn

TS:   super.greet();
来源：http://ih.wgjwhj.cn

Java: super.greet();
来源：http://ue.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xb.shtwfgs.cn

Ruby: super
来源：http://tr.shxzskj.cn

C#:   base.Greet();
来源：http://mt.shxzukj.cn

[G08] 静态方法与属性
来源：http://db.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qb.muxihuayi.cn

PHP:  public static function f() {}
来源：http://fp.9csxet.cn

JS:   static f() {}
来源：http://ao.jctech888.com.cn

TS:   static f(): void {}
来源：http://cp.bjjhwx.cn

Java: static void f() {}
来源：http://xz.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pw.wgjwhj.cn

Ruby: def self.f; end
来源：http://hy.shxzukj.cn

C#:   public static void F() {}
来源：http://aq.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://gq.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://do.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ga.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zj.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://vl.nszjky.cn

Java: interface Shape { double area(); }
来源：http://yz.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://lu.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pc.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://aq.hahajie.cn

[G10] 访问控制
来源：http://yb.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://kw.wgjwhj.cn

PHP:  public / protected / private
来源：http://dp.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://hm.shxzskj.cn

TS:   public / protected / private
来源：http://ri.asd995.cn

Java: public / protected / private / 默认包级
来源：http://ep.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hq.nicolike.cn

Ruby: public / protected / private
来源：http://yu.hnjuh.cn

C#:   public / protected / private / internal
来源：http://tz.szxytkj.cn

[G11] getter / setter
来源：http://ne.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://rh.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://it.asd995.cn

JS:   get name() { return this._name; }
来源：http://sl.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://gq.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://mc.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ax.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://de.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://jz.nicolike.cn

[G12] 对象转字符串
来源：http://si.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://aa.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qn.nszjky.cn

JS:   toString() { return this.name; }
来源：http://hc.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://kr.521024.cn

Java: @Override public String toString() { return name; }
来源：http://ux.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cr.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://qn.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://wc.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://pu.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://iq.chemitech.net.cn

PHP:  $u instanceof User
来源：http://bm.yuexingan06.cn

JS:   u instanceof User
来源：http://ti.wgjwhj.cn

TS:   u instanceof User
来源：http://jy.huixiangedu.cn

Java: u instanceof User
来源：http://ib.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dd.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://dh.jctech888.com.cn

C#:   u is User
来源：http://nh.chemitech.net.cn

[G14] 数据类 / record
来源：http://tr.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uj.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://ni.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vx.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://ud.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://vn.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://vo.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oc.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://en.jianghongdianzi.cn

[G15] 枚举
来源：http://te.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://as.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mu.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wv.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fg.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://ha.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qj.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://pj.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ar.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://oi.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zv.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://uc.asd995.cn

JS:   Object.entries(obj)
来源：http://ca.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://nq.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oq.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ql.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://it.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://cg.9csxet.cn

================================================================================
来源：http://rw.panjiajie.cn

H. 异常与错误处理
来源：http://dv.521024.cn

================================================================================
来源：http://si.panjiajie.cn

[H01] try / catch 基础
来源：http://in.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yc.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tm.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bv.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wu.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ld.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zj.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yh.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rg.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://vf.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ei.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wi.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rs.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pv.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lx.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ka.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gb.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jp.asd995.cn

[H03] 主动抛出异常
来源：http://zr.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://hr.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hh.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://tu.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://tv.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rj.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lo.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zb.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wx.lnxyls.cn

[H04] 自定义异常类型
来源：http://pi.521024.cn

Py:   class MyError(Exception): pass
来源：http://yo.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gt.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://al.hahajie.cn

TS:   class MyError extends Error {}
来源：http://ac.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://ds.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rw.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ra.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://nj.szxytkj.cn

[H05] 捕获特定类型
来源：http://vp.chemitech.net.cn

Py:   except ValueError as e:
来源：http://pb.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ts.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://fs.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://ma.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://xo.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://es.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://os.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kn.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://ir.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://ax.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lg.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dl.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ru.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ui.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mw.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://rk.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://xr.lnxyls.cn

[H07] 断言
来源：http://ww.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://bh.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://nc.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://fd.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://ro.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://mh.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wj.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hl.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://oz.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://uc.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://su.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iv.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://us.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dt.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fp.nszjky.cn

Go:   err.Error()
来源：http://oj.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://um.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://ip.nszjky.cn

[H09] 带错误码的异常
来源：http://vh.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hb.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bq.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ie.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tj.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uv.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lg.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wg.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fq.lnxyls.cn

[H10] 资源自动释放
来源：http://ln.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qp.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sc.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://in.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kg.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xb.lnxyls.cn

Go:   defer f.Close()
来源：http://al.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ja.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ew.jianghongdianzi.cn

================================================================================
来源：http://kx.colortex.cn

I. 正则表达式
来源：http://du.chemitech.net.cn

================================================================================
来源：http://is.muxihuayi.cn

[I01] 判断是否匹配
来源：http://gk.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hb.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ow.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://dg.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://ba.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jn.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ba.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://be.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gm.gzmigu.cn

[I02] 提取所有匹配
来源：http://yf.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://kc.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://im.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mg.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://ir.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fw.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yk.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://sh.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bj.shtwfgs.cn

[I03] 提取捕获分组
来源：http://sm.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kh.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nw.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oz.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rg.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gr.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://um.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vo.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://km.9csxet.cn

[I04] 正则替换
来源：http://ym.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://to.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mm.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pm.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tb.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cc.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lb.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yf.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mc.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://vk.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xy.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sd.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://nh.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://lj.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://ri.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dl.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wu.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oa.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mj.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://al.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xr.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fl.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zb.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dk.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gi.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nq.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jo.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://vg.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ao.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nq.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ys.colortex.cn

TS:   /error/gim
来源：http://ht.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://se.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fb.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://oz.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ys.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://yr.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wq.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gu.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ra.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yg.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eg.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mh.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ko.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xy.shtwfgs.cn

================================================================================
来源：http://sk.jctech888.com.cn

J. 日期与时间
来源：http://cg.bookmarksfly.cn

================================================================================
来源：http://bv.gzmigu.cn

[J01] 获取当前时间
来源：http://jr.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wl.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ao.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://yz.nicolike.cn

TS:   new Date();  Date.now()
来源：http://zv.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wk.asd995.cn

Go:   time.Now()
来源：http://wq.colortex.cn

Ruby: Time.now
来源：http://ws.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xi.asd995.cn

[J02] 格式化输出
来源：http://yp.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wa.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jb.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lb.wgjwhj.cn

TS:   d.toISOString()
来源：http://et.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xp.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uo.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://an.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gf.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://sk.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gs.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vd.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://vg.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://bj.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pq.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xa.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://ft.newstarts.cn


<!-- 参考信息 -->