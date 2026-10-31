代发 wailian999

[A02] 变量声明与赋值
来源：http://hw.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ge.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jf.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ke.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qz.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://mk.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://aq.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://lq.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ux.huixiangedu.cn

[A03] 常量定义
来源：http://ea.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hb.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://tk.huanxung.cn

JS:   const PI = 3.14159;
来源：http://ml.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://eb.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://ym.huanxung.cn

Go:   const PI = 3.14159
来源：http://ot.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://wi.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://xb.newstarts.cn

[A04] 判断变量类型
来源：http://ay.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bj.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pc.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lk.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://ta.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ak.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tt.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ns.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://lz.hnjuh.cn

[A05] 整数除法与取模
来源：http://jy.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dt.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xr.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ln.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nr.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://ha.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://an.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://pu.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://yf.haigaiapp.cn

[A06] 字符串转数字
来源：http://yb.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://ba.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ga.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jw.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zj.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tn.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cg.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pu.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xs.huanxung.cn

[A07] 数字转字符串
来源：http://bc.gzmigu.cn

Py:   str(42)
来源：http://tt.521024.cn

PHP:  (string) 42; strval(42)
来源：http://gt.colortex.cn

JS:   String(42); (42).toString()
来源：http://mb.gzmigu.cn

TS:   String(42)
来源：http://er.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sl.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://uj.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://yq.szxytkj.cn

C#:   42.ToString()
来源：http://ji.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://jj.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vu.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://on.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sn.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pq.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ig.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pw.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ga.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pk.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://hh.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ul.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yz.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ig.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ue.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uj.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kc.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ur.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://po.bookmarksfly.cn

[A10] 生成随机数
来源：http://xq.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://zg.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://xa.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hl.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://od.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://qh.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zu.gzmigu.cn

Ruby: rand(1..100)
来源：http://di.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://fk.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://za.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://zy.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uw.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sd.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fc.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://oy.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ps.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ba.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vh.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://lq.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kd.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yj.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://nf.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://vk.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://yg.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ow.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://nq.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://om.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ru.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://cb.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://iv.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://cp.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://iv.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://ou.hahajie.cn

Go:   "第一行\n第二行"
来源：http://en.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://yf.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://wq.jctech888.com.cn

[A14] 注释写法
来源：http://zn.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://us.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ol.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://qp.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://hl.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vd.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://cj.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ne.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://sa.nicolike.cn

[A15] 空值判断与默认值
来源：http://sl.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://le.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://yq.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://mv.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://rx.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ph.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://qk.huanxung.cn

Ruby: value = data || "默认值"
来源：http://gi.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://uu.nicolike.cn

[A16] 真假值判断规则
来源：http://xs.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eo.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uc.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hj.nicolike.cn

TS:   if (!x) {}
来源：http://hp.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zo.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ng.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://si.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nr.lnxyls.cn

[A17] 位运算
来源：http://yb.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sz.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fo.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ng.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ck.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dt.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wo.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zk.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gp.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://fz.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://iz.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://yp.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xo.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dq.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://za.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ix.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://lr.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://rj.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://nh.hahajie.cn

Py:   a, b = b, a
来源：http://nq.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ne.colortex.cn

JS:   [a, b] = [b, a];
来源：http://nh.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://zw.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://eq.jctech888.com.cn

Go:   a, b = b, a
来源：http://cu.bjjhwx.cn

Ruby: a, b = b, a
来源：http://yf.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://hv.chemitech.net.cn

[A20] 读取标准输入
来源：http://rg.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://is.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eh.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oj.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://yx.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://zq.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nd.9csxet.cn

Ruby: gets.chomp
来源：http://ms.huanxung.cn

C#:   Console.ReadLine();
来源：http://ot.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://jd.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://mp.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rv.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://ft.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://hs.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://yf.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oq.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://mi.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://gu.bjjhwx.cn

[A22] 获取字符串长度
来源：http://ng.jianghongdianzi.cn

Py:   len(s)
来源：http://uv.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dq.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cu.szsharing.cn

TS:   s.length
来源：http://xt.huixinmuqiang.cn

Java: s.length()
来源：http://he.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bs.shxzukj.cn

Ruby: s.length
来源：http://ag.shxzskj.cn

C#:   s.Length
来源：http://fv.chemitech.net.cn

[A23] 大小写转换
来源：http://jq.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://na.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pk.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pw.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fs.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bp.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://op.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jn.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fk.nszjky.cn

[A24] 去除首尾空白
来源：http://zb.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tp.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ni.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vs.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ee.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ss.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://it.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bf.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cu.colortex.cn

[A25] 字符串比较
来源：http://br.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://mx.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lk.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pa.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cc.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ef.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rg.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gk.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mo.wgjwhj.cn

[A26] 类型转换总览
来源：http://um.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hb.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qn.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ao.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://ij.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oy.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rw.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hr.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bk.jctech888.com.cn

================================================================================
来源：http://yj.bookmarksfly.cn

B. 流程控制
来源：http://em.panjiajie.cn

================================================================================
来源：http://no.hnjuh.cn

[B01] 条件判断 if / else
来源：http://bh.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://im.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ru.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vi.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dw.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tw.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rd.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dg.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qx.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://va.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://om.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zd.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://om.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uq.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ms.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ky.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hq.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.szsharing.cn

[B03] switch / match / case
来源：http://qm.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ns.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ws.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mu.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tx.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rh.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rf.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mh.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wn.huanxung.cn

[B04] for 计数循环
来源：http://sl.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://xs.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vj.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iy.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mg.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dp.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mz.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://ge.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cj.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://nr.szsharing.cn

Py:   for item in arr: print(item)
来源：http://kl.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://is.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ya.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hf.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lq.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pf.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://oo.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ol.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://hg.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://on.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sj.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ax.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wt.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ue.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kx.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ut.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://la.huixiangedu.cn

[B07] while 循环
来源：http://rr.asd995.cn

Py:   while i < 10: i += 1
来源：http://ll.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fb.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://tb.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://ig.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://te.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zc.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://ec.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://sc.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://bq.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://fz.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fg.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://lx.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://xf.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://jd.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ja.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lm.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://ns.szxytkj.cn


<!-- 参考信息 -->