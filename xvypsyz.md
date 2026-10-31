代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wa.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ew.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://of.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ml.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://tg.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://ww.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://bg.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://co.shtwfgs.cn

[A06] 字符串转数字
来源：http://ql.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://ge.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ny.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sj.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qe.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sl.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ke.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sd.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uw.chemitech.net.cn

[A07] 数字转字符串
来源：http://rf.shtwfgs.cn

Py:   str(42)
来源：http://jn.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://cg.szsharing.cn

JS:   String(42); (42).toString()
来源：http://gf.yuntaijiaju.cn

TS:   String(42)
来源：http://ej.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ru.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://bw.colortex.cn

Ruby: 42.to_s
来源：http://ux.yuexingan06.cn

C#:   42.ToString()
来源：http://vj.lnxyls.cn

[A08] 取整与四舍五入
来源：http://aj.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jg.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yh.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mo.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yv.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://py.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sn.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://je.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gv.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://iw.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kj.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xn.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cj.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kd.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ho.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jn.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qt.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bj.yuexingan06.cn

[A10] 生成随机数
来源：http://ib.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://jx.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://kj.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cm.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bq.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://qy.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xu.jctech888.com.cn

Ruby: rand(1..100)
来源：http://hw.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://jx.521024.cn

[A11] 条件表达式（三元）
来源：http://wj.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://da.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ln.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ud.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hj.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://nn.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://as.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bh.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nv.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://hx.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ti.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://if.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://tr.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://lo.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://nh.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lo.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://aa.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://gk.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gm.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://jq.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://rw.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://as.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://nt.shxzskj.cn

Java: "第一行\n第二行"
来源：http://kt.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://ig.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://xw.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://mg.jianghongdianzi.cn

[A14] 注释写法
来源：http://rg.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hx.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ew.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://wk.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://dr.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kh.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://ds.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bo.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://oc.szxytkj.cn

[A15] 空值判断与默认值
来源：http://ka.colortex.cn

Py:   value = data or "默认值"
来源：http://gb.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://qg.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://st.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://lo.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sa.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://nq.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://oh.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://tl.chemitech.net.cn

[A16] 真假值判断规则
来源：http://za.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://us.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://id.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lm.bookmarksfly.cn

TS:   if (!x) {}
来源：http://on.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ov.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ew.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vg.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bx.huixiangedu.cn

[A17] 位运算
来源：http://ow.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ev.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vf.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jr.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wh.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dq.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lc.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tn.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eo.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://qo.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://xq.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://fx.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jy.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tm.521024.cn

Java: (int) 'A'; (char) 65
来源：http://aa.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xb.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://jc.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://wi.huixiangedu.cn

[A19] 交换两个变量
来源：http://rr.chemitech.net.cn

Py:   a, b = b, a
来源：http://xk.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fl.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://ct.asd995.cn

TS:   [a, b] = [b, a];
来源：http://fl.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://gu.colortex.cn

Go:   a, b = b, a
来源：http://td.nszjky.cn

Ruby: a, b = b, a
来源：http://vr.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://zm.wgjwhj.cn

[A20] 读取标准输入
来源：http://os.szxytkj.cn

Py:   name = input("请输入：")
来源：http://wk.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jy.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wd.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://fu.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://uv.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dm.haigaiapp.cn

Ruby: gets.chomp
来源：http://kw.9csxet.cn

C#:   Console.ReadLine();
来源：http://oj.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://nq.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://hq.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://un.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://eg.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://xm.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://qd.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lw.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://uw.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://wf.haigaiapp.cn

[A22] 获取字符串长度
来源：http://ts.nicolike.cn

Py:   len(s)
来源：http://tp.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://or.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ea.nicolike.cn

TS:   s.length
来源：http://dd.jianghongdianzi.cn

Java: s.length()
来源：http://ae.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zo.nicolike.cn

Ruby: s.length
来源：http://lo.hahajie.cn

C#:   s.Length
来源：http://bm.bookmarksfly.cn

[A23] 大小写转换
来源：http://mc.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://av.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eb.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ej.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zx.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qh.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mi.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rk.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zi.newstarts.cn

[A24] 去除首尾空白
来源：http://hk.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://us.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pl.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vi.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lz.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xb.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://ss.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xm.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hq.gzmigu.cn

[A25] 字符串比较
来源：http://ja.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://dy.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zy.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cq.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gl.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://go.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pf.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vm.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vx.szsharing.cn

[A26] 类型转换总览
来源：http://ks.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://is.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ro.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ni.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://ff.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cy.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pe.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zp.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ux.yuntaijiaju.cn

================================================================================
来源：http://iz.colortex.cn

B. 流程控制
来源：http://tl.521024.cn

================================================================================
来源：http://wm.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://sa.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://po.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mo.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pv.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rn.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iw.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qy.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hd.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xk.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://mh.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cx.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yb.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://an.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ow.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fm.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ky.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ln.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hr.szsharing.cn

[B03] switch / match / case
来源：http://cf.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jn.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dl.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://am.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vi.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aw.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wp.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://km.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://na.bookmarksfly.cn

[B04] for 计数循环
来源：http://yz.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://ue.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ef.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ha.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://by.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dx.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://on.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://ae.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://im.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://rw.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://vr.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ky.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wl.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rn.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oq.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://to.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://ie.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vc.521024.cn

[B06] 遍历字典 / 对象
来源：http://gi.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zc.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://md.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mj.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ce.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ny.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eu.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iz.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bx.521024.cn

[B07] while 循环
来源：http://it.nicolike.cn

Py:   while i < 10: i += 1
来源：http://jd.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rb.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://eb.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://dy.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://xh.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rz.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://fh.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://dr.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://do.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://zc.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ma.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://vi.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://et.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://ru.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xj.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zg.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://kb.huixinmuqiang.cn

[B09] break 与 continue
来源：http://vx.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hl.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://np.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dx.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sy.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://px.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vs.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iz.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://it.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hg.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zr.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pt.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mf.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tt.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vf.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fc.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ci.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://ma.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://cr.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://cg.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ag.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fw.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hb.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pt.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://tj.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bb.huanxung.cn

[B12] 跳出多层循环
来源：http://qd.gzmigu.cn


<!-- 参考信息 -->