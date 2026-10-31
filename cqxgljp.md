代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://tu.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://qv.521024.cn

TS:   greet(): string { return this.name; }
来源：http://dx.jctech888.com.cn

Java: String greet() { return name; }
来源：http://cv.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jd.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://mh.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://pw.huixiangedu.cn

[G05] 继承
来源：http://jh.szsharing.cn

Py:   class Admin(User): pass
来源：http://fq.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://lh.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://au.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://ub.shtwfgs.cn

Java: class Admin extends User {}
来源：http://lc.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uv.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://zs.521024.cn

C#:   class Admin : User {}
来源：http://cb.yuexingan06.cn

[G06] 重写方法
来源：http://ny.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://be.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bj.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://yz.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://co.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://oy.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hl.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://mg.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://xu.colortex.cn

[G07] 调用父类方法
来源：http://bz.yuexingan06.cn

Py:   super().greet()
来源：http://dd.bjjhwx.cn

PHP:  parent::greet();
来源：http://ey.9csxet.cn

JS:   super.greet();
来源：http://sc.shtwfgs.cn

TS:   super.greet();
来源：http://zm.nicolike.cn

Java: super.greet();
来源：http://ff.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qt.jianghongdianzi.cn

Ruby: super
来源：http://fz.szxytkj.cn

C#:   base.Greet();
来源：http://lm.colortex.cn

[G08] 静态方法与属性
来源：http://ng.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kl.shtwfgs.cn

PHP:  public static function f() {}
来源：http://qg.lnxyls.cn

JS:   static f() {}
来源：http://um.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://ef.hahajie.cn

Java: static void f() {}
来源：http://oc.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bj.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://rm.szsharing.cn

C#:   public static void F() {}
来源：http://eo.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://jv.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://cr.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://en.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nh.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://il.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://ow.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://qb.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gn.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://xj.nicolike.cn

[G10] 访问控制
来源：http://fd.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://mg.bjjhwx.cn

PHP:  public / protected / private
来源：http://fd.9csxet.cn

JS:   #private 字段；其余公开
来源：http://be.asd995.cn

TS:   public / protected / private
来源：http://qn.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://av.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tl.wgjwhj.cn

Ruby: public / protected / private
来源：http://nf.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://wj.jianghongdianzi.cn

[G11] getter / setter
来源：http://af.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://ju.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nh.colortex.cn

JS:   get name() { return this._name; }
来源：http://dx.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://ak.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://fy.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qy.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://yf.nicolike.cn

C#:   public string Name { get; set; }
来源：http://wd.yuexingan06.cn

[G12] 对象转字符串
来源：http://mu.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://jh.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pe.asd995.cn

JS:   toString() { return this.name; }
来源：http://gp.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://sr.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://qy.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wx.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://qo.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://ts.gzmigu.cn

[G13] 判断对象类型
来源：http://el.szxytkj.cn

Py:   isinstance(u, User)
来源：http://md.hahajie.cn

PHP:  $u instanceof User
来源：http://ub.asd995.cn

JS:   u instanceof User
来源：http://cy.jianghongdianzi.cn

TS:   u instanceof User
来源：http://tj.shtwfgs.cn

Java: u instanceof User
来源：http://sy.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sv.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://sz.haigaiapp.cn

C#:   u is User
来源：http://ar.hnjuh.cn

[G14] 数据类 / record
来源：http://de.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zu.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://xy.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sg.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://tw.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://rc.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://ks.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hl.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://tf.chemitech.net.cn

[G15] 枚举
来源：http://bc.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://it.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hs.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ew.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ny.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://rd.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qi.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://cf.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tt.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://ak.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ew.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://an.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ql.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://pc.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ec.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xh.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://uc.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://rd.jianghongdianzi.cn

================================================================================
来源：http://io.bookmarksfly.cn

H. 异常与错误处理
来源：http://lv.szsharing.cn

================================================================================
来源：http://ux.nszjky.cn

