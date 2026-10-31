代发 wailian999

JS:   this.name = "x";
来源：http://mo.haigaiapp.cn

TS:   name: string = "x";
来源：http://oz.nicolike.cn

Java: private String name;
来源：http://gd.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cp.panjiajie.cn

Ruby: @name = "x"
来源：http://lz.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://qh.panjiajie.cn

[G04] 定义方法
来源：http://xd.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://bm.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ia.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://hf.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://yz.bjjhwx.cn

Java: String greet() { return name; }
来源：http://dt.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gu.szsharing.cn

Ruby: def greet; @name; end
来源：http://mb.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://is.gzmigu.cn

[G05] 继承
来源：http://dl.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://bp.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://vm.newstarts.cn

JS:   class Admin extends User {}
来源：http://bx.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://ao.bjjhwx.cn

Java: class Admin extends User {}
来源：http://vk.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mb.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://ni.panjiajie.cn

C#:   class Admin : User {}
来源：http://fg.shxzukj.cn

[G06] 重写方法
来源：http://wc.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://mh.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zp.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://rw.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://ta.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://vj.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qg.521024.cn

Ruby: def greet; "admin"; end
来源：http://cu.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://ae.bjjhwx.cn

[G07] 调用父类方法
来源：http://pv.asd995.cn

Py:   super().greet()
来源：http://jb.hnjuh.cn

PHP:  parent::greet();
来源：http://by.szsharing.cn

JS:   super.greet();
来源：http://ys.yuntaijiaju.cn

TS:   super.greet();
来源：http://bl.bjjhwx.cn

Java: super.greet();
来源：http://iw.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bf.yuexingan06.cn

Ruby: super
来源：http://vb.shxzukj.cn

C#:   base.Greet();
来源：http://nm.nicolike.cn

[G08] 静态方法与属性
来源：http://qv.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gr.panjiajie.cn

PHP:  public static function f() {}
来源：http://dp.shtwfgs.cn

JS:   static f() {}
来源：http://ua.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://cp.muxihuayi.cn

Java: static void f() {}
来源：http://fy.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rf.haigaiapp.cn

Ruby: def self.f; end
来源：http://ej.lnxyls.cn

C#:   public static void F() {}
来源：http://nz.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://iz.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://jd.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cl.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ow.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://ra.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://hb.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://cu.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wl.521024.cn

C#:   interface IShape { double Area(); }
来源：http://vq.muxihuayi.cn

[G10] 访问控制
来源：http://gs.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://hj.szxytkj.cn

PHP:  public / protected / private
来源：http://db.asd995.cn

JS:   #private 字段；其余公开
来源：http://hs.shtwfgs.cn

TS:   public / protected / private
来源：http://pt.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://os.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://od.nicolike.cn

Ruby: public / protected / private
来源：http://jd.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://ej.hnjuh.cn

[G11] getter / setter
来源：http://ig.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://dv.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jb.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://ll.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://dd.nszjky.cn

Java: public String getName() { return name; }
来源：http://rb.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://md.newstarts.cn

Ruby: attr_accessor :name
来源：http://sm.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://sz.szsharing.cn

[G12] 对象转字符串
来源：http://tx.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://bp.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fq.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://gh.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://hk.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://et.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ou.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://kz.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://xb.shtwfgs.cn

[G13] 判断对象类型
来源：http://zu.521024.cn

Py:   isinstance(u, User)
来源：http://ph.shtwfgs.cn

PHP:  $u instanceof User
来源：http://gu.yuexingan06.cn

JS:   u instanceof User
来源：http://rm.szsharing.cn

TS:   u instanceof User
来源：http://cv.newstarts.cn

Java: u instanceof User
来源：http://ho.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rs.nicolike.cn

Ruby: u.is_a?(User)
来源：http://hb.newstarts.cn

C#:   u is User
来源：http://ny.huixiangedu.cn

[G14] 数据类 / record
来源：http://pq.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rv.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://ku.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ni.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://xr.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://dp.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://bo.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://um.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://ew.huanxung.cn

