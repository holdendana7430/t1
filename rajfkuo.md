代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://if.hnjuh.cn

Ruby: def greet; @name; end
来源：http://bm.521024.cn

C#:   public string Greet() => Name;
来源：http://kk.521024.cn

[G05] 继承
来源：http://ax.newstarts.cn

Py:   class Admin(User): pass
来源：http://ew.hahajie.cn

PHP:  class Admin extends User {}
来源：http://ys.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://su.nicolike.cn

TS:   class Admin extends User {}
来源：http://gv.huanxung.cn

Java: class Admin extends User {}
来源：http://lv.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://je.newstarts.cn

Ruby: class Admin < User; end
来源：http://oo.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://td.shtwfgs.cn

[G06] 重写方法
来源：http://sp.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://bw.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iv.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://ae.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://rq.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://sr.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yq.colortex.cn

Ruby: def greet; "admin"; end
来源：http://zb.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://py.shtwfgs.cn

[G07] 调用父类方法
来源：http://ex.nicolike.cn

Py:   super().greet()
来源：http://hn.521024.cn

PHP:  parent::greet();
来源：http://we.jctech888.com.cn

JS:   super.greet();
来源：http://fp.chemitech.net.cn

TS:   super.greet();
来源：http://pm.nszjky.cn

Java: super.greet();
来源：http://jw.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oc.yuntaijiaju.cn

Ruby: super
来源：http://zz.newstarts.cn

C#:   base.Greet();
来源：http://kb.szsharing.cn

[G08] 静态方法与属性
来源：http://yf.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nm.hahajie.cn

PHP:  public static function f() {}
来源：http://on.haigaiapp.cn

JS:   static f() {}
来源：http://ig.9csxet.cn

TS:   static f(): void {}
来源：http://hs.colortex.cn

Java: static void f() {}
来源：http://zx.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qg.haigaiapp.cn

Ruby: def self.f; end
来源：http://bf.gzmigu.cn

C#:   public static void F() {}
来源：http://bu.nicolike.cn

[G09] 接口 / 抽象类
来源：http://mh.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://ql.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gb.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ln.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://aj.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://dd.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://ny.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ue.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://zq.shxzukj.cn

[G10] 访问控制
来源：http://rl.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://ig.bookmarksfly.cn

PHP:  public / protected / private
来源：http://vx.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://zs.bookmarksfly.cn

TS:   public / protected / private
来源：http://xm.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://jq.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mf.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://sh.asd995.cn

C#:   public / protected / private / internal
来源：http://zj.szxytkj.cn

[G11] getter / setter
来源：http://oq.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://wf.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ts.colortex.cn

JS:   get name() { return this._name; }
来源：http://oz.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://dh.panjiajie.cn

Java: public String getName() { return name; }
来源：http://tq.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wc.huanxung.cn

Ruby: attr_accessor :name
来源：http://pj.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://wu.bjjhwx.cn

[G12] 对象转字符串
来源：http://ny.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://df.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cm.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://hy.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://dt.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://oo.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ny.szsharing.cn

Ruby: def to_s; @name; end
来源：http://qq.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://iv.lnxyls.cn

[G13] 判断对象类型
来源：http://cn.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://jl.asd995.cn

PHP:  $u instanceof User
来源：http://au.shtwfgs.cn

JS:   u instanceof User
来源：http://lb.hnjuh.cn

TS:   u instanceof User
来源：http://hm.huixinmuqiang.cn

Java: u instanceof User
来源：http://wo.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yj.nicolike.cn

Ruby: u.is_a?(User)
来源：http://dr.bookmarksfly.cn

C#:   u is User
来源：http://il.hahajie.cn

[G14] 数据类 / record
来源：http://op.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wc.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://hu.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cx.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://fs.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://po.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://je.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tj.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://rs.huixinmuqiang.cn

[G15] 枚举
来源：http://fa.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tr.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bo.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oz.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cj.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://vb.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sr.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://nh.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sl.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://sx.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ct.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://oc.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://vp.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://nq.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pj.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oi.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://cx.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://ds.hnjuh.cn

