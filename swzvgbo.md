代发 wailian999

JS:   this.name = "x";
来源：http://ij.szxytkj.cn

TS:   name: string = "x";
来源：http://va.szsharing.cn

Java: private String name;
来源：http://dt.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yc.hnjuh.cn

Ruby: @name = "x"
来源：http://xq.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://bo.521024.cn

[G04] 定义方法
来源：http://ry.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://ci.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ty.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://ft.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://pj.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://xz.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oa.hahajie.cn

Ruby: def greet; @name; end
来源：http://pm.521024.cn

C#:   public string Greet() => Name;
来源：http://ur.9csxet.cn

[G05] 继承
来源：http://ft.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://io.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://kl.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://qm.nicolike.cn

TS:   class Admin extends User {}
来源：http://kr.gzmigu.cn

Java: class Admin extends User {}
来源：http://hh.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fu.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://rv.9csxet.cn

C#:   class Admin : User {}
来源：http://sy.9csxet.cn

[G06] 重写方法
来源：http://be.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://gk.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kd.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://sv.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://xy.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://jz.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ek.521024.cn

Ruby: def greet; "admin"; end
来源：http://ij.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ou.bjjhwx.cn

[G07] 调用父类方法
来源：http://kk.hahajie.cn

Py:   super().greet()
来源：http://bw.lnxyls.cn

PHP:  parent::greet();
来源：http://nd.newstarts.cn

JS:   super.greet();
来源：http://er.szxytkj.cn

TS:   super.greet();
来源：http://ie.newstarts.cn

Java: super.greet();
来源：http://aq.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zn.9csxet.cn

Ruby: super
来源：http://sa.yuexingan06.cn

C#:   base.Greet();
来源：http://fm.hahajie.cn

[G08] 静态方法与属性
来源：http://sz.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mi.nszjky.cn

PHP:  public static function f() {}
来源：http://bl.9csxet.cn

JS:   static f() {}
来源：http://vp.huixiangedu.cn

TS:   static f(): void {}
来源：http://ip.nicolike.cn

Java: static void f() {}
来源：http://tv.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://es.haigaiapp.cn

Ruby: def self.f; end
来源：http://bs.wgjwhj.cn

C#:   public static void F() {}
来源：http://gq.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://gz.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://ye.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ac.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zq.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://ly.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://bq.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://qf.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ct.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://pr.muxihuayi.cn

[G10] 访问控制
来源：http://bk.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://iz.521024.cn

PHP:  public / protected / private
来源：http://ni.huanxung.cn

JS:   #private 字段；其余公开
来源：http://nh.jctech888.com.cn

TS:   public / protected / private
来源：http://ls.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://bp.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nk.huixiangedu.cn

Ruby: public / protected / private
来源：http://qm.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://sg.asd995.cn

[G11] getter / setter
来源：http://zl.hahajie.cn

Py:   @property 与 @x.setter
来源：http://sz.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wz.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://xe.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://eu.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://bs.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xq.colortex.cn

Ruby: attr_accessor :name
来源：http://mu.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://wa.asd995.cn

[G12] 对象转字符串
来源：http://jx.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://xe.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mp.asd995.cn

JS:   toString() { return this.name; }
来源：http://so.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://kh.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://jg.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hj.asd995.cn

Ruby: def to_s; @name; end
来源：http://xv.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://oi.colortex.cn

[G13] 判断对象类型
来源：http://hc.521024.cn

Py:   isinstance(u, User)
来源：http://nh.hahajie.cn

PHP:  $u instanceof User
来源：http://tz.jianghongdianzi.cn

JS:   u instanceof User
来源：http://vc.bookmarksfly.cn

TS:   u instanceof User
来源：http://ys.nszjky.cn

Java: u instanceof User
来源：http://xy.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://py.szsharing.cn

Ruby: u.is_a?(User)
来源：http://ki.hnjuh.cn

C#:   u is User
来源：http://fh.panjiajie.cn

[G14] 数据类 / record
来源：http://sc.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cj.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://hq.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ub.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://xg.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://vl.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://wu.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ve.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://bi.jianghongdianzi.cn

