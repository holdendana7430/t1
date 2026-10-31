代发 wailian999

JS:   this.name = "x";
来源：http://kf.nszjky.cn

TS:   name: string = "x";
来源：http://ys.huanxung.cn

Java: private String name;
来源：http://rj.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://do.shtwfgs.cn

Ruby: @name = "x"
来源：http://bt.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://cp.nicolike.cn

[G04] 定义方法
来源：http://on.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://fe.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wg.huanxung.cn

JS:   greet() { return this.name; }
来源：http://ol.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://fn.muxihuayi.cn

Java: String greet() { return name; }
来源：http://ef.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://do.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://wx.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://gp.9csxet.cn

[G05] 继承
来源：http://uf.shxzukj.cn

Py:   class Admin(User): pass
来源：http://lj.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://by.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://bn.nicolike.cn

TS:   class Admin extends User {}
来源：http://rw.yuexingan06.cn

Java: class Admin extends User {}
来源：http://cb.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kp.lnxyls.cn

Ruby: class Admin < User; end
来源：http://sk.muxihuayi.cn

C#:   class Admin : User {}
来源：http://zn.colortex.cn

[G06] 重写方法
来源：http://au.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://ws.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eh.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://qt.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://dp.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://mm.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ds.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://me.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://yl.panjiajie.cn

[G07] 调用父类方法
来源：http://cz.huixinmuqiang.cn

Py:   super().greet()
来源：http://tk.asd995.cn

PHP:  parent::greet();
来源：http://qb.bookmarksfly.cn

JS:   super.greet();
来源：http://qh.yuexingan06.cn

TS:   super.greet();
来源：http://da.hnjuh.cn

Java: super.greet();
来源：http://tp.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ob.wgjwhj.cn

Ruby: super
来源：http://cb.huixinmuqiang.cn

C#:   base.Greet();
来源：http://gd.bjjhwx.cn

[G08] 静态方法与属性
来源：http://yc.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vd.wgjwhj.cn

PHP:  public static function f() {}
来源：http://pv.521024.cn

JS:   static f() {}
来源：http://ld.bjjhwx.cn

TS:   static f(): void {}
来源：http://pm.panjiajie.cn

Java: static void f() {}
来源：http://tg.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qe.yuexingan06.cn

Ruby: def self.f; end
来源：http://sw.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://ty.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://ki.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://st.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kt.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bk.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://jp.hahajie.cn

Java: interface Shape { double area(); }
来源：http://ha.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://ew.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ml.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://er.lnxyls.cn

[G10] 访问控制
来源：http://ov.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://bq.muxihuayi.cn

PHP:  public / protected / private
来源：http://du.hahajie.cn

JS:   #private 字段；其余公开
来源：http://ja.hnjuh.cn

TS:   public / protected / private
来源：http://st.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://ro.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pt.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://bx.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://gd.9csxet.cn

[G11] getter / setter
来源：http://mk.9csxet.cn

Py:   @property 与 @x.setter
来源：http://py.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oz.nicolike.cn

JS:   get name() { return this._name; }
来源：http://wt.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://he.hnjuh.cn

Java: public String getName() { return name; }
来源：http://id.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cl.9csxet.cn

Ruby: attr_accessor :name
来源：http://yf.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://if.muxihuayi.cn

[G12] 对象转字符串
来源：http://op.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://xd.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jf.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://zt.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://id.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://ld.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ce.hahajie.cn

Ruby: def to_s; @name; end
来源：http://dy.colortex.cn

C#:   public override string ToString() => Name;
来源：http://fm.jctech888.com.cn

[G13] 判断对象类型
来源：http://ve.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://hf.9csxet.cn

PHP:  $u instanceof User
来源：http://kq.shxzukj.cn

JS:   u instanceof User
来源：http://dk.shxzskj.cn

TS:   u instanceof User
来源：http://lx.huixiangedu.cn

Java: u instanceof User
来源：http://ht.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bi.hahajie.cn

Ruby: u.is_a?(User)
来源：http://zm.asd995.cn

C#:   u is User
来源：http://lb.shxzskj.cn

[G14] 数据类 / record
来源：http://dv.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lc.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://qj.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ny.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://pm.521024.cn

Java: record User(String name, int age) {}
来源：http://sr.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://ev.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pp.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://jh.wgjwhj.cn

