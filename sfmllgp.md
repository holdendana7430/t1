代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://ze.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fd.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rp.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://of.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sy.yuexingan06.cn

[A07] 数字转字符串
来源：http://aq.hahajie.cn

Py:   str(42)
来源：http://kd.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://bb.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://df.bjjhwx.cn

TS:   String(42)
来源：http://ab.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nm.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://in.9csxet.cn

Ruby: 42.to_s
来源：http://ix.szsharing.cn

C#:   42.ToString()
来源：http://it.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://ce.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cz.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bg.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nv.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://je.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hw.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dn.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jm.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wb.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://zp.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nz.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ev.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wb.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ps.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cs.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://di.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://za.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fp.wgjwhj.cn

[A10] 生成随机数
来源：http://iu.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://hc.colortex.cn

PHP:  random_int(1, 100);
来源：http://yy.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://im.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kk.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://tx.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gm.wgjwhj.cn

Ruby: rand(1..100)
来源：http://rx.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://oq.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://qh.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://gx.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://os.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ef.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fn.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://wq.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dq.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vt.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ph.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://ul.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://of.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ny.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://qb.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://ag.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://nr.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hg.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://pm.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://uc.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fw.nicolike.cn

Py:   "第一行\n第二行"
来源：http://pr.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://qo.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://pi.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://zx.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://wa.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://qq.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://ii.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://qj.521024.cn

[A14] 注释写法
来源：http://ya.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qq.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hs.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://pp.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://cz.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qq.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://iu.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ij.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://wb.gzmigu.cn

[A15] 空值判断与默认值
来源：http://gy.szsharing.cn

Py:   value = data or "默认值"
来源：http://un.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://jx.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://ii.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://gf.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wf.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://xo.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://nj.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://re.nszjky.cn

[A16] 真假值判断规则
来源：http://zt.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ba.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://no.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://da.newstarts.cn

TS:   if (!x) {}
来源：http://ym.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ny.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ep.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ez.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lw.jianghongdianzi.cn

[A17] 位运算
来源：http://zf.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xx.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oc.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tl.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xg.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ug.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xh.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fx.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://cz.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://ae.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://bm.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://js.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://or.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://bj.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mf.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://lm.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://sg.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://cy.szxytkj.cn

Py:   a, b = b, a
来源：http://ly.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gt.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://bm.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://op.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://af.shxzskj.cn

Go:   a, b = b, a
来源：http://uc.hnjuh.cn

Ruby: a, b = b, a
来源：http://nd.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://sh.newstarts.cn

[A20] 读取标准输入
来源：http://eb.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://qz.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lq.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vh.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://qv.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://fb.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://in.newstarts.cn

Ruby: gets.chomp
来源：http://ft.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://jp.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://hq.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://wb.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ef.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://hf.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://or.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://hk.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nl.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://pt.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://rx.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://ro.colortex.cn

Py:   len(s)
来源：http://yb.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vq.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ue.colortex.cn

TS:   s.length
来源：http://id.shxzskj.cn

Java: s.length()
来源：http://og.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wi.bjjhwx.cn

Ruby: s.length
来源：http://xl.newstarts.cn

C#:   s.Length
来源：http://wd.nszjky.cn

[A23] 大小写转换
来源：http://ge.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rc.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qb.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bx.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qp.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://so.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zk.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zr.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cb.szsharing.cn

[A24] 去除首尾空白
来源：http://vr.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gl.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wm.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rz.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pf.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gt.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://wx.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yv.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tp.panjiajie.cn

[A25] 字符串比较
来源：http://ix.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://qj.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sp.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ln.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fx.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wo.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tn.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mu.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qb.bjjhwx.cn

[A26] 类型转换总览
来源：http://wz.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mj.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ri.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qp.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://we.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bi.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eu.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rs.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iz.9csxet.cn

================================================================================
来源：http://or.szsharing.cn

B. 流程控制
来源：http://ft.9csxet.cn

================================================================================
来源：http://hb.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://dr.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xo.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ym.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://re.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vj.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gv.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cp.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vy.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://la.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://lw.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gm.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vq.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qw.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nk.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rz.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ix.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://px.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bn.newstarts.cn

[B03] switch / match / case
来源：http://hk.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jz.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nd.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ta.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dg.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dd.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jo.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ql.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xe.colortex.cn

[B04] for 计数循环
来源：http://em.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://vk.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dl.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ii.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://og.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jy.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fh.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://su.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sr.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://dh.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://km.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ag.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://om.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ez.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gz.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xf.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://aa.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fn.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://ft.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kh.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zx.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pj.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zf.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gs.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wg.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zr.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rz.bookmarksfly.cn

[B07] while 循环
来源：http://xn.szsharing.cn

Py:   while i < 10: i += 1
来源：http://cw.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yh.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://lb.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://ck.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://de.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mc.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://jd.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://fm.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://vf.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://vr.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cg.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://lg.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://uo.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://xa.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ws.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zt.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://jp.nszjky.cn

[B09] break 与 continue
来源：http://nb.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yo.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vw.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zz.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ra.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xe.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hx.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hq.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://va.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ny.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mr.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bz.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bq.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bg.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yr.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iq.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://go.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://kp.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://cf.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://vb.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dl.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://td.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ny.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rd.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://cg.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mm.lnxyls.cn

[B12] 跳出多层循环
来源：http://ok.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fh.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vq.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ia.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yh.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://us.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kt.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pn.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fo.bjjhwx.cn

[B13] 判断是否为数字
来源：http://tw.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://pi.gzmigu.cn

PHP:  is_numeric($x)
来源：http://bp.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vz.nszjky.cn


<!-- 参考信息 -->