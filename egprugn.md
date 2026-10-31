代发 wailian999

[A02] 变量声明与赋值
来源：http://rr.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pv.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uv.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://to.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://km.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://fb.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://rf.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://jx.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://db.hahajie.cn

[A03] 常量定义
来源：http://ib.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lu.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://bt.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://da.521024.cn

TS:   const PI: number = 3.14159;
来源：http://sp.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://ak.9csxet.cn

Go:   const PI = 3.14159
来源：http://qh.gzmigu.cn

Ruby: PI = 3.14159
来源：http://ag.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://wq.szxytkj.cn

[A04] 判断变量类型
来源：http://fo.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ke.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dp.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ii.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://cb.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vh.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qm.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cz.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://ev.hnjuh.cn

[A05] 整数除法与取模
来源：http://cv.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://en.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://si.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fr.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tv.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://mo.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://zk.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://hm.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://pb.chemitech.net.cn

[A06] 字符串转数字
来源：http://hk.521024.cn

Py:   int("42"); float("3.14")
来源：http://lw.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pr.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rq.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dc.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fi.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ab.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sc.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mz.szsharing.cn

[A07] 数字转字符串
来源：http://rk.nicolike.cn

Py:   str(42)
来源：http://fo.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://zl.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://wu.colortex.cn

TS:   String(42)
来源：http://yy.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gf.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://rm.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://nf.bookmarksfly.cn

C#:   42.ToString()
来源：http://li.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://nh.chemitech.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ar.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ts.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ma.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yg.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cy.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yh.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cw.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gj.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://qs.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://on.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nf.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qc.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wl.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ld.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pk.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xz.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jg.panjiajie.cn

[A10] 生成随机数
来源：http://un.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://mz.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://kw.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jb.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pn.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://eu.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://iy.szsharing.cn

Ruby: rand(1..100)
来源：http://vn.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://lt.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://zv.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://kb.jianghongdianzi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jp.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ju.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jw.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://lp.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eu.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dp.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://da.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://ge.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://en.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qa.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://qb.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://nr.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://kz.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qj.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://xv.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://ng.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jo.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://ug.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://su.szsharing.cn

JS:   "第一行\n第二行"
来源：http://wp.colortex.cn

TS:   "第一行\n第二行"
来源：http://ud.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://in.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://rw.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://hb.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://tu.nszjky.cn

[A14] 注释写法
来源：http://ae.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ao.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hb.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://ny.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://ui.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vy.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://gt.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qw.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://og.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://xh.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://rf.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://ko.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://re.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://kg.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pp.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://ym.521024.cn

Ruby: value = data || "默认值"
来源：http://xz.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://kl.nicolike.cn

[A16] 真假值判断规则
来源：http://yd.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tj.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ll.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oe.wgjwhj.cn

TS:   if (!x) {}
来源：http://vp.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ma.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yl.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ga.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aj.wgjwhj.cn

[A17] 位运算
来源：http://xi.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mf.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vl.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uj.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nf.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ns.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yc.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bq.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ho.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://xb.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://ok.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://sc.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://el.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qe.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://bg.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lu.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://aj.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://zs.nszjky.cn

[A19] 交换两个变量
来源：http://pa.wgjwhj.cn

Py:   a, b = b, a
来源：http://fz.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sh.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://nv.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://eq.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://ru.newstarts.cn

Go:   a, b = b, a
来源：http://ts.szxytkj.cn

Ruby: a, b = b, a
来源：http://am.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://hr.huixiangedu.cn

[A20] 读取标准输入
来源：http://sa.shxzukj.cn

Py:   name = input("请输入：")
来源：http://bp.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ls.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ji.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://yv.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://ia.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wr.bjjhwx.cn

Ruby: gets.chomp
来源：http://bm.asd995.cn

C#:   Console.ReadLine();
来源：http://xv.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://vi.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://fw.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ei.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://xm.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://iy.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://qf.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://th.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://jq.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://ug.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://hb.asd995.cn

Py:   len(s)
来源：http://wo.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sd.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://av.huixiangedu.cn

TS:   s.length
来源：http://mz.521024.cn

Java: s.length()
来源：http://go.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ot.wgjwhj.cn

Ruby: s.length
来源：http://nc.shxzskj.cn

C#:   s.Length
来源：http://ot.szxytkj.cn

[A23] 大小写转换
来源：http://xx.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://md.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pv.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iv.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oe.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ph.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bs.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eu.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kk.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://ke.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sl.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bm.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fz.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dq.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://um.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://ly.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eh.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kf.chemitech.net.cn

[A25] 字符串比较
来源：http://vm.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://ge.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ou.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yt.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kw.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qd.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fc.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hf.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ib.szsharing.cn

[A26] 类型转换总览
来源：http://qi.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://us.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://za.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rm.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://lz.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://db.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://da.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tz.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vb.shxzskj.cn

================================================================================
来源：http://vf.jctech888.com.cn

B. 流程控制
来源：http://eh.yuexingan06.cn

================================================================================
来源：http://mu.hnjuh.cn

[B01] 条件判断 if / else
来源：http://tx.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rh.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mk.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mf.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vl.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ee.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ek.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rb.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gg.huanxung.cn

[B02] 多分支 else if / elif
来源：http://ls.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rb.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xk.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xp.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iu.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yd.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tn.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oa.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xx.hahajie.cn

[B03] switch / match / case
来源：http://je.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tu.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sa.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gt.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bt.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fh.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qb.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xr.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://my.nszjky.cn

[B04] for 计数循环
来源：http://cp.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://bm.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ey.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mf.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vo.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wn.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ml.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://qj.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yb.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://ty.hahajie.cn

Py:   for item in arr: print(item)
来源：http://ow.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qd.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://st.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lo.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nv.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yp.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://gs.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ns.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://va.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xg.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kz.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sv.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gi.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://il.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ze.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kq.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jd.colortex.cn

[B07] while 循环
来源：http://yh.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://sk.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zq.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://fv.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://nr.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://qg.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nd.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://tk.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://lh.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://eg.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://bj.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cf.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://wk.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://qk.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://sh.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mu.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ha.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://oj.yuexingan06.cn


<!-- 参考信息 -->