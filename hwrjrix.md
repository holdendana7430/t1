代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wi.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gy.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eq.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://no.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qo.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qc.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ce.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://gn.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wp.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tp.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vr.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wp.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yb.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ba.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://an.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uv.jianghongdianzi.cn

[A10] 生成随机数
来源：http://xb.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://ka.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://xh.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vl.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mp.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://fy.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pd.bjjhwx.cn

Ruby: rand(1..100)
来源：http://mj.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://lz.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://vp.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://dp.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ip.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zm.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wz.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://sy.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qx.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wv.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://st.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://yo.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cz.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ag.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://ig.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://xi.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://zd.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wz.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://dt.521024.cn

C#:   $"Hello, {name}!"
来源：http://hd.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xj.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://tj.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://ef.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://uc.521024.cn

TS:   "第一行\n第二行"
来源：http://sa.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://ad.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://da.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://ic.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://ph.yuexingan06.cn

[A14] 注释写法
来源：http://mv.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nk.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ei.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://fg.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://fq.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ze.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://sg.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nf.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://se.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://qa.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://ba.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://am.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://qv.521024.cn

TS:   const value = data ?? "默认值";
来源：http://ny.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kq.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://uc.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://bk.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://oe.gzmigu.cn

[A16] 真假值判断规则
来源：http://uw.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cr.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pq.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yh.bookmarksfly.cn

TS:   if (!x) {}
来源：http://lh.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aw.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iw.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ty.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dp.bookmarksfly.cn

[A17] 位运算
来源：http://kt.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bu.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ho.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nd.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ca.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vc.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ft.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qe.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://os.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://vw.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://ld.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bb.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cu.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://ja.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qd.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://qf.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://la.haigaiapp.cn

[A19] 交换两个变量
来源：http://yj.9csxet.cn

Py:   a, b = b, a
来源：http://zk.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tj.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://zz.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://cu.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://fx.szsharing.cn

Go:   a, b = b, a
来源：http://rl.yuexingan06.cn

Ruby: a, b = b, a
来源：http://na.asd995.cn

C#:   (a, b) = (b, a);
来源：http://np.shtwfgs.cn

[A20] 读取标准输入
来源：http://mx.szsharing.cn

Py:   name = input("请输入：")
来源：http://vr.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gd.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yc.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://bq.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://fw.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pw.muxihuayi.cn

Ruby: gets.chomp
来源：http://yl.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://cn.521024.cn

[A21] 保留指定小数位输出
来源：http://pa.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://hy.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zd.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://uq.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://om.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://dz.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zo.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://yh.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://vk.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://cz.lnxyls.cn

Py:   len(s)
来源：http://wh.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pa.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aw.shxzskj.cn

TS:   s.length
来源：http://eg.huixiangedu.cn

Java: s.length()
来源：http://hn.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sy.haigaiapp.cn

Ruby: s.length
来源：http://pe.521024.cn

C#:   s.Length
来源：http://fn.haigaiapp.cn

[A23] 大小写转换
来源：http://ul.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sk.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xa.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ga.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rh.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aq.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://op.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lw.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sz.newstarts.cn

[A24] 去除首尾空白
来源：http://dd.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uf.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bu.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ip.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cb.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ft.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://ya.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fm.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ef.huixiangedu.cn

[A25] 字符串比较
来源：http://vr.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://au.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xt.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bm.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nb.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mx.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kk.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fz.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jy.wgjwhj.cn

[A26] 类型转换总览
来源：http://am.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bl.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aw.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hg.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://fo.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lw.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mf.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zx.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ls.wgjwhj.cn

================================================================================
来源：http://vv.haigaiapp.cn

B. 流程控制
来源：http://pe.haigaiapp.cn

================================================================================
来源：http://vj.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://vt.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gn.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ia.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fc.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vm.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cy.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ts.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aw.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://db.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://jc.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zi.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mh.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sw.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yn.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qh.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ua.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lo.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nl.huixiangedu.cn

[B03] switch / match / case
来源：http://be.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://be.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dw.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ea.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eh.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cw.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cl.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://he.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qf.jianghongdianzi.cn

[B04] for 计数循环
来源：http://zf.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://ov.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qy.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ci.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lb.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ns.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ti.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://nd.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ot.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://gd.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://aa.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xx.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ke.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kb.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dy.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gz.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://gp.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ws.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://qk.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pq.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jx.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yy.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dz.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://il.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://um.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iw.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://de.newstarts.cn

[B07] while 循环
来源：http://qt.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://kw.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://su.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://al.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://sd.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://kq.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nh.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://ix.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://gw.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://rd.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://nk.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zr.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://jz.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://le.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://lq.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tt.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bf.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://ao.szxytkj.cn

[B09] break 与 continue
来源：http://ia.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hh.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://du.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bf.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ez.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nz.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ak.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cj.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ww.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://aa.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bx.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sp.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vp.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zs.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qi.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xa.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iy.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zj.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://ys.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://pg.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://dp.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://im.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pi.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vq.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zu.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://ti.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ew.colortex.cn

[B12] 跳出多层循环
来源：http://nh.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://te.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vx.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://om.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kc.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ha.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ig.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rz.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lq.wgjwhj.cn

[B13] 判断是否为数字
来源：http://wv.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://zy.nicolike.cn

PHP:  is_numeric($x)
来源：http://fw.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vx.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ig.yuexingan06.cn

Java: x instanceof Number
来源：http://uq.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vp.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://bk.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://ye.9csxet.cn

[B14] 判断值是否在集合内
来源：http://nq.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hi.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qb.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://sq.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://jz.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fp.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zk.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ug.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cx.hnjuh.cn

[B15] 布尔运算与取反
来源：http://vs.shxzskj.cn

Py:   a and b or not c
来源：http://af.szxytkj.cn


<!-- 参考信息 -->