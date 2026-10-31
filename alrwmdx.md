代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jg.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cw.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hf.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://os.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://wm.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://fb.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://vb.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://gv.hahajie.cn

[A06] 字符串转数字
来源：http://ar.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://ib.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rx.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uh.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://up.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kb.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gc.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tq.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fv.bookmarksfly.cn

[A07] 数字转字符串
来源：http://cg.shxzukj.cn

Py:   str(42)
来源：http://eo.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://aq.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://bm.huixiangedu.cn

TS:   String(42)
来源：http://ju.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ta.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://be.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://il.haigaiapp.cn

C#:   42.ToString()
来源：http://ft.nicolike.cn

[A08] 取整与四舍五入
来源：http://el.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sd.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://im.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lt.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qp.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bl.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xp.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pf.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fc.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://rz.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hg.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yy.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vt.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ts.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uu.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ur.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cy.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ds.hnjuh.cn

[A10] 生成随机数
来源：http://vj.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://ki.szsharing.cn

PHP:  random_int(1, 100);
来源：http://ax.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hv.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wa.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://hc.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://um.szxytkj.cn

Ruby: rand(1..100)
来源：http://wk.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://jd.hahajie.cn

[A11] 条件表达式（三元）
来源：http://bs.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://pf.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dw.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ed.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ah.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://vs.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hi.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kk.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ji.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://cc.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jn.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tf.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://jc.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://mj.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://rq.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xa.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ck.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://di.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gt.hahajie.cn

Py:   "第一行\n第二行"
来源：http://nx.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://vu.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://tg.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://dk.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://wl.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://pg.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://di.521024.cn

C#:   "第一行\n第二行"
来源：http://qq.panjiajie.cn

[A14] 注释写法
来源：http://lg.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bv.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://db.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://dp.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://be.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yp.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://cf.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fc.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://rj.asd995.cn

[A15] 空值判断与默认值
来源：http://wb.szxytkj.cn

Py:   value = data or "默认值"
来源：http://ox.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://wf.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://qd.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://ni.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bc.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://aw.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://ub.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://ff.521024.cn

[A16] 真假值判断规则
来源：http://uq.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ip.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bf.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gr.wgjwhj.cn

TS:   if (!x) {}
来源：http://fm.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mv.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lc.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yi.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ig.huixinmuqiang.cn

[A17] 位运算
来源：http://pu.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kn.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://as.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://un.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fq.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://na.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mp.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bj.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fc.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://sh.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://zp.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://pi.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zr.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nd.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://ap.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xz.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://hp.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://aj.chemitech.net.cn

[A19] 交换两个变量
来源：http://ye.jctech888.com.cn

Py:   a, b = b, a
来源：http://dg.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ud.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://ej.521024.cn

TS:   [a, b] = [b, a];
来源：http://is.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://hj.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://uq.9csxet.cn

Ruby: a, b = b, a
来源：http://xv.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://yw.chemitech.net.cn

[A20] 读取标准输入
来源：http://sk.hnjuh.cn

Py:   name = input("请输入：")
来源：http://qf.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pf.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yz.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://se.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://na.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bf.colortex.cn

Ruby: gets.chomp
来源：http://rb.shxzskj.cn

C#:   Console.ReadLine();
来源：http://fq.colortex.cn

[A21] 保留指定小数位输出
来源：http://uy.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://yg.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xk.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://jo.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://px.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://hn.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ez.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://zt.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://ke.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://wk.bjjhwx.cn

Py:   len(s)
来源：http://xk.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gt.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xi.9csxet.cn

TS:   s.length
来源：http://lr.chemitech.net.cn

Java: s.length()
来源：http://yu.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eg.huixiangedu.cn

Ruby: s.length
来源：http://cn.yuntaijiaju.cn

C#:   s.Length
来源：http://qj.asd995.cn

[A23] 大小写转换
来源：http://gi.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wy.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fo.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cj.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ad.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wc.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ug.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eb.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ik.szsharing.cn

[A24] 去除首尾空白
来源：http://dp.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zb.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hx.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qq.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nu.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gt.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://hi.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ms.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pp.huixinmuqiang.cn

[A25] 字符串比较
来源：http://yk.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://yp.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fz.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oq.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zl.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zm.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://be.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mb.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bp.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://cb.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dl.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mk.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lm.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://lv.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tu.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xe.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wx.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xk.hnjuh.cn

================================================================================
来源：http://vt.shxzskj.cn

B. 流程控制
来源：http://pj.lnxyls.cn

================================================================================
来源：http://vs.panjiajie.cn

[B01] 条件判断 if / else
来源：http://ve.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gb.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qv.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vy.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ad.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ul.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tn.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lp.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bt.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://nt.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fh.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ta.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dj.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ik.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qn.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wn.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bk.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hr.gzmigu.cn

[B03] switch / match / case
来源：http://fh.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sw.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xt.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zn.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ud.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eg.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fj.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yi.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gj.newstarts.cn

[B04] for 计数循环
来源：http://vi.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://ip.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kh.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ed.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ju.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lp.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vb.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://fs.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uo.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://sp.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://zk.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nd.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pt.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ky.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qr.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qo.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://gx.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ia.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://gn.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dm.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hj.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ap.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vv.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kc.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fq.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ph.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yo.yuexingan06.cn

[B07] while 循环
来源：http://kz.szsharing.cn

Py:   while i < 10: i += 1
来源：http://ek.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ad.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://hb.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://gy.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://go.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://va.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://bo.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://jw.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://tl.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://km.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://co.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://ve.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://sr.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://gf.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ha.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nw.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://rh.shxzukj.cn

[B09] break 与 continue
来源：http://km.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://es.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lq.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zd.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ox.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yd.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cg.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jg.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ny.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://rr.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vf.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ta.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tl.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ai.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://os.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ct.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://el.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pm.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://wd.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://no.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://tl.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hb.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fd.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zn.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xm.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://ir.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pm.szsharing.cn

[B12] 跳出多层循环
来源：http://gl.bookmarksfly.cn


<!-- 参考信息 -->