代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://za.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://oz.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://cj.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dq.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ht.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rr.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://bh.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lp.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vq.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hy.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://lx.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zw.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://at.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://le.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://xv.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://tr.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ht.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://aw.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://wy.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bu.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://qe.asd995.cn

PHP:  "第一行\n第二行"
来源：http://ki.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://wn.asd995.cn

TS:   "第一行\n第二行"
来源：http://tx.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://lj.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://pb.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://jj.9csxet.cn

C#:   "第一行\n第二行"
来源：http://pc.lnxyls.cn

[A14] 注释写法
来源：http://wi.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wl.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wz.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://cb.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://xa.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://an.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://il.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ll.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://xo.szxytkj.cn

[A15] 空值判断与默认值
来源：http://qi.asd995.cn

Py:   value = data or "默认值"
来源：http://lj.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://yg.521024.cn

JS:   const value = data ?? "默认值";
来源：http://tc.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://cp.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dr.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://gx.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://su.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://ml.asd995.cn

[A16] 真假值判断规则
来源：http://kf.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nm.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jg.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rn.yuexingan06.cn

TS:   if (!x) {}
来源：http://yc.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fz.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dx.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://as.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zo.jianghongdianzi.cn

[A17] 位运算
来源：http://rq.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://or.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hx.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://my.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://un.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rz.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iv.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://na.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bk.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://nv.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://kz.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://fi.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bd.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pm.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://ye.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ro.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://kp.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://bs.huanxung.cn

[A19] 交换两个变量
来源：http://vd.yuexingan06.cn

Py:   a, b = b, a
来源：http://du.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ud.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://dl.asd995.cn

TS:   [a, b] = [b, a];
来源：http://hk.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://hf.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://io.nszjky.cn

Ruby: a, b = b, a
来源：http://fg.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://wo.muxihuayi.cn

[A20] 读取标准输入
来源：http://qx.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://co.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ak.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pb.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://fe.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://yz.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://db.wgjwhj.cn

Ruby: gets.chomp
来源：http://cq.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://ni.szsharing.cn

[A21] 保留指定小数位输出
来源：http://rg.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://os.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bz.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://rl.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ee.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://cp.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lr.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://ep.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://qo.newstarts.cn

[A22] 获取字符串长度
来源：http://ij.huixiangedu.cn

Py:   len(s)
来源：http://gl.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ib.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dv.newstarts.cn

TS:   s.length
来源：http://dw.chemitech.net.cn

Java: s.length()
来源：http://sy.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qk.bjjhwx.cn

Ruby: s.length
来源：http://ji.bjjhwx.cn

C#:   s.Length
来源：http://ro.muxihuayi.cn

[A23] 大小写转换
来源：http://zc.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xm.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bt.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ci.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tf.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wn.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ij.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ug.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jr.yuexingan06.cn

[A24] 去除首尾空白
来源：http://yp.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tx.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://op.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://un.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nb.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dy.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://pd.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mw.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ws.huixiangedu.cn

[A25] 字符串比较
来源：http://vm.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://hs.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://te.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vd.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qz.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jz.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lx.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mc.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ka.chemitech.net.cn

[A26] 类型转换总览
来源：http://ps.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dd.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ab.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gq.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://lk.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yw.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hj.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xk.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sj.huixinmuqiang.cn

================================================================================
来源：http://fv.hnjuh.cn

B. 流程控制
来源：http://mm.nicolike.cn

================================================================================
来源：http://du.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://mv.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jo.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oa.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pu.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://et.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dh.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zq.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cm.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://al.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://td.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ss.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qg.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yo.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lf.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eg.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sl.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fy.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sk.9csxet.cn

[B03] switch / match / case
来源：http://jy.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yy.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bn.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wp.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oa.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jc.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rs.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oa.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://od.yuexingan06.cn

[B04] for 计数循环
来源：http://eq.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://dq.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dr.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xg.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rf.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ol.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://on.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://lj.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cp.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://bf.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://lt.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jx.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dm.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cb.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jp.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ul.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://mu.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ck.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://bq.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sz.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cb.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ks.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gf.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jx.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ny.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qq.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bv.colortex.cn

[B07] while 循环
来源：http://bp.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://uh.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://er.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://gk.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://hx.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://zb.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://va.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://tu.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://cz.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://jh.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://sx.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aa.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://eo.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://aw.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://vj.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sg.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qs.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://bv.huixiangedu.cn

[B09] break 与 continue
来源：http://va.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jh.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gp.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tz.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cs.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vc.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fh.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vj.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://gl.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yy.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ve.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tr.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qr.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uq.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ei.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uh.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nz.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://yy.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://kp.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://wy.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mj.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xp.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ft.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ce.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://sf.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wa.jctech888.com.cn

[B12] 跳出多层循环
来源：http://sg.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oz.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kr.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nv.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sy.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bt.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pl.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://el.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xj.chemitech.net.cn

[B13] 判断是否为数字
来源：http://cn.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://gd.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://ks.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aq.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gy.szxytkj.cn

Java: x instanceof Number
来源：http://id.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wh.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://yj.newstarts.cn

C#:   x is int or double or decimal
来源：http://wx.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://tf.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jm.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gy.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://dv.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://fp.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://na.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ye.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gt.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vo.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://sf.asd995.cn

Py:   a and b or not c
来源：http://ep.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://yz.nszjky.cn

JS:   a && b || !c
来源：http://wb.521024.cn

TS:   a && b || !c
来源：http://qk.lnxyls.cn

Java: a && b || !c
来源：http://jo.huixiangedu.cn

Go:   a && b || !c
来源：http://pj.newstarts.cn

Ruby: a && b || !c
来源：http://pm.521024.cn

C#:   a && b || !c
来源：http://zg.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wv.nszjky.cn

Py:   if not data: return
来源：http://lc.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://mc.gzmigu.cn

JS:   if (!data) return;
来源：http://ha.hnjuh.cn

TS:   if (!data) return;
来源：http://ew.chemitech.net.cn

Java: if (data == null) return;
来源：http://ve.szxytkj.cn

Go:   if data == nil { return }
来源：http://oi.haigaiapp.cn

Ruby: return if data.nil?
来源：http://vb.nszjky.cn

C#:   if (data == null) return;
来源：http://ny.jctech888.com.cn

================================================================================
来源：http://ms.lnxyls.cn

C. 函数与作用域
来源：http://zi.shxzskj.cn

================================================================================
来源：http://uo.shxzukj.cn

[C01] 定义函数
来源：http://ku.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://vv.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fh.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://dr.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pq.muxihuayi.cn


<!-- 参考信息 -->