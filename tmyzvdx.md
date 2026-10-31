代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://br.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xe.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://jf.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dq.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vh.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fp.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://wp.huanxung.cn

[A05] 整数除法与取模
来源：http://dc.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jg.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vd.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://el.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ra.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://kr.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://pg.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://me.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://vh.colortex.cn

[A06] 字符串转数字
来源：http://hl.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://kb.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wm.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://il.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tw.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gt.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://km.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ze.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mn.bookmarksfly.cn

[A07] 数字转字符串
来源：http://tt.nszjky.cn

Py:   str(42)
来源：http://yk.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://pp.hahajie.cn

JS:   String(42); (42).toString()
来源：http://cy.wgjwhj.cn

TS:   String(42)
来源：http://qn.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pb.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://kq.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://cg.muxihuayi.cn

C#:   42.ToString()
来源：http://lb.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://gt.chemitech.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bf.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gr.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qq.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iy.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vf.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hw.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pq.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hd.asd995.cn

[A09] 绝对值与最大最小值
来源：http://ck.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zf.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gw.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wc.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ww.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xi.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bz.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ln.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://no.asd995.cn

[A10] 生成随机数
来源：http://nk.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://de.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://fl.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://js.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vd.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://af.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dx.hahajie.cn

Ruby: rand(1..100)
来源：http://vw.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://ff.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://nx.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://rz.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wl.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://km.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zf.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://zf.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wz.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bb.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tn.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://mb.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hq.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rk.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://rc.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://aw.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://ro.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hv.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://xt.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://aq.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zf.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://om.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://gx.szsharing.cn

JS:   "第一行\n第二行"
来源：http://om.asd995.cn

TS:   "第一行\n第二行"
来源：http://ht.nicolike.cn

Java: "第一行\n第二行"
来源：http://ai.9csxet.cn

Go:   "第一行\n第二行"
来源：http://ok.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://ei.nszjky.cn

C#:   "第一行\n第二行"
来源：http://le.chemitech.net.cn

[A14] 注释写法
来源：http://wj.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ah.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ib.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://ed.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://th.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zm.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://sx.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nh.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://ey.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://sa.szxytkj.cn

Py:   value = data or "默认值"
来源：http://xs.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://kx.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://dg.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://nn.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zh.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://ul.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://fu.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://vt.wgjwhj.cn

[A16] 真假值判断规则
来源：http://xe.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xv.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lo.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rx.bjjhwx.cn

TS:   if (!x) {}
来源：http://to.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oz.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fj.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qt.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qq.nszjky.cn

[A17] 位运算
来源：http://pz.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://an.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gv.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fz.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fd.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://no.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dd.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pl.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://mh.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://fp.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://nv.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lx.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://la.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://uy.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ib.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://rh.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://fh.hnjuh.cn

[A19] 交换两个变量
来源：http://hf.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://sb.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qe.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://vb.521024.cn

TS:   [a, b] = [b, a];
来源：http://ap.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://vl.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://vy.shxzskj.cn

Ruby: a, b = b, a
来源：http://yt.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://fy.panjiajie.cn

[A20] 读取标准输入
来源：http://pp.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://jp.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gv.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xb.colortex.cn

TS:   // Node.js：readline 模块
来源：http://oc.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://bq.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ik.huixiangedu.cn

Ruby: gets.chomp
来源：http://fj.nicolike.cn

C#:   Console.ReadLine();
来源：http://dx.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://iv.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://op.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xu.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://ra.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://te.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://rl.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dw.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://ph.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://ds.lnxyls.cn

[A22] 获取字符串长度
来源：http://wb.nicolike.cn

Py:   len(s)
来源：http://au.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hb.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://td.gzmigu.cn

TS:   s.length
来源：http://yj.szxytkj.cn

Java: s.length()
来源：http://lb.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lv.haigaiapp.cn

Ruby: s.length
来源：http://ee.shtwfgs.cn

C#:   s.Length
来源：http://fz.521024.cn

[A23] 大小写转换
来源：http://pt.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oa.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bh.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xt.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wt.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://db.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rt.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pz.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cj.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://zy.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wd.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kj.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ry.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ta.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gp.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://bz.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yo.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wx.colortex.cn

[A25] 字符串比较
来源：http://aw.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://kh.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nm.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ig.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ch.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zk.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rz.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://me.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yc.haigaiapp.cn

[A26] 类型转换总览
来源：http://mq.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bb.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ry.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jl.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://eo.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fj.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rl.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fu.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tj.lnxyls.cn

================================================================================
来源：http://ib.nszjky.cn

B. 流程控制
来源：http://lm.nicolike.cn

================================================================================
来源：http://if.hnjuh.cn

[B01] 条件判断 if / else
来源：http://wk.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://my.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bg.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ab.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ix.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cb.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dx.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pw.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wo.nicolike.cn

[B02] 多分支 else if / elif
来源：http://io.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://go.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zq.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xv.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wo.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nl.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qe.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dp.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qy.shxzskj.cn

[B03] switch / match / case
来源：http://ze.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nz.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zj.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tw.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vv.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vo.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gh.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fj.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://no.nszjky.cn

[B04] for 计数循环
来源：http://cn.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://nf.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cx.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yz.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rq.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vc.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zt.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://kz.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iy.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://ll.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://iw.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ly.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nl.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rf.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ca.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tu.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://hl.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xu.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://cz.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ta.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vk.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gu.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://et.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qx.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lr.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xd.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://an.hnjuh.cn

[B07] while 循环
来源：http://vf.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://ht.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cf.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://zk.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://xd.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://mf.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mu.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://cu.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://im.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://tf.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://wy.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://he.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://nq.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://hq.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://eo.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wo.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oe.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://bp.yuntaijiaju.cn

[B09] break 与 continue
来源：http://je.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uw.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yi.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zj.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hr.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://db.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vj.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qv.9csxet.cn

[B10] 遍历同时拿索引
来源：http://hz.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qj.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pw.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dg.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cf.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ov.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jz.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ob.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yo.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://vt.521024.cn

Py:   list(range(0, 10, 2))
来源：http://ti.9csxet.cn


<!-- 参考信息 -->