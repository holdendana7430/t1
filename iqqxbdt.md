代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gk.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gu.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qu.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://un.nicolike.cn

Java: 7 / 2; 7 % 2
来源：http://ap.521024.cn

Go:   7 / 2; 7 % 2
来源：http://sb.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://jb.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://py.nszjky.cn

[A06] 字符串转数字
来源：http://tb.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://pi.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://il.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ad.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qv.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kp.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://te.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sf.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mr.colortex.cn

[A07] 数字转字符串
来源：http://dn.521024.cn

Py:   str(42)
来源：http://cg.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://zr.colortex.cn

JS:   String(42); (42).toString()
来源：http://nj.shtwfgs.cn

TS:   String(42)
来源：http://qn.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qe.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://ww.lnxyls.cn

Ruby: 42.to_s
来源：http://uy.newstarts.cn

C#:   42.ToString()
来源：http://vg.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://ej.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mj.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hy.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://we.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vo.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://or.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kw.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sd.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xe.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://ib.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ea.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://po.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://if.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mh.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ia.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ro.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gg.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pr.shxzskj.cn

[A10] 生成随机数
来源：http://aq.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://tt.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://of.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nt.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cr.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://sq.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xv.wgjwhj.cn

Ruby: rand(1..100)
来源：http://ts.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://xu.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://rd.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://ki.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://or.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sl.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://la.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://wu.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://om.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sl.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vw.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://dn.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gj.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cc.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://kb.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://ez.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://vo.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ek.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://ez.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://tq.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jc.521024.cn

Py:   "第一行\n第二行"
来源：http://vs.colortex.cn

PHP:  "第一行\n第二行"
来源：http://cs.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://vh.9csxet.cn

TS:   "第一行\n第二行"
来源：http://nx.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://hs.colortex.cn

Go:   "第一行\n第二行"
来源：http://yn.colortex.cn

Ruby: "第一行\n第二行"
来源：http://lp.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://ke.nszjky.cn

[A14] 注释写法
来源：http://rc.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qd.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jp.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://dp.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://np.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xv.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://og.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://iy.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://jg.panjiajie.cn

[A15] 空值判断与默认值
来源：http://ln.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://ke.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ys.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://px.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://ag.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oz.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://gq.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://hp.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://sy.521024.cn

[A16] 真假值判断规则
来源：http://bb.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ii.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ba.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sc.nszjky.cn

TS:   if (!x) {}
来源：http://yi.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qa.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kj.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hr.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uq.nszjky.cn

[A17] 位运算
来源：http://tk.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sz.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xs.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eq.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vz.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sx.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bl.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://en.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://gm.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://bl.521024.cn

PHP:  ord("A"); chr(65)
来源：http://bn.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mo.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ib.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://mu.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rz.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://mr.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://nw.huixiangedu.cn

[A19] 交换两个变量
来源：http://cs.szxytkj.cn

Py:   a, b = b, a
来源：http://sf.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ga.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://ph.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://oz.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://sp.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://mx.haigaiapp.cn

Ruby: a, b = b, a
来源：http://vl.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://pm.lnxyls.cn

[A20] 读取标准输入
来源：http://zv.szxytkj.cn

Py:   name = input("请输入：")
来源：http://xa.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tx.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://en.colortex.cn

TS:   // Node.js：readline 模块
来源：http://sy.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://gr.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vl.nicolike.cn

Ruby: gets.chomp
来源：http://eg.9csxet.cn

C#:   Console.ReadLine();
来源：http://gj.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://ji.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://pu.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ke.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://uo.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://th.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://nw.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gc.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://al.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://pz.jctech888.com.cn

[A22] 获取字符串长度
来源：http://sf.yuntaijiaju.cn

Py:   len(s)
来源：http://go.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ox.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tj.jianghongdianzi.cn

TS:   s.length
来源：http://qx.wgjwhj.cn

Java: s.length()
来源：http://km.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cl.jctech888.com.cn

Ruby: s.length
来源：http://wu.yuexingan06.cn

C#:   s.Length
来源：http://en.chemitech.net.cn

[A23] 大小写转换
来源：http://rj.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vr.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kz.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ho.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://df.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zd.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uu.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ob.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ep.asd995.cn

[A24] 去除首尾空白
来源：http://fr.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aq.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ym.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wv.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://an.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fr.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://zk.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pe.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yq.colortex.cn

[A25] 字符串比较
来源：http://mc.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://xm.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ap.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bl.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://es.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ut.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://us.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gw.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ki.muxihuayi.cn

[A26] 类型转换总览
来源：http://wu.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tc.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rb.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wn.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://ud.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cx.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bf.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pz.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jq.szsharing.cn

================================================================================
来源：http://fe.gzmigu.cn

B. 流程控制
来源：http://dm.nszjky.cn

================================================================================
来源：http://by.shxzukj.cn

[B01] 条件判断 if / else
来源：http://ss.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://is.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yn.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uo.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xk.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rf.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gt.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eb.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://va.asd995.cn

[B02] 多分支 else if / elif
来源：http://yd.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ch.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pb.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://et.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fj.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vu.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rz.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://es.szxytkj.cn

[B03] switch / match / case
来源：http://ix.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oc.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ed.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://um.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ur.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ej.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vt.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qq.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bi.9csxet.cn

[B04] for 计数循环
来源：http://mq.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://qf.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://au.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lx.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qx.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zi.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nb.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://vi.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://og.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://um.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://wu.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gu.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hm.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gn.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dh.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xw.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://lk.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bd.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://id.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ui.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nx.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fd.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ol.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kz.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kk.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ab.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ut.jianghongdianzi.cn

[B07] while 循环
来源：http://uv.newstarts.cn

Py:   while i < 10: i += 1
来源：http://ob.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hd.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://hb.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://cc.asd995.cn

Java: while (i < 10) { i++; }
来源：http://jy.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hb.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://us.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://gv.asd995.cn

[B08] do-while（至少执行一次）
来源：http://ri.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://hl.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://og.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://nf.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://hi.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://qp.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mn.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ca.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://xm.jctech888.com.cn

[B09] break 与 continue
来源：http://mu.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hi.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kj.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rd.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ga.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hi.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nv.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ki.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oh.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://im.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zi.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xj.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mf.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fz.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jd.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ch.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eb.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nm.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://qx.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://yk.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://jd.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://we.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cd.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://am.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bb.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://cd.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gh.9csxet.cn

[B12] 跳出多层循环
来源：http://db.wgjwhj.cn


<!-- 参考信息 -->