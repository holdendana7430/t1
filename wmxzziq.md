代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://ku.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ab.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://fm.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zo.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://ok.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jk.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sd.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cc.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uj.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://ba.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://tj.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://zm.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vv.jctech888.com.cn

[A03] 常量定义
来源：http://vr.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ze.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://cr.9csxet.cn

JS:   const PI = 3.14159;
来源：http://ki.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://yf.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://gi.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://lw.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://ao.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://ff.panjiajie.cn

[A04] 判断变量类型
来源：http://ft.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dr.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cp.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pp.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://sl.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kw.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://it.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oz.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://pm.hahajie.cn

[A05] 整数除法与取模
来源：http://xd.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ke.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wi.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ey.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rd.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://sk.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://qb.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://hl.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://ja.lnxyls.cn

[A06] 字符串转数字
来源：http://cj.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://ap.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vm.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ua.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hm.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://do.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wz.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ma.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ii.hahajie.cn

[A07] 数字转字符串
来源：http://ht.9csxet.cn

Py:   str(42)
来源：http://en.521024.cn

PHP:  (string) 42; strval(42)
来源：http://zg.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://yk.bjjhwx.cn

TS:   String(42)
来源：http://jn.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ac.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://tu.muxihuayi.cn

Ruby: 42.to_s
来源：http://wl.jctech888.com.cn

C#:   42.ToString()
来源：http://lo.gzmigu.cn

[A08] 取整与四舍五入
来源：http://zh.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vd.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sh.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dh.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://du.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fk.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mu.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mf.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xh.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://bv.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://is.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://eu.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pt.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cx.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xi.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bo.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yg.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ko.bookmarksfly.cn

[A10] 生成随机数
来源：http://nb.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://fl.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://en.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wd.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xb.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://te.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sv.shtwfgs.cn

Ruby: rand(1..100)
来源：http://js.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://cu.nicolike.cn

[A11] 条件表达式（三元）
来源：http://bw.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://el.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tw.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mt.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://od.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://ar.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zk.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xy.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ab.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://kp.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xq.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iz.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://ec.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://fk.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://fx.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ms.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ul.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://nu.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://aw.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://ug.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://al.hahajie.cn

JS:   "第一行\n第二行"
来源：http://so.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://cz.gzmigu.cn

Java: "第一行\n第二行"
来源：http://kg.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://bn.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://jd.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://ox.hnjuh.cn

[A14] 注释写法
来源：http://pt.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eg.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://go.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://bo.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://mj.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tu.521024.cn

Go:   // 单行；/* 多行 */
来源：http://nq.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ti.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://qg.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://ui.shxzskj.cn

Py:   value = data or "默认值"
来源：http://oo.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://dq.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://az.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://te.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eu.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://pc.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://mk.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://lo.9csxet.cn

[A16] 真假值判断规则
来源：http://uc.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kd.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fd.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oa.asd995.cn

TS:   if (!x) {}
来源：http://jm.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yn.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ll.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sx.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cq.huixiangedu.cn

[A17] 位运算
来源：http://sn.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ks.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://je.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ed.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wo.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ns.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fp.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sk.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oj.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://zb.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://lx.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://hg.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jg.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xg.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://kw.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dx.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://id.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://xo.huanxung.cn

[A19] 交换两个变量
来源：http://hd.bjjhwx.cn

Py:   a, b = b, a
来源：http://zu.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hl.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://iy.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://us.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://ne.wgjwhj.cn

Go:   a, b = b, a
来源：http://vv.haigaiapp.cn

Ruby: a, b = b, a
来源：http://ev.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://jk.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ro.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://bw.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iz.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hy.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://ai.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://ff.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cy.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://ie.asd995.cn

C#:   Console.ReadLine();
来源：http://hn.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://oo.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://ma.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vq.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://hm.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://kq.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://ew.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ns.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://dk.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://dy.nicolike.cn

[A22] 获取字符串长度
来源：http://ea.shxzukj.cn

Py:   len(s)
来源：http://rt.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wp.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zl.huixiangedu.cn

TS:   s.length
来源：http://rw.chemitech.net.cn

Java: s.length()
来源：http://yt.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dv.bookmarksfly.cn

Ruby: s.length
来源：http://id.shtwfgs.cn

C#:   s.Length
来源：http://ax.wgjwhj.cn

[A23] 大小写转换
来源：http://xu.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yb.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://po.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://he.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wa.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lc.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vg.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jz.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ct.asd995.cn

[A24] 去除首尾空白
来源：http://kd.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tg.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rh.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tz.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://px.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uv.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://zj.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://np.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ng.bjjhwx.cn

[A25] 字符串比较
来源：http://fi.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://jg.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://br.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yf.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tx.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vq.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gn.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gk.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ff.nszjky.cn

[A26] 类型转换总览
来源：http://pl.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xj.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qk.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://um.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://lc.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fz.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xq.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qm.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vy.hahajie.cn

================================================================================
来源：http://gr.yuexingan06.cn

B. 流程控制
来源：http://lc.9csxet.cn

================================================================================
来源：http://gu.nszjky.cn

[B01] 条件判断 if / else
来源：http://to.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tv.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zq.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://at.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://on.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tg.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xv.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cd.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pd.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://xk.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ji.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://go.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fv.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://af.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xl.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qx.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yl.muxihuayi.cn

[B03] switch / match / case
来源：http://mg.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zo.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mt.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aa.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kj.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://va.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pq.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xv.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eo.jctech888.com.cn

[B04] for 计数循环
来源：http://vv.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://tw.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://by.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ap.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tc.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ap.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eb.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://as.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jq.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://du.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://mv.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zz.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://am.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cm.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qn.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oq.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://fl.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bq.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://mn.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gg.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yq.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sc.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bz.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://li.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gl.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wc.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ew.bookmarksfly.cn

[B07] while 循环
来源：http://ul.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://wj.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://om.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://wc.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://wq.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://pu.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vv.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://cp.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://ck.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://jc.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://vi.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aw.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://jg.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://yi.lnxyls.cn


<!-- 参考信息 -->