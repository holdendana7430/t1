代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://tu.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://rb.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qq.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://ic.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://pw.521024.cn

[G07] 调用父类方法
来源：http://fn.nszjky.cn

Py:   super().greet()
来源：http://hv.nszjky.cn

PHP:  parent::greet();
来源：http://xf.colortex.cn

JS:   super.greet();
来源：http://nl.nicolike.cn

TS:   super.greet();
来源：http://tm.lnxyls.cn

Java: super.greet();
来源：http://ng.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gg.nicolike.cn

Ruby: super
来源：http://dl.shxzukj.cn

C#:   base.Greet();
来源：http://zx.huanxung.cn

[G08] 静态方法与属性
来源：http://gt.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ma.wgjwhj.cn

PHP:  public static function f() {}
来源：http://ax.shxzskj.cn

JS:   static f() {}
来源：http://vk.bookmarksfly.cn

TS:   static f(): void {}
来源：http://jy.hahajie.cn

Java: static void f() {}
来源：http://li.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lx.szxytkj.cn

Ruby: def self.f; end
来源：http://ni.szxytkj.cn

C#:   public static void F() {}
来源：http://bm.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://el.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://bc.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mo.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bm.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://vd.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://yc.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://ku.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ax.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://re.huanxung.cn

[G10] 访问控制
来源：http://qx.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://ch.colortex.cn

PHP:  public / protected / private
来源：http://ld.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://hg.chemitech.net.cn

TS:   public / protected / private
来源：http://np.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://sc.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uq.shxzukj.cn

Ruby: public / protected / private
来源：http://xp.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://ci.huixinmuqiang.cn

[G11] getter / setter
来源：http://qq.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://qa.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ji.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://sf.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://vm.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://ly.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wh.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://nj.newstarts.cn

C#:   public string Name { get; set; }
来源：http://gr.shtwfgs.cn

[G12] 对象转字符串
来源：http://oh.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://zt.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rm.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://ns.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://jy.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://nf.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fl.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://jx.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://lq.hnjuh.cn

[G13] 判断对象类型
来源：http://sl.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://gc.shxzukj.cn

PHP:  $u instanceof User
来源：http://rr.muxihuayi.cn

JS:   u instanceof User
来源：http://pj.yuntaijiaju.cn

TS:   u instanceof User
来源：http://ka.colortex.cn

Java: u instanceof User
来源：http://mb.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yj.colortex.cn

Ruby: u.is_a?(User)
来源：http://ba.huanxung.cn

C#:   u is User
来源：http://st.lnxyls.cn

[G14] 数据类 / record
来源：http://yu.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ck.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://sh.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ja.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://wy.huanxung.cn

Java: record User(String name, int age) {}
来源：http://nx.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://mi.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mx.asd995.cn

C#:   record User(string Name, int Age);
来源：http://mp.jianghongdianzi.cn

[G15] 枚举
来源：http://zu.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fa.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jp.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iv.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ix.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://lf.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nd.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://nu.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kt.colortex.cn

[G16] 对象转数组 / 字典
来源：http://cm.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hx.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://pb.nszjky.cn

JS:   Object.entries(obj)
来源：http://qc.asd995.cn

TS:   Object.entries(obj)
来源：http://pm.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kb.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pc.colortex.cn

Ruby: obj.instance_variables
来源：http://tc.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ja.bjjhwx.cn

================================================================================
来源：http://ns.nszjky.cn

H. 异常与错误处理
来源：http://tf.lnxyls.cn

================================================================================
来源：http://op.huixiangedu.cn

[H01] try / catch 基础
来源：http://rt.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fu.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ux.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bn.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://np.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sa.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rw.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yt.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bq.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://yp.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hu.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ik.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cm.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rn.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gj.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iq.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yr.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mj.521024.cn

[H03] 主动抛出异常
来源：http://el.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://ed.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://og.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://bk.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://mi.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wq.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ad.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ti.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hw.lnxyls.cn

