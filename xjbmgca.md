代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zw.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wu.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ha.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ay.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wi.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zo.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gz.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hy.shtwfgs.cn

[A10] 生成随机数
来源：http://ti.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://ud.nicolike.cn

PHP:  random_int(1, 100);
来源：http://fn.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xd.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kd.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://ak.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yc.yuexingan06.cn

Ruby: rand(1..100)
来源：http://dl.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://yl.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://zp.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://rf.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zu.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yd.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ya.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://ee.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zy.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yo.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yh.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://rs.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aw.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ll.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://mr.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://fq.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://ri.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ek.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://dg.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://de.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://je.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://cy.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://yw.asd995.cn

JS:   "第一行\n第二行"
来源：http://xx.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://ds.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://fq.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://va.521024.cn

Ruby: "第一行\n第二行"
来源：http://is.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://ex.jctech888.com.cn

[A14] 注释写法
来源：http://se.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xf.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ca.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://ir.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://qo.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ya.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://pu.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jc.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://zj.hahajie.cn

[A15] 空值判断与默认值
来源：http://oj.newstarts.cn

Py:   value = data or "默认值"
来源：http://ng.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://ef.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://zh.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://fg.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fw.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://fa.9csxet.cn

Ruby: value = data || "默认值"
来源：http://nk.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://ju.hahajie.cn

[A16] 真假值判断规则
来源：http://vo.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wn.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cb.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bs.szxytkj.cn

TS:   if (!x) {}
来源：http://sn.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vd.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cj.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rv.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://et.bjjhwx.cn

[A17] 位运算
来源：http://vu.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vi.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wi.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ad.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ps.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ul.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tx.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wn.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hc.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://vv.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://oy.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://st.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dl.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ac.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://gp.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hu.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://kh.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://nv.shtwfgs.cn

[A19] 交换两个变量
来源：http://sw.asd995.cn

Py:   a, b = b, a
来源：http://gm.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ei.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://gc.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://zf.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://cu.hnjuh.cn

Go:   a, b = b, a
来源：http://ql.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://ah.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://ys.huixiangedu.cn

[A20] 读取标准输入
来源：http://ms.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://sm.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ai.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gs.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://mk.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://wy.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://di.gzmigu.cn

Ruby: gets.chomp
来源：http://vo.shxzskj.cn

C#:   Console.ReadLine();
来源：http://st.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://nq.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://yk.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ic.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://cw.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://ze.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://cq.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://np.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://cz.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://hw.yuexingan06.cn

[A22] 获取字符串长度
来源：http://xi.lnxyls.cn

Py:   len(s)
来源：http://ow.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ly.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ns.huixiangedu.cn

TS:   s.length
来源：http://pf.yuntaijiaju.cn

Java: s.length()
来源：http://bs.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lb.hnjuh.cn

Ruby: s.length
来源：http://wm.shxzskj.cn

C#:   s.Length
来源：http://ln.chemitech.net.cn

[A23] 大小写转换
来源：http://jh.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ag.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aw.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hf.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://br.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ik.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qy.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bt.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vk.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://zi.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wt.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wj.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://we.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xz.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cd.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://th.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fr.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aa.nszjky.cn

[A25] 字符串比较
来源：http://cy.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://on.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lr.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zs.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wk.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rx.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://px.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vs.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cf.huanxung.cn

[A26] 类型转换总览
来源：http://zt.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mk.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cp.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mt.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://mw.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rz.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bm.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qj.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yx.haigaiapp.cn

================================================================================
来源：http://li.bookmarksfly.cn

B. 流程控制
来源：http://gg.yuexingan06.cn

================================================================================
来源：http://bt.shxzukj.cn

[B01] 条件判断 if / else
来源：http://uc.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mt.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fb.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jx.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pz.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zu.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tr.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dj.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jv.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://mh.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lm.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hn.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ej.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fh.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mp.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xk.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uy.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ll.huanxung.cn

[B03] switch / match / case
来源：http://iw.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://io.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gp.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vh.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://os.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cv.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jn.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bl.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bc.nicolike.cn

[B04] for 计数循环
来源：http://zt.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://yg.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lz.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bz.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xv.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oi.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://fi.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tm.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://xc.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://xv.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mf.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mj.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kt.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wm.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ca.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://yv.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ry.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://vx.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vl.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://of.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qm.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://am.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sr.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wl.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nz.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uu.bookmarksfly.cn

[B07] while 循环
来源：http://jk.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://fm.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jn.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://mb.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://ff.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://rm.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dh.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://pd.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://wx.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://xf.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ri.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yy.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://vb.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://fy.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://vz.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bf.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eh.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://nl.newstarts.cn

[B09] break 与 continue
来源：http://sk.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ve.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cl.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kb.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iz.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wi.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pp.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://um.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://su.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://md.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kp.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://it.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pb.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ta.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tq.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zb.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jt.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://iv.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://sr.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://pc.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mx.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uo.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bc.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tp.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://fi.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cp.lnxyls.cn

[B12] 跳出多层循环
来源：http://tk.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://va.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ed.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qf.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hd.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kc.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mi.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hv.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bk.huixiangedu.cn

[B13] 判断是否为数字
来源：http://kr.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://ts.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://zu.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bl.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kp.huixinmuqiang.cn

Java: x instanceof Number
来源：http://cs.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vn.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://ov.nszjky.cn

C#:   x is int or double or decimal
来源：http://ui.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://nz.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fo.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bf.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://jb.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://rn.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://td.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qf.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hj.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ay.panjiajie.cn

[B15] 布尔运算与取反
来源：http://oi.yuexingan06.cn

Py:   a and b or not c
来源：http://bs.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://mf.huixiangedu.cn

JS:   a && b || !c
来源：http://ba.yuntaijiaju.cn

TS:   a && b || !c
来源：http://qi.lnxyls.cn

Java: a && b || !c
来源：http://lh.hnjuh.cn

Go:   a && b || !c
来源：http://ii.wgjwhj.cn

Ruby: a && b || !c
来源：http://oi.9csxet.cn

C#:   a && b || !c
来源：http://fg.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oj.huixiangedu.cn


<!-- 参考信息 -->