[G15] 枚举
来源：http://ln.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wb.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ro.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zj.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qy.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://qd.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gj.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://hv.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lk.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://vw.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cs.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://ty.newstarts.cn

JS:   Object.entries(obj)
来源：http://gv.huanxung.cn

TS:   Object.entries(obj)
来源：http://ti.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ai.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bv.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://ad.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://lg.shxzskj.cn

================================================================================
来源：http://zp.huanxung.cn

H. 异常与错误处理
来源：http://gm.gzmigu.cn

================================================================================
来源：http://hd.nszjky.cn

[H01] try / catch 基础
来源：http://vu.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qu.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fk.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sv.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ev.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://do.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rk.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mk.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kq.nicolike.cn

[H02] finally / ensure 收尾
来源：http://od.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hm.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ne.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qd.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oo.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wo.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bd.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://av.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ux.9csxet.cn

[H03] 主动抛出异常
来源：http://wr.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://vl.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nm.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://se.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://cc.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qe.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jx.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zk.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wb.huixiangedu.cn

[H04] 自定义异常类型
来源：http://tk.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://jz.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yx.newstarts.cn

JS:   class MyError extends Error {}
来源：http://hq.colortex.cn

TS:   class MyError extends Error {}
来源：http://yy.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://mj.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ig.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://xp.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://da.521024.cn

[H05] 捕获特定类型
来源：http://gv.jctech888.com.cn

Py:   except ValueError as e:
来源：http://fv.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nn.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://ox.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://wi.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://of.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pv.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://sy.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bw.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://nk.nszjky.cn

Py:   value = d.get("k") or default
来源：http://bk.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pn.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uo.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gu.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://he.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://os.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://gz.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://pp.9csxet.cn

[H07] 断言
来源：http://eh.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://bj.szxytkj.cn

PHP:  assert($x > 0);
来源：http://ck.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://ze.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://ry.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://oo.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rq.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rt.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://in.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://ij.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://sx.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nk.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://co.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gc.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dr.lnxyls.cn

Go:   err.Error()
来源：http://mt.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://xl.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://dc.9csxet.cn

[H09] 带错误码的异常
来源：http://np.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tu.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zd.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ed.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gd.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ba.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://as.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fa.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yz.lnxyls.cn

[H10] 资源自动释放
来源：http://me.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fg.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zd.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oa.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ug.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kt.hnjuh.cn

Go:   defer f.Close()
来源：http://yh.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vn.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zc.chemitech.net.cn

================================================================================
来源：http://ey.muxihuayi.cn

I. 正则表达式
来源：http://gm.lnxyls.cn

================================================================================
来源：http://uo.wgjwhj.cn

[I01] 判断是否匹配
来源：http://mf.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dd.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pa.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://uu.nicolike.cn

TS:   /\d+/.test(s)
来源：http://ly.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ql.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sx.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://tl.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sv.asd995.cn

[I02] 提取所有匹配
来源：http://lv.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://no.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ls.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bj.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://zb.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zr.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jn.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://jc.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nv.gzmigu.cn

[I03] 提取捕获分组
来源：http://qz.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pu.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ue.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ds.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ll.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rp.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wr.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hn.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bd.hnjuh.cn

[I04] 正则替换
来源：http://mh.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jl.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wz.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bq.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://il.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dw.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qm.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tn.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pa.shxzskj.cn

[I05] 按正则拆分
来源：http://eo.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qf.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xs.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ll.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://cz.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://qy.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bm.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vv.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uc.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rz.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vm.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bn.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qd.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vx.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wz.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rx.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://st.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ho.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://gg.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://et.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qr.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fa.huanxung.cn

TS:   /error/gim
来源：http://tt.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lh.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://om.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://el.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://et.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://to.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sf.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ai.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gr.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lf.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://re.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gf.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ws.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wa.hnjuh.cn

================================================================================
来源：http://jx.521024.cn

J. 日期与时间
来源：http://dr.asd995.cn

================================================================================
来源：http://vx.bjjhwx.cn

[J01] 获取当前时间
来源：http://gd.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vu.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gb.521024.cn

JS:   new Date();  Date.now()
来源：http://nu.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://xs.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rj.muxihuayi.cn


<!-- 参考信息 -->