代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://do.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://ih.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ue.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://jg.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://wk.colortex.cn

[G07] 调用父类方法
来源：http://an.wgjwhj.cn

Py:   super().greet()
来源：http://rz.chemitech.net.cn

PHP:  parent::greet();
来源：http://ab.shxzukj.cn

JS:   super.greet();
来源：http://zl.yuexingan06.cn

TS:   super.greet();
来源：http://hb.muxihuayi.cn

Java: super.greet();
来源：http://qy.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ib.newstarts.cn

Ruby: super
来源：http://au.shxzskj.cn

C#:   base.Greet();
来源：http://yp.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://qx.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dx.chemitech.net.cn

PHP:  public static function f() {}
来源：http://iv.nicolike.cn

JS:   static f() {}
来源：http://gd.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://vx.bookmarksfly.cn

Java: static void f() {}
来源：http://gt.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tg.newstarts.cn

Ruby: def self.f; end
来源：http://wu.521024.cn

C#:   public static void F() {}
来源：http://ju.nszjky.cn

[G09] 接口 / 抽象类
来源：http://zr.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://ya.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vt.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bg.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://sh.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://hn.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://yi.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gj.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://id.huanxung.cn

[G10] 访问控制
来源：http://yv.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://ov.521024.cn

PHP:  public / protected / private
来源：http://dp.colortex.cn

JS:   #private 字段；其余公开
来源：http://dr.hahajie.cn

TS:   public / protected / private
来源：http://vr.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://zs.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jk.jctech888.com.cn

Ruby: public / protected / private
来源：http://zi.hnjuh.cn

C#:   public / protected / private / internal
来源：http://qq.huixinmuqiang.cn

[G11] getter / setter
来源：http://hy.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://yt.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eq.nszjky.cn

JS:   get name() { return this._name; }
来源：http://xv.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://eg.hahajie.cn

Java: public String getName() { return name; }
来源：http://gi.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qu.9csxet.cn

Ruby: attr_accessor :name
来源：http://nr.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://sg.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://fs.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://fx.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zu.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://nx.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://ur.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://as.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cz.newstarts.cn

Ruby: def to_s; @name; end
来源：http://jo.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://jq.szsharing.cn

[G13] 判断对象类型
来源：http://hz.shxzskj.cn

Py:   isinstance(u, User)
来源：http://od.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://wj.huixinmuqiang.cn

JS:   u instanceof User
来源：http://py.muxihuayi.cn

TS:   u instanceof User
来源：http://xb.newstarts.cn

Java: u instanceof User
来源：http://cy.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tc.huanxung.cn

Ruby: u.is_a?(User)
来源：http://ke.yuexingan06.cn

C#:   u is User
来源：http://jl.shtwfgs.cn

[G14] 数据类 / record
来源：http://sv.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yi.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://yt.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kw.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://db.nszjky.cn

Java: record User(String name, int age) {}
来源：http://kt.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://ug.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lu.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://ag.9csxet.cn

[G15] 枚举
来源：http://pb.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vx.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rr.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jc.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vd.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://wm.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cl.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://ds.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vg.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://pt.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nl.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://ue.huanxung.cn

JS:   Object.entries(obj)
来源：http://mg.panjiajie.cn

TS:   Object.entries(obj)
来源：http://jb.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yr.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://zj.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://uv.jianghongdianzi.cn

================================================================================
来源：http://rv.hahajie.cn

H. 异常与错误处理
来源：http://wp.huanxung.cn

================================================================================
来源：http://fh.hahajie.cn

[H01] try / catch 基础
来源：http://cn.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ip.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bs.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bc.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ti.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yy.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gb.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qn.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ql.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ki.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pf.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vu.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wr.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rb.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pn.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ic.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ok.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dj.szsharing.cn

[H03] 主动抛出异常
来源：http://oi.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://jq.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pr.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://ei.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://wn.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tc.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lg.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fi.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ic.hnjuh.cn

[H04] 自定义异常类型
来源：http://ma.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://al.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vh.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://ay.nicolike.cn

TS:   class MyError extends Error {}
来源：http://lt.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://kb.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://un.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://yq.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://mx.521024.cn

[H05] 捕获特定类型
来源：http://mr.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://mc.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://te.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://li.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://hp.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://qv.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://az.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://mw.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://na.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://xn.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://xb.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vt.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://du.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nz.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jm.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qs.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://sc.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://eu.bookmarksfly.cn

[H07] 断言
来源：http://bf.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://pt.hahajie.cn

PHP:  assert($x > 0);
来源：http://kq.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://ma.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://zv.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://mp.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ak.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qm.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://ai.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://zr.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://dz.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ae.521024.cn

JS:   e.message;  e.stack
来源：http://tm.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yi.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fn.huanxung.cn

Go:   err.Error()
来源：http://gm.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://xs.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://hm.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://ce.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yp.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vf.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gk.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gt.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ez.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lw.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://om.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mc.hahajie.cn

[H10] 资源自动释放
来源：http://gv.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fb.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://km.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://le.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wv.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kl.asd995.cn

Go:   defer f.Close()
来源：http://gm.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tu.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wq.wgjwhj.cn

================================================================================
来源：http://tb.nicolike.cn

I. 正则表达式
来源：http://nz.chemitech.net.cn

================================================================================
来源：http://yu.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://yi.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bb.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://is.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://kk.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://ay.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ya.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ke.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://fx.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wm.yuexingan06.cn

[I02] 提取所有匹配
来源：http://hg.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://zg.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gw.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://li.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://ed.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://as.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rc.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://jx.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vu.9csxet.cn

[I03] 提取捕获分组
来源：http://uo.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gu.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dk.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ld.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bu.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uy.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hp.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ml.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://az.muxihuayi.cn

[I04] 正则替换
来源：http://it.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oq.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lo.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pr.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://il.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ww.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wv.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hj.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gn.521024.cn

[I05] 按正则拆分
来源：http://oz.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ty.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qd.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ii.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://dw.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://cw.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lr.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dn.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bn.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lv.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://du.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iz.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zo.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lv.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wb.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pm.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oj.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jh.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://ng.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hc.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tx.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kd.hahajie.cn

TS:   /error/gim
来源：http://th.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://og.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ch.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://fq.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eb.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://gf.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eh.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dj.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kc.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qc.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zf.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vd.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mp.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gt.panjiajie.cn

================================================================================
来源：http://pz.jctech888.com.cn

J. 日期与时间
来源：http://sl.gzmigu.cn

================================================================================
来源：http://og.huixiangedu.cn

[J01] 获取当前时间
来源：http://bx.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ek.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yv.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://gg.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://rx.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ji.szxytkj.cn

Go:   time.Now()
来源：http://po.chemitech.net.cn

Ruby: Time.now
来源：http://py.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://km.shxzskj.cn

[J02] 格式化输出
来源：http://cu.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wu.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zg.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rl.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://bw.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ik.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://be.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fm.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://od.nszjky.cn

[J03] 字符串解析为日期
来源：http://bn.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ju.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qq.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://qv.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://sy.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ru.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cw.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://eb.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ta.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://kb.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sy.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sp.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ki.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fh.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lb.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wo.nszjky.cn


<!-- 参考信息 -->