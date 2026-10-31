代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jg.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://be.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ou.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ib.hahajie.cn

[A10] 生成随机数
来源：http://sp.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://wr.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://yy.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nm.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xe.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://il.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yd.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://ts.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://gl.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://tb.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://ye.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mj.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ho.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wy.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://zu.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wy.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fl.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eo.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://ys.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rt.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ei.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://jd.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://go.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://jz.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lk.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://hw.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://ah.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ww.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://al.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://ho.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://vo.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://qp.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://dj.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://ue.521024.cn

Ruby: "第一行\n第二行"
来源：http://jr.huanxung.cn

C#:   "第一行\n第二行"
来源：http://ae.szxytkj.cn

[A14] 注释写法
来源：http://ji.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vs.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ld.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://fc.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://pk.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cw.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://yc.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yc.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://hv.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://la.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://wy.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://qd.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://hh.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://bf.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gu.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://ls.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://vt.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://uo.nszjky.cn

[A16] 真假值判断规则
来源：http://ok.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vx.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lr.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ar.shxzukj.cn

TS:   if (!x) {}
来源：http://ej.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iu.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yu.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wz.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bi.newstarts.cn

[A17] 位运算
来源：http://mx.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ts.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jy.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lc.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bs.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ga.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zq.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qy.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bv.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://vu.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://gt.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://qd.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fr.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://at.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://fz.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zg.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://ew.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://vj.lnxyls.cn

[A19] 交换两个变量
来源：http://ct.asd995.cn

Py:   a, b = b, a
来源：http://mv.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pa.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://bp.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://ea.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://fm.lnxyls.cn

Go:   a, b = b, a
来源：http://vy.gzmigu.cn

Ruby: a, b = b, a
来源：http://em.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://sv.yuexingan06.cn

[A20] 读取标准输入
来源：http://lc.newstarts.cn

Py:   name = input("请输入：")
来源：http://dz.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dq.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ph.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://ze.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://vv.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dn.wgjwhj.cn

Ruby: gets.chomp
来源：http://mn.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://vk.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://rq.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://vc.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pz.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://qw.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://gd.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://is.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kn.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://zp.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://fn.yuexingan06.cn

[A22] 获取字符串长度
来源：http://ki.521024.cn

Py:   len(s)
来源：http://mb.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kz.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kq.lnxyls.cn

TS:   s.length
来源：http://mz.521024.cn

Java: s.length()
来源：http://ir.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mx.colortex.cn

Ruby: s.length
来源：http://og.hnjuh.cn

C#:   s.Length
来源：http://eh.huixinmuqiang.cn

[A23] 大小写转换
来源：http://qi.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nv.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tg.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ra.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hr.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bg.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ix.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ja.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sb.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://qp.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cq.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://td.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nz.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tw.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eo.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://lo.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ve.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ys.chemitech.net.cn

[A25] 字符串比较
来源：http://bt.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://fm.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fg.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cp.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kb.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zg.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kx.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xe.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nc.shxzukj.cn

[A26] 类型转换总览
来源：http://km.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qy.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mq.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wk.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://xz.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zg.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nl.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gt.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wl.panjiajie.cn

================================================================================
来源：http://zi.huanxung.cn

B. 流程控制
来源：http://st.haigaiapp.cn

================================================================================
来源：http://go.gzmigu.cn

[B01] 条件判断 if / else
来源：http://by.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jp.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uw.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bw.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pr.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bl.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nz.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xk.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hi.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://df.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ny.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vc.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vr.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xw.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fl.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uy.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cs.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://am.lnxyls.cn

[B03] switch / match / case
来源：http://gi.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jo.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rs.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gu.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://my.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://va.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ve.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ug.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xo.gzmigu.cn

[B04] for 计数循环
来源：http://ni.asd995.cn

Py:   for i in range(10): print(i)
来源：http://dp.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xi.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rr.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vk.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ui.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pw.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://lz.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mz.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://jv.newstarts.cn

Py:   for item in arr: print(item)
来源：http://of.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sa.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bi.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vo.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ua.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kb.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://pu.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lg.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://cj.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yt.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dh.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mt.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yt.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ll.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://th.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ch.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kd.szsharing.cn

[B07] while 循环
来源：http://uh.colortex.cn

Py:   while i < 10: i += 1
来源：http://ap.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://od.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://ds.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://bc.colortex.cn

Java: while (i < 10) { i++; }
来源：http://vi.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nu.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://eg.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://wv.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://zo.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://lv.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jm.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://xe.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://wh.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://jo.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rt.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qt.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://bd.521024.cn

[B09] break 与 continue
来源：http://as.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ew.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cm.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hy.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xs.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mn.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pt.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ba.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ct.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://qx.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cr.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ni.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gr.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://er.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kl.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eg.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qj.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ns.521024.cn

[B11] 生成数字序列 / 区间
来源：http://cb.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://nz.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://ll.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tm.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bg.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://je.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nl.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://be.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ch.gzmigu.cn

[B12] 跳出多层循环
来源：http://kl.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://au.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hf.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bk.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yz.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hg.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://la.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qp.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kk.shtwfgs.cn

[B13] 判断是否为数字
来源：http://cr.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://ow.szxytkj.cn

PHP:  is_numeric($x)
来源：http://io.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vp.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nv.gzmigu.cn

Java: x instanceof Number
来源：http://cm.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rd.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://wn.gzmigu.cn

C#:   x is int or double or decimal
来源：http://nq.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://pn.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yw.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yc.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://zq.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://bq.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zf.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dr.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zj.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lp.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://va.yuexingan06.cn

Py:   a and b or not c
来源：http://ib.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://uk.newstarts.cn

JS:   a && b || !c
来源：http://nm.bjjhwx.cn

TS:   a && b || !c
来源：http://jx.nszjky.cn

Java: a && b || !c
来源：http://cn.muxihuayi.cn

Go:   a && b || !c
来源：http://cz.521024.cn

Ruby: a && b || !c
来源：http://cg.huixiangedu.cn

C#:   a && b || !c
来源：http://fq.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://km.shtwfgs.cn

Py:   if not data: return
来源：http://qv.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://zb.lnxyls.cn

JS:   if (!data) return;
来源：http://wf.gzmigu.cn

TS:   if (!data) return;
来源：http://ml.colortex.cn


<!-- 参考信息 -->