代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nz.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://xf.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://za.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://mq.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lk.gzmigu.cn

[A03] 常量定义
来源：http://tj.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://np.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://tp.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://ha.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://qk.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://xf.gzmigu.cn

Go:   const PI = 3.14159
来源：http://ft.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://pf.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://ma.nszjky.cn

[A04] 判断变量类型
来源：http://sb.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dn.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ir.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://av.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://ug.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qk.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dq.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://go.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://uc.haigaiapp.cn

[A05] 整数除法与取模
来源：http://kj.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://up.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kq.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ly.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xx.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://dg.521024.cn

Go:   7 / 2; 7 % 2
来源：http://mt.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://up.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://rq.wgjwhj.cn

[A06] 字符串转数字
来源：http://qw.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://om.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yl.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dw.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cl.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vb.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jx.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hm.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tu.shxzukj.cn

[A07] 数字转字符串
来源：http://hc.lnxyls.cn

Py:   str(42)
来源：http://vi.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://ah.colortex.cn

JS:   String(42); (42).toString()
来源：http://dl.newstarts.cn

TS:   String(42)
来源：http://hz.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zk.asd995.cn

Go:   strconv.Itoa(42)
来源：http://gy.newstarts.cn

Ruby: 42.to_s
来源：http://af.wgjwhj.cn

C#:   42.ToString()
来源：http://mc.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://vf.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uz.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yk.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bn.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://px.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bz.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wn.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://np.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ix.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://ku.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vm.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jt.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vd.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yh.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ol.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dc.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cx.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ya.jctech888.com.cn

[A10] 生成随机数
来源：http://bs.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://bx.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://ov.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rv.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qp.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://gk.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lt.yuexingan06.cn

Ruby: rand(1..100)
来源：http://jj.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://lh.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://uv.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://yj.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rd.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://em.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oc.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://ef.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mh.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nk.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hv.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://wl.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kw.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aj.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://cu.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://on.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ie.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://an.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://og.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://gp.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ey.521024.cn

Py:   "第一行\n第二行"
来源：http://lr.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://kz.huanxung.cn

JS:   "第一行\n第二行"
来源：http://bz.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://zo.shxzskj.cn

Java: "第一行\n第二行"
来源：http://jc.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://zd.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://sn.nicolike.cn

C#:   "第一行\n第二行"
来源：http://qp.jctech888.com.cn

[A14] 注释写法
来源：http://un.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://os.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ur.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://wf.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://kw.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vr.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://xl.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pu.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://jm.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://hv.newstarts.cn

Py:   value = data or "默认值"
来源：http://ck.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://jg.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://un.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://bn.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xq.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://pc.nicolike.cn

Ruby: value = data || "默认值"
来源：http://yt.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://bj.haigaiapp.cn

[A16] 真假值判断规则
来源：http://er.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://re.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ge.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lt.panjiajie.cn

TS:   if (!x) {}
来源：http://sk.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://eu.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mk.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lr.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mb.huanxung.cn

[A17] 位运算
来源：http://ji.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lz.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ax.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rx.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uy.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://om.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ck.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://og.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jg.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://ff.521024.cn

Py:   ord("A"); chr(65)
来源：http://cr.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://sc.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ne.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jl.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ec.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ge.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://rv.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://gh.haigaiapp.cn

[A19] 交换两个变量
来源：http://yv.asd995.cn

Py:   a, b = b, a
来源：http://cy.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pn.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://uv.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://kx.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://zx.shxzskj.cn

Go:   a, b = b, a
来源：http://zv.asd995.cn

Ruby: a, b = b, a
来源：http://zi.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://wo.panjiajie.cn

[A20] 读取标准输入
来源：http://oh.panjiajie.cn

Py:   name = input("请输入：")
来源：http://mv.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zw.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nu.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://vo.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://kd.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nm.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://dk.lnxyls.cn

C#:   Console.ReadLine();
来源：http://uq.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://dk.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://bz.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gy.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://iw.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://lq.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://aw.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://do.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://tf.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://gn.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://jf.gzmigu.cn

Py:   len(s)
来源：http://kh.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yh.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nn.asd995.cn

TS:   s.length
来源：http://fl.huixinmuqiang.cn

Java: s.length()
来源：http://xv.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mi.gzmigu.cn

Ruby: s.length
来源：http://pj.nszjky.cn

C#:   s.Length
来源：http://mb.yuexingan06.cn

[A23] 大小写转换
来源：http://jb.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hm.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://be.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mz.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iy.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qf.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sl.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ef.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dt.chemitech.net.cn

[A24] 去除首尾空白
来源：http://kz.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hw.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rv.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hk.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hv.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yz.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://ot.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mp.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sq.9csxet.cn

[A25] 字符串比较
来源：http://dw.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://wq.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bs.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hq.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qy.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oc.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vp.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wl.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ok.panjiajie.cn

[A26] 类型转换总览
来源：http://kj.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ds.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qg.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ar.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://ya.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fl.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tf.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ht.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oa.chemitech.net.cn

================================================================================
来源：http://qo.521024.cn

B. 流程控制
来源：http://np.nszjky.cn

================================================================================
来源：http://uv.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://ua.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yk.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gg.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pr.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qy.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ee.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ca.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fh.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://no.9csxet.cn

[B02] 多分支 else if / elif
来源：http://vu.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dq.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ud.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uh.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jm.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ir.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ap.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jq.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mu.szsharing.cn

[B03] switch / match / case
来源：http://xc.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fy.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yn.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ft.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cd.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ee.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vf.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zb.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ap.huixiangedu.cn

[B04] for 计数循环
来源：http://vg.521024.cn

Py:   for i in range(10): print(i)
来源：http://ym.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pt.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pk.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nb.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pm.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mg.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://cy.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wg.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://ce.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://ee.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kv.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fw.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vs.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iy.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ub.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://bh.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://du.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://tf.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tc.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qt.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gm.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sh.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ld.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ci.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cr.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ho.huanxung.cn

[B07] while 循环
来源：http://zu.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://lq.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aj.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://sa.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://hg.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://vu.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ku.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://bj.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://rc.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://ne.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://cb.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cb.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://gm.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://xj.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://xh.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ak.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xn.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://vn.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ru.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qn.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tf.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mn.shxzskj.cn


<!-- 参考信息 -->