[H01] try / catch 基础
来源：http://xl.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pq.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gj.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oz.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cw.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xy.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ur.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://od.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://st.colortex.cn

[H02] finally / ensure 收尾
来源：http://ht.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gp.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://km.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rx.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mv.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uh.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ib.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oi.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://es.nszjky.cn

[H03] 主动抛出异常
来源：http://fs.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://uf.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://od.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://di.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://gt.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ga.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qv.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ki.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://my.gzmigu.cn

[H04] 自定义异常类型
来源：http://mp.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://td.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gk.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://yh.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://sn.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://kr.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dh.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://sz.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://zb.nicolike.cn

[H05] 捕获特定类型
来源：http://vs.huixiangedu.cn

Py:   except ValueError as e:
来源：http://du.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ti.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://us.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://vp.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://ai.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ly.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://ez.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lc.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://ch.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://ae.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fx.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cx.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vk.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ht.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tm.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://ch.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://ut.szsharing.cn

[H07] 断言
来源：http://ld.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://bq.9csxet.cn

PHP:  assert($x > 0);
来源：http://mk.newstarts.cn

JS:   console.assert(x > 0);
来源：http://ca.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://dx.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://dm.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pb.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://js.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://is.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://ui.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://wq.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nk.asd995.cn

JS:   e.message;  e.stack
来源：http://vs.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ye.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ik.lnxyls.cn

Go:   err.Error()
来源：http://th.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://fy.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://or.gzmigu.cn

[H09] 带错误码的异常
来源：http://dk.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qo.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lr.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vl.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ok.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yu.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wf.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zn.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qk.yuexingan06.cn

[H10] 资源自动释放
来源：http://hl.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uu.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oa.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tk.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://km.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kk.huanxung.cn

Go:   defer f.Close()
来源：http://sj.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gx.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xx.jctech888.com.cn

================================================================================
来源：http://hj.wgjwhj.cn

I. 正则表达式
来源：http://pf.jctech888.com.cn

================================================================================
来源：http://kl.gzmigu.cn

[I01] 判断是否匹配
来源：http://ci.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aj.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mp.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://bn.hahajie.cn

TS:   /\d+/.test(s)
来源：http://jk.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kf.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ad.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://qd.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kr.hnjuh.cn

[I02] 提取所有匹配
来源：http://ww.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://bj.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wy.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zt.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://fb.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gq.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xx.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://kf.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fz.nicolike.cn

[I03] 提取捕获分组
来源：http://tc.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uu.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uh.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yp.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vm.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wb.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mg.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ni.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://on.szxytkj.cn

[I04] 正则替换
来源：http://uh.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zg.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://in.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lc.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bp.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hl.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dz.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eu.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hp.gzmigu.cn

[I05] 按正则拆分
来源：http://me.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fl.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://er.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://cj.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://pv.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://lm.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tt.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qh.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ej.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ys.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vl.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rb.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://st.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yk.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zb.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://td.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zy.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hc.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://fj.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ni.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://se.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nl.shtwfgs.cn

TS:   /error/gim
来源：http://vz.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ia.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ey.asd995.cn

Ruby: s.scan(/error/i)
来源：http://vj.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fv.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://hs.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ih.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gl.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ij.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kp.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lw.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rj.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zs.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tt.hahajie.cn

================================================================================
来源：http://rc.asd995.cn

J. 日期与时间
来源：http://kp.nszjky.cn

================================================================================
来源：http://rf.shxzskj.cn

[J01] 获取当前时间
来源：http://kw.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gr.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dr.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://bp.colortex.cn

TS:   new Date();  Date.now()
来源：http://dd.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ir.shxzukj.cn

Go:   time.Now()
来源：http://bw.lnxyls.cn

Ruby: Time.now
来源：http://km.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ae.521024.cn

[J02] 格式化输出
来源：http://mu.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oz.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ay.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yp.asd995.cn

TS:   d.toISOString()
来源：http://ak.asd995.cn


<!-- 参考信息 -->