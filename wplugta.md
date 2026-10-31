代发 wailian999

Java: class Admin extends User {}
来源：http://pv.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kc.nicolike.cn

Ruby: class Admin < User; end
来源：http://ae.hahajie.cn

C#:   class Admin : User {}
来源：http://bv.nicolike.cn

[G06] 重写方法
来源：http://ya.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://uv.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uh.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://kf.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://cv.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://lm.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xc.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://bj.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://lp.shtwfgs.cn

[G07] 调用父类方法
来源：http://ck.bjjhwx.cn

Py:   super().greet()
来源：http://rg.huanxung.cn

PHP:  parent::greet();
来源：http://fo.haigaiapp.cn

JS:   super.greet();
来源：http://ju.bookmarksfly.cn

TS:   super.greet();
来源：http://ea.jctech888.com.cn

Java: super.greet();
来源：http://nu.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wj.lnxyls.cn

Ruby: super
来源：http://vg.jianghongdianzi.cn

C#:   base.Greet();
来源：http://pw.jctech888.com.cn

[G08] 静态方法与属性
来源：http://va.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lv.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://dd.wgjwhj.cn

JS:   static f() {}
来源：http://mz.panjiajie.cn

TS:   static f(): void {}
来源：http://vw.huixinmuqiang.cn

Java: static void f() {}
来源：http://pw.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rq.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://ov.colortex.cn

C#:   public static void F() {}
来源：http://ph.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://wu.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://wz.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ph.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://em.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://es.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://tm.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://wc.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ug.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://qn.shtwfgs.cn

[G10] 访问控制
来源：http://ih.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://wd.shxzskj.cn

PHP:  public / protected / private
来源：http://ga.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://al.huixinmuqiang.cn

TS:   public / protected / private
来源：http://pf.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://qj.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dc.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://fr.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://us.shxzukj.cn

[G11] getter / setter
来源：http://oz.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://ag.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qz.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://rf.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://et.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://jn.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gf.huanxung.cn

Ruby: attr_accessor :name
来源：http://no.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://nf.nicolike.cn

[G12] 对象转字符串
来源：http://ce.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://qt.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pe.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://av.521024.cn

TS:   toString(): string { return this.name; }
来源：http://qp.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://ma.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dm.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://cv.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://xj.newstarts.cn

[G13] 判断对象类型
来源：http://cg.asd995.cn

Py:   isinstance(u, User)
来源：http://vp.panjiajie.cn

PHP:  $u instanceof User
来源：http://eh.bookmarksfly.cn

JS:   u instanceof User
来源：http://wb.521024.cn

TS:   u instanceof User
来源：http://cf.asd995.cn

Java: u instanceof User
来源：http://cm.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lr.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://od.asd995.cn

C#:   u is User
来源：http://no.asd995.cn

[G14] 数据类 / record
来源：http://gl.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ya.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://qp.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eq.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://gg.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://pb.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://sb.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iv.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://dl.hnjuh.cn

[G15] 枚举
来源：http://jx.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tc.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vg.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bu.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rn.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://io.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iz.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://kp.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kp.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://xt.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://an.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://ef.lnxyls.cn

JS:   Object.entries(obj)
来源：http://eq.gzmigu.cn

TS:   Object.entries(obj)
来源：http://ne.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wp.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jh.9csxet.cn

Ruby: obj.instance_variables
来源：http://hd.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://pv.hnjuh.cn

================================================================================
来源：http://db.yuexingan06.cn

H. 异常与错误处理
来源：http://pc.szsharing.cn

================================================================================
来源：http://tp.huixiangedu.cn

[H01] try / catch 基础
来源：http://jm.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eg.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vu.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ge.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ya.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pu.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fh.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ll.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jz.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://mw.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mu.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ge.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://af.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jt.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pn.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mw.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://av.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yb.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://mg.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://jn.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kb.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://tt.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://qq.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qk.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xz.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pp.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hn.gzmigu.cn

[H04] 自定义异常类型
来源：http://pl.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://sl.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ld.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://bb.newstarts.cn

TS:   class MyError extends Error {}
来源：http://ql.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://gx.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yz.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://ze.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://nt.colortex.cn

[H05] 捕获特定类型
来源：http://vr.huanxung.cn

Py:   except ValueError as e:
来源：http://fr.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://ip.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://vc.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://zn.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uk.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://la.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iy.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ey.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://mh.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jr.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hw.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sc.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cy.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yz.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://ub.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://qv.jianghongdianzi.cn

[H07] 断言
来源：http://hd.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://lw.colortex.cn

PHP:  assert($x > 0);
来源：http://up.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://kr.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://us.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://qz.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vw.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mq.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://ap.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://kw.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://ue.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wl.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://vh.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wv.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qb.huanxung.cn

Go:   err.Error()
来源：http://oz.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://dz.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://jq.gzmigu.cn

[H09] 带错误码的异常
来源：http://qq.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nn.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ef.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fr.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eh.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tl.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oa.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fs.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ef.gzmigu.cn

[H10] 资源自动释放
来源：http://se.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yz.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gh.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ut.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wm.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fq.yuexingan06.cn

Go:   defer f.Close()
来源：http://od.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ng.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hs.colortex.cn

================================================================================
来源：http://cl.jianghongdianzi.cn

I. 正则表达式
来源：http://aa.bjjhwx.cn

================================================================================
来源：http://pu.jctech888.com.cn

[I01] 判断是否匹配
来源：http://dx.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yx.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yv.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://ld.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://fs.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://em.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bt.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://ue.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zr.colortex.cn

[I02] 提取所有匹配
来源：http://vi.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://ni.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mn.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tl.asd995.cn

TS:   s.match(/\d+/g)
来源：http://mn.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uy.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hw.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://wr.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ny.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://fl.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gd.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://za.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sv.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gw.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ly.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xs.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fj.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ld.bookmarksfly.cn

[I04] 正则替换
来源：http://qj.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jk.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pd.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zd.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bv.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kn.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sx.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fj.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wc.521024.cn

[I05] 按正则拆分
来源：http://bj.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eb.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://su.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://tb.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://ym.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://gq.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ns.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bi.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://di.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wx.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://io.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gy.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ka.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qv.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kl.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oc.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://te.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xr.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://hj.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dg.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yu.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wd.nszjky.cn

TS:   /error/gim
来源：http://fu.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bx.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qp.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://ua.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mp.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://ao.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ju.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ya.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://am.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ba.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jk.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qx.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://et.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qu.jctech888.com.cn

================================================================================
来源：http://uz.bjjhwx.cn

J. 日期与时间
来源：http://qf.colortex.cn

================================================================================
来源：http://sm.shxzskj.cn

[J01] 获取当前时间
来源：http://ii.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ir.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xx.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://ly.nicolike.cn

TS:   new Date();  Date.now()
来源：http://lm.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xj.lnxyls.cn

Go:   time.Now()
来源：http://ku.asd995.cn

Ruby: Time.now
来源：http://sq.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gn.chemitech.net.cn

[J02] 格式化输出
来源：http://bw.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ok.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ox.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ao.521024.cn

TS:   d.toISOString()
来源：http://rm.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qf.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ci.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uh.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hm.9csxet.cn

[J03] 字符串解析为日期
来源：http://wq.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qq.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://el.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://lv.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://dl.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bm.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://od.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ym.jctech888.com.cn


<!-- 参考信息 -->