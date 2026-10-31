代发 wailian999

[A02] 变量声明与赋值
来源：http://pg.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bx.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oc.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xz.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ut.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://ul.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://pd.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://hl.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dy.jctech888.com.cn

[A03] 常量定义
来源：http://uo.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xm.521024.cn

PHP:  const PI = 3.14159;
来源：http://ju.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://lh.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://kv.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://yq.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://cx.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://fx.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://yh.hnjuh.cn

[A04] 判断变量类型
来源：http://xw.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ng.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://em.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jw.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://jq.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vm.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vo.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://aw.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://en.haigaiapp.cn

[A05] 整数除法与取模
来源：http://nj.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kf.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kf.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ao.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cs.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://in.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://ln.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://rq.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://ak.szsharing.cn

[A06] 字符串转数字
来源：http://bn.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://zg.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vi.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rl.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vt.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yt.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ad.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yx.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gs.shtwfgs.cn

[A07] 数字转字符串
来源：http://gu.shtwfgs.cn

Py:   str(42)
来源：http://ir.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://bv.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://el.asd995.cn

TS:   String(42)
来源：http://hb.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uc.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://zb.nicolike.cn

Ruby: 42.to_s
来源：http://ya.wgjwhj.cn

C#:   42.ToString()
来源：http://nc.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://yu.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wr.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bu.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ss.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yz.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dz.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ts.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wi.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sc.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://lh.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ef.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tw.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pk.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zv.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dg.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gp.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ng.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ku.colortex.cn

[A10] 生成随机数
来源：http://ul.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://pt.nszjky.cn

PHP:  random_int(1, 100);
来源：http://sr.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ox.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vs.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://yg.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cm.huixiangedu.cn

Ruby: rand(1..100)
来源：http://bf.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://ic.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://qa.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://ah.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nt.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pc.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xb.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://zo.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gp.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qs.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://un.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://tv.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tf.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ud.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://oo.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://en.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://zn.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wd.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://qc.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://il.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pt.szsharing.cn

Py:   "第一行\n第二行"
来源：http://pr.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://dc.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://ji.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://gs.colortex.cn

Java: "第一行\n第二行"
来源：http://qw.nszjky.cn

Go:   "第一行\n第二行"
来源：http://wc.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://zx.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://ef.szxytkj.cn

[A14] 注释写法
来源：http://vh.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dz.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fa.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://hy.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://tq.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ry.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://wd.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ev.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://kk.shxzukj.cn

[A15] 空值判断与默认值
来源：http://to.shxzskj.cn

Py:   value = data or "默认值"
来源：http://rl.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://ks.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://qx.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://pk.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fa.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://tg.huanxung.cn

Ruby: value = data || "默认值"
来源：http://kh.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://fh.newstarts.cn

[A16] 真假值判断规则
来源：http://mk.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eq.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sr.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ug.shtwfgs.cn

TS:   if (!x) {}
来源：http://jw.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fp.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ye.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vi.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lf.huanxung.cn

[A17] 位运算
来源：http://av.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kt.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mc.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://on.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yr.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yc.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mj.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mu.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fb.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://vd.colortex.cn

Py:   ord("A"); chr(65)
来源：http://he.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://im.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gq.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ji.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://yt.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://or.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://uq.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://qc.hnjuh.cn

[A19] 交换两个变量
来源：http://by.asd995.cn

Py:   a, b = b, a
来源：http://az.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ph.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://oc.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://wn.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://oh.muxihuayi.cn

Go:   a, b = b, a
来源：http://po.wgjwhj.cn

Ruby: a, b = b, a
来源：http://eg.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://gn.hnjuh.cn

[A20] 读取标准输入
来源：http://dt.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://lm.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mk.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xq.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://nu.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://di.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ep.bjjhwx.cn

Ruby: gets.chomp
来源：http://hd.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://qw.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://sb.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://kq.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://be.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://je.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://hi.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://om.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xb.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://xu.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://mp.nicolike.cn

[A22] 获取字符串长度
来源：http://mk.shxzukj.cn

Py:   len(s)
来源：http://ab.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zj.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ls.yuntaijiaju.cn

TS:   s.length
来源：http://ef.yuntaijiaju.cn

Java: s.length()
来源：http://gi.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ta.bookmarksfly.cn

Ruby: s.length
来源：http://ze.yuexingan06.cn

C#:   s.Length
来源：http://ui.yuexingan06.cn

[A23] 大小写转换
来源：http://cp.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zi.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ru.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kp.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cw.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gh.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aw.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dx.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jb.wgjwhj.cn

[A24] 去除首尾空白
来源：http://qp.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gs.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kx.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://js.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xw.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jy.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://ud.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ml.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eo.haigaiapp.cn

[A25] 字符串比较
来源：http://mo.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://ux.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jk.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ye.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zd.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fc.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zp.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://in.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wp.bjjhwx.cn

[A26] 类型转换总览
来源：http://dm.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hc.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wg.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vv.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://ds.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wl.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ay.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ly.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qy.bjjhwx.cn

================================================================================
来源：http://fj.shxzskj.cn

B. 流程控制
来源：http://zn.panjiajie.cn

================================================================================
来源：http://nb.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://iz.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hl.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ic.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ti.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tf.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uy.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fq.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qp.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ne.hahajie.cn

[B02] 多分支 else if / elif
来源：http://cu.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ot.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://be.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yt.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://py.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uk.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ri.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hs.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fo.huixiangedu.cn

[B03] switch / match / case
来源：http://lm.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iu.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dm.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dx.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://du.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rm.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fi.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dl.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fu.szsharing.cn

[B04] for 计数循环
来源：http://bk.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://zu.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hl.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jq.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gx.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://up.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zh.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://fn.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eg.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://wo.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://ti.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oo.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nq.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kl.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xj.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qt.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://vk.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cu.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://hg.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ce.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dh.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uc.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bj.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sg.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rh.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cj.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zm.9csxet.cn

[B07] while 循环
来源：http://sq.szsharing.cn

Py:   while i < 10: i += 1
来源：http://qk.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://op.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://ra.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://ef.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://lg.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pt.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://ef.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://nt.521024.cn

[B08] do-while（至少执行一次）
来源：http://mv.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://cf.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kg.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://vb.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://vt.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://jm.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ry.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ym.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://kt.nicolike.cn


<!-- 参考信息 -->