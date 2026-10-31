代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://tr.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://iu.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://fe.9csxet.cn

[A05] 整数除法与取模
来源：http://jp.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vq.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ba.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qw.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ha.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://iy.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://ys.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://vh.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://ui.shxzskj.cn

[A06] 字符串转数字
来源：http://oh.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://jh.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dp.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pw.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dq.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://of.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bn.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kx.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dw.521024.cn

[A07] 数字转字符串
来源：http://kg.shtwfgs.cn

Py:   str(42)
来源：http://qq.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://tp.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://vh.shxzskj.cn

TS:   String(42)
来源：http://hx.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ax.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://pp.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://iq.szsharing.cn

C#:   42.ToString()
来源：http://aw.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://ap.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pk.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pb.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eh.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nf.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://js.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lo.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sp.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mf.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://zg.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ef.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xc.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ww.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ge.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://st.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ee.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ks.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bz.jianghongdianzi.cn

[A10] 生成随机数
来源：http://la.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://wz.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://xl.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eb.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dl.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://qe.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gf.wgjwhj.cn

Ruby: rand(1..100)
来源：http://ig.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://ju.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://bf.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://mn.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fi.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fj.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://og.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://cj.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xw.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zl.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hz.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://wu.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xz.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hm.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://vl.asd995.cn

TS:   `Hello, ${name}!`
来源：http://qf.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://kc.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qi.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://mf.521024.cn

C#:   $"Hello, {name}!"
来源：http://cv.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lh.huanxung.cn

Py:   "第一行\n第二行"
来源：http://uf.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://dv.szsharing.cn

JS:   "第一行\n第二行"
来源：http://fj.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://rd.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://ng.szsharing.cn

Go:   "第一行\n第二行"
来源：http://xk.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://qs.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://go.haigaiapp.cn

[A14] 注释写法
来源：http://is.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kz.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jy.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://ix.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://qp.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tq.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://yo.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jq.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://cn.newstarts.cn

[A15] 空值判断与默认值
来源：http://dz.newstarts.cn

Py:   value = data or "默认值"
来源：http://tg.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://tu.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://tc.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://uh.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iy.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://ud.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://ny.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://wy.lnxyls.cn

[A16] 真假值判断规则
来源：http://fu.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bb.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ar.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jd.huixiangedu.cn

TS:   if (!x) {}
来源：http://rk.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rs.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rl.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fc.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mu.shxzskj.cn

[A17] 位运算
来源：http://wx.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mz.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uu.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fa.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vf.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://br.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zw.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zf.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xp.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://cu.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://uc.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://tl.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yx.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ts.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://ty.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xk.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://ll.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://nx.jctech888.com.cn

[A19] 交换两个变量
来源：http://sp.muxihuayi.cn

Py:   a, b = b, a
来源：http://do.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jv.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://ui.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://mv.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://ss.szxytkj.cn

Go:   a, b = b, a
来源：http://aq.szxytkj.cn

Ruby: a, b = b, a
来源：http://xc.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://os.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://il.panjiajie.cn

Py:   name = input("请输入：")
来源：http://nx.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://it.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zx.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://ue.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://wt.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ed.9csxet.cn

Ruby: gets.chomp
来源：http://lc.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://pw.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://us.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://wb.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zf.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://au.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://cy.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://un.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yq.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://mw.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://hm.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://gk.yuexingan06.cn

Py:   len(s)
来源：http://qh.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fu.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gt.shxzskj.cn

TS:   s.length
来源：http://vf.wgjwhj.cn

Java: s.length()
来源：http://rj.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ri.chemitech.net.cn

Ruby: s.length
来源：http://uq.shtwfgs.cn

C#:   s.Length
来源：http://id.wgjwhj.cn

[A23] 大小写转换
来源：http://el.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vo.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cx.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hd.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ic.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nx.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eg.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cl.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fe.huixiangedu.cn

[A24] 去除首尾空白
来源：http://lc.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mi.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pb.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fx.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://io.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iz.521024.cn

Go:   strings.TrimSpace(s)
来源：http://qx.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kr.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cu.gzmigu.cn

[A25] 字符串比较
来源：http://ar.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://tl.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ra.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ln.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nc.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mi.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dq.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gn.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xf.nszjky.cn

[A26] 类型转换总览
来源：http://np.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wp.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tq.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pn.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://om.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zw.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kn.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bs.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xs.yuntaijiaju.cn

================================================================================
来源：http://gp.9csxet.cn

B. 流程控制
来源：http://hy.hahajie.cn

================================================================================
来源：http://pa.521024.cn

[B01] 条件判断 if / else
来源：http://vm.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gd.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vi.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rm.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pk.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ro.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fh.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ce.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://de.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://jp.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://se.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oz.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gs.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gm.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mu.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ha.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dv.hahajie.cn

[B03] switch / match / case
来源：http://oy.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sn.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hx.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cy.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hk.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ry.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yy.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yi.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pk.huixiangedu.cn

[B04] for 计数循环
来源：http://mp.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://rd.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ph.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tk.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mr.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jd.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dz.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://qk.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ij.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://hb.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://sf.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zy.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kx.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ay.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rj.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ib.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://ls.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yy.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://wu.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ot.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qo.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vj.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nv.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wr.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nr.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nj.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aw.hnjuh.cn

[B07] while 循环
来源：http://cg.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://lb.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qv.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://uh.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://cd.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://lp.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cp.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://yu.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://dt.521024.cn

[B08] do-while（至少执行一次）
来源：http://qt.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://hs.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jo.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://of.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://bv.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://mi.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://se.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yr.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://ez.jctech888.com.cn

[B09] break 与 continue
来源：http://iy.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nc.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fy.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dt.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dk.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dm.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ts.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fn.521024.cn

[B10] 遍历同时拿索引
来源：http://rv.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hg.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pp.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sg.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sf.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kx.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bo.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://af.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cm.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://ej.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://cv.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://vn.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oi.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vn.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wq.panjiajie.cn


<!-- 参考信息 -->