[G15] 枚举
来源：http://ry.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oe.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gw.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ru.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xo.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://cr.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iy.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://an.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nx.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://rq.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jy.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://wv.nszjky.cn

JS:   Object.entries(obj)
来源：http://fv.nszjky.cn

TS:   Object.entries(obj)
来源：http://uu.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ih.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tx.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://qv.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://xh.bjjhwx.cn

================================================================================
来源：http://fs.newstarts.cn

H. 异常与错误处理
来源：http://jb.jctech888.com.cn

================================================================================
来源：http://lc.bjjhwx.cn

[H01] try / catch 基础
来源：http://re.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sr.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vk.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xj.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mp.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qx.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://me.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qm.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sx.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://rw.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pr.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yy.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hc.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yl.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hm.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ty.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qp.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kx.lnxyls.cn

[H03] 主动抛出异常
来源：http://ho.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://pi.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hk.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://rx.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://ns.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oj.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ta.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nr.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pq.hahajie.cn

[H04] 自定义异常类型
来源：http://uz.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://lb.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ro.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://ui.9csxet.cn

TS:   class MyError extends Error {}
来源：http://pg.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://wm.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zp.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://uq.9csxet.cn

C#:   class MyException : Exception {}
来源：http://vm.asd995.cn

[H05] 捕获特定类型
来源：http://kz.shtwfgs.cn

Py:   except ValueError as e:
来源：http://ef.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ry.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://gj.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://ta.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://wk.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qb.521024.cn

Ruby: rescue ArgumentError => e
来源：http://rg.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://js.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://hr.asd995.cn

Py:   value = d.get("k") or default
来源：http://hg.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wq.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rc.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rd.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://af.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ii.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://ex.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://bw.9csxet.cn

[H07] 断言
来源：http://zm.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://at.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://fo.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://jc.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://lt.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://mo.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nx.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uc.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ef.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://ch.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://pr.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bx.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://nu.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oo.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nd.huixiangedu.cn

Go:   err.Error()
来源：http://wf.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://wk.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://oy.wgjwhj.cn

[H09] 带错误码的异常
来源：http://kl.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://il.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fd.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rq.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://db.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wx.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bi.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hv.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rq.haigaiapp.cn

[H10] 资源自动释放
来源：http://wd.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fd.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://re.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://he.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kk.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ec.gzmigu.cn

Go:   defer f.Close()
来源：http://ot.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jg.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zy.yuntaijiaju.cn

================================================================================
来源：http://lt.panjiajie.cn

I. 正则表达式
来源：http://bq.nszjky.cn

================================================================================
来源：http://zy.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://ih.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gz.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vd.newstarts.cn

JS:   /\d+/.test(s)
来源：http://pv.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://qi.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kn.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iz.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://pi.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gu.muxihuayi.cn

[I02] 提取所有匹配
来源：http://fu.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://qy.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yq.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zb.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://xh.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dj.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fb.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://qw.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ul.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://ky.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://st.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kt.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yv.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qr.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tz.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vu.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yo.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fr.szsharing.cn

[I04] 正则替换
来源：http://il.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cf.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dd.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ut.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ff.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gk.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ty.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pn.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xa.9csxet.cn

[I05] 按正则拆分
来源：http://sp.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uf.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://md.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://pl.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://lt.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://ia.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ju.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zc.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xq.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hf.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ns.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://or.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://od.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mc.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kv.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nu.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ne.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ws.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://ty.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wh.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kq.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kd.jianghongdianzi.cn

TS:   /error/gim
来源：http://wk.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gt.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zg.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://uj.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ae.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://uv.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ml.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://in.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zv.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zg.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pd.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://du.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://az.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fj.9csxet.cn

================================================================================
来源：http://be.bookmarksfly.cn

J. 日期与时间
来源：http://zg.jianghongdianzi.cn

================================================================================
来源：http://cx.521024.cn

[J01] 获取当前时间
来源：http://mw.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cz.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fw.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://uq.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://sk.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wl.jctech888.com.cn


<!-- 参考信息 -->