================================================================================
来源：http://wi.huanxung.cn

H. 异常与错误处理
来源：http://hl.muxihuayi.cn

================================================================================
来源：http://jf.jctech888.com.cn

[H01] try / catch 基础
来源：http://xh.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://go.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ub.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ho.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://np.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kx.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nk.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zs.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://up.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://fd.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bg.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ni.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fj.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xg.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://et.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uf.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ei.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://me.haigaiapp.cn

[H03] 主动抛出异常
来源：http://qp.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://vv.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nf.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://xk.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://xu.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tz.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tq.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lz.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qr.newstarts.cn

[H04] 自定义异常类型
来源：http://kg.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://ku.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kq.nicolike.cn

JS:   class MyError extends Error {}
来源：http://qw.colortex.cn

TS:   class MyError extends Error {}
来源：http://iq.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://jm.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bk.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://qv.521024.cn

C#:   class MyException : Exception {}
来源：http://op.huanxung.cn

[H05] 捕获特定类型
来源：http://ba.jctech888.com.cn

Py:   except ValueError as e:
来源：http://hs.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xg.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://jz.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://ub.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://jv.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dg.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://ie.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://my.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://kn.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://ti.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qq.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gs.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cs.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://em.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rq.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://sn.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://tp.shxzskj.cn

[H07] 断言
来源：http://bq.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://ww.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://zm.szsharing.cn

JS:   console.assert(x > 0);
来源：http://nw.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://wd.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://nu.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tp.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ez.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://rs.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://cu.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://lp.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mi.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://rt.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lq.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://av.asd995.cn

Go:   err.Error()
来源：http://wb.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://xv.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://ao.shtwfgs.cn

[H09] 带错误码的异常
来源：http://uq.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://do.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ov.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oa.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://re.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gs.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://td.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jr.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zn.colortex.cn

[H10] 资源自动释放
来源：http://dc.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ng.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ya.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wd.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ca.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xt.shtwfgs.cn

Go:   defer f.Close()
来源：http://cg.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mu.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vb.yuntaijiaju.cn

================================================================================
来源：http://dj.jctech888.com.cn

I. 正则表达式
来源：http://cq.asd995.cn

================================================================================
来源：http://qc.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://aj.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ei.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dj.hahajie.cn

JS:   /\d+/.test(s)
来源：http://tn.huanxung.cn

TS:   /\d+/.test(s)
来源：http://ml.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://na.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hg.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://mx.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ak.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://pq.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://mo.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bw.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://co.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://kn.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ve.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vc.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://qe.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vy.jctech888.com.cn

[I03] 提取捕获分组
来源：http://kx.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qy.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mm.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lf.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sh.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://to.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fs.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cc.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://td.chemitech.net.cn

[I04] 正则替换
来源：http://xb.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ue.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://da.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vy.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nq.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mk.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xc.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ds.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lk.hnjuh.cn

[I05] 按正则拆分
来源：http://ra.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pb.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://su.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://ib.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://xl.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://to.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gf.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xj.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yg.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ai.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fc.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gb.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://io.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kw.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ky.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gr.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gu.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://td.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://ei.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ec.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uk.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hm.asd995.cn

TS:   /error/gim
来源：http://ro.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://li.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ok.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://kh.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aj.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://vv.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://in.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hh.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jv.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wy.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bp.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vg.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wq.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pe.yuntaijiaju.cn

================================================================================
来源：http://pw.wgjwhj.cn

J. 日期与时间
来源：http://ti.521024.cn

================================================================================
来源：http://if.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://jw.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ku.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://el.521024.cn

JS:   new Date();  Date.now()
来源：http://yx.nszjky.cn

TS:   new Date();  Date.now()
来源：http://iv.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mc.shxzukj.cn

Go:   time.Now()
来源：http://ol.szxytkj.cn

Ruby: Time.now
来源：http://ew.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dd.521024.cn

[J02] 格式化输出
来源：http://il.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sd.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lz.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yk.shtwfgs.cn

TS:   d.toISOString()
来源：http://jk.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sm.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jf.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zl.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uy.asd995.cn


<!-- 参考信息 -->