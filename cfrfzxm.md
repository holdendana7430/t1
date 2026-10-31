代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://cy.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://tg.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://xt.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xr.521024.cn

[A02] 变量声明与赋值
来源：http://mo.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jd.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://aa.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jw.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nm.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://ny.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://zz.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://lv.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cn.muxihuayi.cn

[A03] 常量定义
来源：http://sq.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hj.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://mq.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://ea.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://ck.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://pp.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://yc.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://sg.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://dr.asd995.cn

[A04] 判断变量类型
来源：http://ur.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wc.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://us.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eh.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://ww.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ek.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ze.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vj.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://il.lnxyls.cn

[A05] 整数除法与取模
来源：http://nn.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ek.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yl.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pw.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fa.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://tq.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://ek.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://gs.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://sg.lnxyls.cn

[A06] 字符串转数字
来源：http://gh.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://lj.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cv.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vx.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cm.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tx.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dm.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tp.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bj.hnjuh.cn

[A07] 数字转字符串
来源：http://ar.lnxyls.cn

Py:   str(42)
来源：http://dx.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://xb.szsharing.cn

JS:   String(42); (42).toString()
来源：http://kt.nicolike.cn

TS:   String(42)
来源：http://ru.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://py.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://mm.bookmarksfly.cn

Ruby: 42.to_s
来源：http://ke.521024.cn

C#:   42.ToString()
来源：http://nm.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://mg.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ms.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uh.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rk.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xn.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hn.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://we.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ij.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hs.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://qk.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://de.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rh.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sj.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nl.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gu.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tj.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lf.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bs.hahajie.cn

[A10] 生成随机数
来源：http://xw.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://vw.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://zc.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wo.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qf.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://ie.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ht.shxzukj.cn

Ruby: rand(1..100)
来源：http://xo.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://qs.newstarts.cn

[A11] 条件表达式（三元）
来源：http://lf.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://bl.jianghongdianzi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yj.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bx.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://si.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://mn.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gy.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bj.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pj.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://xv.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kq.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pj.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://gl.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://fl.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://vh.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://go.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://qe.521024.cn

C#:   $"Hello, {name}!"
来源：http://uo.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pj.hahajie.cn

Py:   "第一行\n第二行"
来源：http://ng.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://it.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://hb.9csxet.cn

TS:   "第一行\n第二行"
来源：http://wk.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://dz.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://ag.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://gf.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://iy.huixinmuqiang.cn

[A14] 注释写法
来源：http://tz.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ox.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tw.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://lt.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://wn.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://np.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://vp.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ze.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://wr.gzmigu.cn

[A15] 空值判断与默认值
来源：http://mr.nszjky.cn

Py:   value = data or "默认值"
来源：http://pv.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://kh.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://jx.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://ix.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kd.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://ru.9csxet.cn

Ruby: value = data || "默认值"
来源：http://ev.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://yw.muxihuayi.cn

[A16] 真假值判断规则
来源：http://vt.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lv.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jp.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rd.huanxung.cn

TS:   if (!x) {}
来源：http://ov.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fl.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wy.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sl.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zt.szsharing.cn

[A17] 位运算
来源：http://ar.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ib.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mh.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zl.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://as.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zr.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ho.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rs.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hr.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://za.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://lb.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://vw.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sg.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tg.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://nk.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cf.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://vh.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://uy.chemitech.net.cn

[A19] 交换两个变量
来源：http://he.521024.cn

Py:   a, b = b, a
来源：http://bp.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zu.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://er.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://ux.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://db.szxytkj.cn

Go:   a, b = b, a
来源：http://vz.chemitech.net.cn

Ruby: a, b = b, a
来源：http://bs.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://cz.bjjhwx.cn

[A20] 读取标准输入
来源：http://wi.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://cc.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cb.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tt.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://vv.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://nx.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nl.nicolike.cn

Ruby: gets.chomp
来源：http://az.lnxyls.cn

C#:   Console.ReadLine();
来源：http://uv.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://is.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://kf.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ft.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://uq.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://zk.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://ff.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hu.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://wj.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://wy.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://jo.jianghongdianzi.cn

Py:   len(s)
来源：http://ta.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://it.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ng.colortex.cn

TS:   s.length
来源：http://vp.haigaiapp.cn

Java: s.length()
来源：http://gx.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bn.hnjuh.cn

Ruby: s.length
来源：http://rf.huixinmuqiang.cn

C#:   s.Length
来源：http://su.huixiangedu.cn

[A23] 大小写转换
来源：http://ye.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ex.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lv.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ob.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eu.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tp.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://si.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ds.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dd.szxytkj.cn

[A24] 去除首尾空白
来源：http://nn.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://je.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yz.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cz.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mi.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sd.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://vq.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kf.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vh.shtwfgs.cn

[A25] 字符串比较
来源：http://xn.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://rh.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zb.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xn.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ii.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bv.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://on.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ug.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xn.panjiajie.cn

[A26] 类型转换总览
来源：http://sn.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://od.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sq.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xo.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://hb.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pt.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vm.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gz.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uj.colortex.cn

================================================================================
来源：http://mg.9csxet.cn

B. 流程控制
来源：http://ae.muxihuayi.cn

================================================================================
来源：http://br.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://td.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bi.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rn.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zf.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://de.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bs.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ke.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qs.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yh.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://dv.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://im.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bd.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jo.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dk.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://el.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vy.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.muxihuayi.cn

[B03] switch / match / case
来源：http://uv.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://go.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ge.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://av.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jd.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pf.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ld.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ar.wgjwhj.cn

[B04] for 计数循环
来源：http://jd.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://zj.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zy.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xt.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ho.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iy.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yw.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://pi.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fw.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://ph.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://hy.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ul.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pr.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yd.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ci.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hv.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://it.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ia.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://gi.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qz.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ei.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://op.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vy.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gs.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://be.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qq.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dx.yuntaijiaju.cn

[B07] while 循环
来源：http://zm.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://bi.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ei.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://iw.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://up.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://al.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ay.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://cc.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://ol.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://tw.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://gs.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://id.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://nt.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://xd.shtwfgs.cn


<!-- 参考信息 -->