[H04] 自定义异常类型
来源：http://nc.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://xj.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://od.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://bd.szsharing.cn

TS:   class MyError extends Error {}
来源：http://km.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://ed.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://di.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://hp.colortex.cn

C#:   class MyException : Exception {}
来源：http://fi.shxzukj.cn

[H05] 捕获特定类型
来源：http://wc.jctech888.com.cn

Py:   except ValueError as e:
来源：http://ip.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ro.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://pc.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://gk.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://um.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cn.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://os.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wb.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://or.szsharing.cn

Py:   value = d.get("k") or default
来源：http://eo.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://an.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lk.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cu.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jr.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vu.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://fc.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://ts.shxzukj.cn

[H07] 断言
来源：http://ml.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://fc.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://as.hahajie.cn

JS:   console.assert(x > 0);
来源：http://li.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://ox.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://wo.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sm.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ez.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://xe.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://tl.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://ua.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iy.szsharing.cn

JS:   e.message;  e.stack
来源：http://zw.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ey.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pn.shtwfgs.cn

Go:   err.Error()
来源：http://vf.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://co.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://rj.bjjhwx.cn

[H09] 带错误码的异常
来源：http://be.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mi.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bx.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yb.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ew.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jn.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cx.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pk.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pa.shxzukj.cn

[H10] 资源自动释放
来源：http://nj.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tl.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ev.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ei.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ki.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fk.yuexingan06.cn

Go:   defer f.Close()
来源：http://rl.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hg.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kb.jctech888.com.cn

================================================================================
来源：http://mh.chemitech.net.cn

I. 正则表达式
来源：http://hx.muxihuayi.cn

================================================================================
来源：http://vn.jctech888.com.cn

[I01] 判断是否匹配
来源：http://ql.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hc.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ai.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://qm.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://yj.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rq.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bt.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://ii.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yq.shxzskj.cn

[I02] 提取所有匹配
来源：http://wu.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://sv.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ql.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nx.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://au.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vn.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dn.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://dy.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kg.yuexingan06.cn

[I03] 提取捕获分组
来源：http://fs.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qr.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ql.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oc.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ne.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mt.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fr.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dy.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mz.chemitech.net.cn

[I04] 正则替换
来源：http://ik.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://at.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yi.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xh.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ci.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://to.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oc.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hw.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oa.yuexingan06.cn

[I05] 按正则拆分
来源：http://dq.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ap.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ku.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://hk.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://ak.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://cs.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qw.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ck.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ub.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xb.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iu.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ny.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ij.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xn.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gy.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vw.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bp.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://is.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://rf.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lr.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mg.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gh.huixiangedu.cn

TS:   /error/gim
来源：http://dg.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zy.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://if.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://uu.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tq.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://yq.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qk.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ww.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cr.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gg.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://th.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uh.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ll.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sz.panjiajie.cn

================================================================================
来源：http://gq.asd995.cn

J. 日期与时间
来源：http://za.shxzskj.cn

================================================================================
来源：http://tw.bookmarksfly.cn

[J01] 获取当前时间
来源：http://oh.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sr.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rb.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://yr.9csxet.cn

TS:   new Date();  Date.now()
来源：http://og.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ku.jianghongdianzi.cn

Go:   time.Now()
来源：http://yx.szxytkj.cn

Ruby: Time.now
来源：http://nh.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dw.huanxung.cn

[J02] 格式化输出
来源：http://uw.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nn.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ep.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://go.shxzukj.cn

TS:   d.toISOString()
来源：http://sc.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://li.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xc.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://am.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nw.nicolike.cn

[J03] 字符串解析为日期
来源：http://gn.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hv.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qq.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://mq.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://vg.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qs.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vt.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://qz.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nv.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://cx.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://db.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tz.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zo.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qd.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nh.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ah.nszjky.cn


<!-- 参考信息 -->