[G15] 枚举
来源：http://tu.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qy.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://te.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mr.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://if.521024.cn

Java: enum Color { RED, GREEN }
来源：http://op.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ss.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://hd.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zj.521024.cn

[G16] 对象转数组 / 字典
来源：http://au.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iz.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://xt.panjiajie.cn

JS:   Object.entries(obj)
来源：http://gy.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://og.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nx.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nh.9csxet.cn

Ruby: obj.instance_variables
来源：http://he.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://lz.bjjhwx.cn

================================================================================
来源：http://nx.gzmigu.cn

H. 异常与错误处理
来源：http://il.bjjhwx.cn

================================================================================
来源：http://al.panjiajie.cn

[H01] try / catch 基础
来源：http://wi.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tx.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gt.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oa.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cc.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tp.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uk.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uh.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ii.nicolike.cn

[H02] finally / ensure 收尾
来源：http://lt.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ux.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ci.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ol.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mp.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vb.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rl.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://py.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ai.nszjky.cn

[H03] 主动抛出异常
来源：http://eo.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://qc.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cg.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://tj.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://xz.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vx.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pf.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ki.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dj.newstarts.cn

[H04] 自定义异常类型
来源：http://er.521024.cn

Py:   class MyError(Exception): pass
来源：http://fx.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ca.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://cv.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://ae.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://sq.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lt.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://nu.nszjky.cn

C#:   class MyException : Exception {}
来源：http://au.wgjwhj.cn

[H05] 捕获特定类型
来源：http://kx.shxzskj.cn

Py:   except ValueError as e:
来源：http://tk.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://is.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://bx.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://nt.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://yr.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xa.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://dy.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uc.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://gf.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://yt.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://oo.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hr.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vl.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wy.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ki.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://gn.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://zv.521024.cn

[H07] 断言
来源：http://ic.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://dd.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://fe.521024.cn

JS:   console.assert(x > 0);
来源：http://jb.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://sl.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://jp.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bv.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ls.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://af.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://fr.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://ia.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://he.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://vs.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://co.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cq.colortex.cn

Go:   err.Error()
来源：http://hi.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://gb.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://db.colortex.cn

[H09] 带错误码的异常
来源：http://jz.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mv.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tg.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hn.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ba.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hx.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gz.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mk.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ek.yuexingan06.cn

[H10] 资源自动释放
来源：http://tm.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://up.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rq.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jq.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fs.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://le.521024.cn

Go:   defer f.Close()
来源：http://iu.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://et.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ko.gzmigu.cn

================================================================================
来源：http://zo.szsharing.cn

I. 正则表达式
来源：http://yk.muxihuayi.cn

================================================================================
来源：http://sy.521024.cn

[I01] 判断是否匹配
来源：http://kr.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bl.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://su.colortex.cn

JS:   /\d+/.test(s)
来源：http://tq.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://hl.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ha.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ze.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://if.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nf.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://td.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://sc.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yp.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cm.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://zc.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://up.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gj.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://je.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rt.lnxyls.cn

[I03] 提取捕获分组
来源：http://bh.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jb.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bh.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kv.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wm.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://la.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qz.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yh.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pp.huixiangedu.cn

[I04] 正则替换
来源：http://kn.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mc.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://im.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dm.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uf.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qk.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ju.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ib.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mw.panjiajie.cn

[I05] 按正则拆分
来源：http://jo.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://az.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bw.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://rl.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://rl.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://as.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kh.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ky.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fx.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cc.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lz.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ec.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wt.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fd.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jp.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nf.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wp.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rp.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://gl.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yy.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ps.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ya.nszjky.cn

TS:   /error/gim
来源：http://vw.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oh.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cv.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://hc.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xh.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://cs.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yp.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sq.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://su.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cf.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ob.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jn.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://al.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mu.wgjwhj.cn

================================================================================
来源：http://ky.panjiajie.cn

J. 日期与时间
来源：http://hx.newstarts.cn

================================================================================
来源：http://ry.huixiangedu.cn

[J01] 获取当前时间
来源：http://ll.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zl.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xy.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://jn.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://di.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ij.szxytkj.cn


<!-- 参考信息 -->