代发 wailian999

[A02] 变量声明与赋值
来源：http://xh.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iz.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wv.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qi.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mw.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://wo.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://cu.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://tp.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cx.szxytkj.cn

[A03] 常量定义
来源：http://oh.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jy.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://ah.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://bt.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://vq.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://dp.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://xx.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://av.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://bj.jctech888.com.cn

[A04] 判断变量类型
来源：http://uv.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sw.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qq.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jq.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://vl.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jq.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yf.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yh.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://ey.szsharing.cn

[A05] 整数除法与取模
来源：http://el.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ij.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cg.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xo.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ih.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://hz.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://gx.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://qh.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://qi.yuexingan06.cn

[A06] 字符串转数字
来源：http://ck.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://pz.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ot.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ur.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uh.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ui.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ud.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mu.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ck.bjjhwx.cn

[A07] 数字转字符串
来源：http://kc.huixiangedu.cn

Py:   str(42)
来源：http://ra.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://gl.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://yg.shxzukj.cn

TS:   String(42)
来源：http://es.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ka.asd995.cn

Go:   strconv.Itoa(42)
来源：http://tc.9csxet.cn

Ruby: 42.to_s
来源：http://sa.jctech888.com.cn

C#:   42.ToString()
来源：http://zm.huanxung.cn

[A08] 取整与四舍五入
来源：http://wu.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hi.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wi.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fe.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sd.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pr.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yi.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kt.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fr.521024.cn

[A09] 绝对值与最大最小值
来源：http://ji.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tz.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fy.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ex.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ew.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zu.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gc.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uh.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ha.panjiajie.cn

[A10] 生成随机数
来源：http://lr.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://jw.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://tg.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ev.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lw.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://dl.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cf.hnjuh.cn

Ruby: rand(1..100)
来源：http://xj.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://pd.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://di.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://rz.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://to.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sk.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://ap.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wv.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dc.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gl.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://to.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hu.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://js.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://do.521024.cn

TS:   `Hello, ${name}!`
来源：http://gz.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://wl.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oq.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://vz.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://cg.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://em.huanxung.cn

Py:   "第一行\n第二行"
来源：http://to.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://za.huanxung.cn

JS:   "第一行\n第二行"
来源：http://ub.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://np.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://do.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://wp.asd995.cn

Ruby: "第一行\n第二行"
来源：http://wr.asd995.cn

C#:   "第一行\n第二行"
来源：http://gi.shtwfgs.cn

[A14] 注释写法
来源：http://ln.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tn.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gr.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://ce.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://aj.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ks.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://mq.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fr.521024.cn

C#:   // 单行；/* 多行 */
来源：http://oq.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://pm.shxzskj.cn

Py:   value = data or "默认值"
来源：http://nx.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://hw.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://io.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://od.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tn.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://up.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://eg.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://qh.huixiangedu.cn

[A16] 真假值判断规则
来源：http://ec.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://op.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uz.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ce.panjiajie.cn

TS:   if (!x) {}
来源：http://dd.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mk.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yh.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gk.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kn.huixinmuqiang.cn

[A17] 位运算
来源：http://kr.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cb.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://av.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gm.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lm.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hx.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pm.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jk.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://im.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://qz.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://yp.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://ba.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lc.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://co.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://jp.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sj.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://ws.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://wl.wgjwhj.cn

[A19] 交换两个变量
来源：http://ds.huixiangedu.cn

Py:   a, b = b, a
来源：http://vm.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uo.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://hm.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://xi.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://yy.hnjuh.cn

Go:   a, b = b, a
来源：http://hi.muxihuayi.cn

Ruby: a, b = b, a
来源：http://tg.asd995.cn

C#:   (a, b) = (b, a);
来源：http://zq.nszjky.cn

[A20] 读取标准输入
来源：http://mi.panjiajie.cn

Py:   name = input("请输入：")
来源：http://it.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ua.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qx.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://jq.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://uv.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kc.nszjky.cn

Ruby: gets.chomp
来源：http://tb.hnjuh.cn

C#:   Console.ReadLine();
来源：http://iy.9csxet.cn

[A21] 保留指定小数位输出
来源：http://cr.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://xq.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://en.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://pc.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://et.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://jy.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vi.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://zg.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://oa.lnxyls.cn

[A22] 获取字符串长度
来源：http://ff.hahajie.cn

Py:   len(s)
来源：http://gu.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vc.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pw.9csxet.cn

TS:   s.length
来源：http://om.9csxet.cn

Java: s.length()
来源：http://os.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ya.nicolike.cn

Ruby: s.length
来源：http://re.asd995.cn

C#:   s.Length
来源：http://uu.huixiangedu.cn

[A23] 大小写转换
来源：http://jk.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://le.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oq.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ry.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nh.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dg.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zq.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ol.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dy.asd995.cn

[A24] 去除首尾空白
来源：http://mc.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uy.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tq.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://un.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oo.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ya.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://dv.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://be.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qx.szxytkj.cn

[A25] 字符串比较
来源：http://mz.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://po.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nb.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ht.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yv.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xf.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yt.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yr.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lg.huixiangedu.cn

[A26] 类型转换总览
来源：http://fu.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yx.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ay.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bg.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://fo.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vz.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ju.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oc.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://er.jctech888.com.cn

================================================================================
来源：http://pw.nicolike.cn

B. 流程控制
来源：http://rx.chemitech.net.cn

================================================================================
来源：http://md.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://zt.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ag.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lb.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yt.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sb.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ny.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wc.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uw.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xo.colortex.cn

[B02] 多分支 else if / elif
来源：http://fk.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xn.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iq.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pp.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nl.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fe.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fb.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://du.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vj.yuntaijiaju.cn

[B03] switch / match / case
来源：http://as.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sq.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oh.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yk.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vw.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sb.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zf.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vo.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bz.shtwfgs.cn

[B04] for 计数循环
来源：http://nn.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://nw.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dg.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hu.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vi.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wy.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hg.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://jn.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eb.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://la.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://jy.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aw.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sk.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cr.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ja.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ac.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://kc.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oh.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://ei.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qa.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://to.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gf.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mw.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ru.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jf.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cf.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sm.gzmigu.cn

[B07] while 循环
来源：http://ek.hahajie.cn

Py:   while i < 10: i += 1
来源：http://ih.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fd.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://kb.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://xq.asd995.cn

Java: while (i < 10) { i++; }
来源：http://pn.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zh.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://zs.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://sq.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://qe.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://tk.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vy.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://sy.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://bh.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://tt.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wn.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gs.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://ne.521024.cn


<!-- 参考信息 -->