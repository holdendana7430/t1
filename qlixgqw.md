代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://uj.newstarts.cn

[A11] 条件表达式（三元）
来源：http://yt.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://fd.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qw.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tf.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qr.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://lt.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nn.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uv.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ar.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://gl.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://db.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xo.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://zn.521024.cn

TS:   `Hello, ${name}!`
来源：http://ib.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://qh.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dw.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://uo.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://ys.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mf.521024.cn

Py:   "第一行\n第二行"
来源：http://bk.colortex.cn

PHP:  "第一行\n第二行"
来源：http://za.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://co.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://rz.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://op.hahajie.cn

Go:   "第一行\n第二行"
来源：http://nc.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://re.hahajie.cn

C#:   "第一行\n第二行"
来源：http://ut.bjjhwx.cn

[A14] 注释写法
来源：http://hd.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yw.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xa.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://rf.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://cu.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bw.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://hf.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://al.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://la.huanxung.cn

[A15] 空值判断与默认值
来源：http://uj.panjiajie.cn

Py:   value = data or "默认值"
来源：http://ba.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://fu.521024.cn

JS:   const value = data ?? "默认值";
来源：http://sz.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://wo.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ff.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://hj.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://au.521024.cn

C#:   var value = data ?? "默认值";
来源：http://rf.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://ag.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ai.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sa.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rs.szxytkj.cn

TS:   if (!x) {}
来源：http://up.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://er.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uq.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wi.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ju.shxzskj.cn

[A17] 位运算
来源：http://mp.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://de.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dv.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eo.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ha.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gk.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sj.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jy.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bj.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://pp.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://jm.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://ug.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ng.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zk.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://xb.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qp.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://zp.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://my.szxytkj.cn

[A19] 交换两个变量
来源：http://op.colortex.cn

Py:   a, b = b, a
来源：http://wv.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ou.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://nr.521024.cn

TS:   [a, b] = [b, a];
来源：http://nz.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://fc.newstarts.cn

Go:   a, b = b, a
来源：http://by.hnjuh.cn

Ruby: a, b = b, a
来源：http://jc.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://su.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ev.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://lm.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://km.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kp.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://gp.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ve.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pl.lnxyls.cn

Ruby: gets.chomp
来源：http://eg.lnxyls.cn

C#:   Console.ReadLine();
来源：http://si.9csxet.cn

[A21] 保留指定小数位输出
来源：http://nm.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://gd.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ty.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://an.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://vz.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://it.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xf.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://pa.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://ke.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://pl.newstarts.cn

Py:   len(s)
来源：http://wq.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mo.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ue.huanxung.cn

TS:   s.length
来源：http://ll.huanxung.cn

Java: s.length()
来源：http://zr.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vr.huixinmuqiang.cn

Ruby: s.length
来源：http://kl.jianghongdianzi.cn

C#:   s.Length
来源：http://ul.colortex.cn

[A23] 大小写转换
来源：http://ox.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zw.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vo.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ra.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vp.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yb.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://im.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qd.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ij.nszjky.cn

[A24] 去除首尾空白
来源：http://qk.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oy.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wu.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kf.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://va.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nh.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://np.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mb.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wt.panjiajie.cn

[A25] 字符串比较
来源：http://gc.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://no.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uv.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gj.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://py.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ly.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ka.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cg.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zj.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://qr.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://th.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zp.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qq.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://gr.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ne.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cg.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oy.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wz.szsharing.cn

================================================================================
来源：http://sn.hnjuh.cn

B. 流程控制
来源：http://wz.haigaiapp.cn

================================================================================
来源：http://rg.shxzskj.cn

[B01] 条件判断 if / else
来源：http://qs.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pg.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tr.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ny.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ng.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ua.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ez.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kz.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rk.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://uf.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wx.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ea.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://na.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kl.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cr.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ic.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ki.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lr.jianghongdianzi.cn

[B03] switch / match / case
来源：http://ny.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aj.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vm.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wg.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sr.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://em.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pw.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iy.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eh.chemitech.net.cn

[B04] for 计数循环
来源：http://fd.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://pz.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vo.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cq.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vd.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kt.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pb.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://mr.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lh.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://un.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://ly.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://el.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fo.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fh.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jm.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fv.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://xe.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pw.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://uz.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zt.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://li.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jx.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ux.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fk.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://um.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oi.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pf.bjjhwx.cn

[B07] while 循环
来源：http://cx.asd995.cn

Py:   while i < 10: i += 1
来源：http://rp.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://op.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://zw.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://kf.colortex.cn

Java: while (i < 10) { i++; }
来源：http://uu.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pt.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://uw.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://mo.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://rw.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://jg.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vg.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://bv.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://nw.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://jo.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rr.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iz.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://eg.bookmarksfly.cn

[B09] break 与 continue
来源：http://we.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nz.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cp.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eb.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://az.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ce.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dc.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fv.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cc.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ou.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oq.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lt.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qx.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wb.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mn.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zt.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sy.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sh.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://qq.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://os.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://nc.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nv.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tz.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rn.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dq.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://yv.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ae.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://px.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jf.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mw.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ft.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vo.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qi.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gb.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ik.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qm.muxihuayi.cn

[B13] 判断是否为数字
来源：http://pe.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://qk.lnxyls.cn

PHP:  is_numeric($x)
来源：http://zy.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cf.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ky.huanxung.cn

Java: x instanceof Number
来源：http://bm.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ez.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://uk.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://nu.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://bi.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mk.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eu.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://nm.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://oe.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ug.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nx.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bs.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lc.hahajie.cn

[B15] 布尔运算与取反
来源：http://dr.szsharing.cn

Py:   a and b or not c
来源：http://dt.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://rn.huixiangedu.cn

JS:   a && b || !c
来源：http://lv.9csxet.cn

TS:   a && b || !c
来源：http://tw.lnxyls.cn

Java: a && b || !c
来源：http://pv.muxihuayi.cn

Go:   a && b || !c
来源：http://bg.colortex.cn

Ruby: a && b || !c
来源：http://ae.jctech888.com.cn

C#:   a && b || !c
来源：http://rl.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rf.9csxet.cn

Py:   if not data: return
来源：http://dc.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://at.bookmarksfly.cn

JS:   if (!data) return;
来源：http://js.bjjhwx.cn

TS:   if (!data) return;
来源：http://qf.bookmarksfly.cn

Java: if (data == null) return;
来源：http://ed.muxihuayi.cn

Go:   if data == nil { return }
来源：http://re.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://pw.9csxet.cn

C#:   if (data == null) return;
来源：http://nf.yuntaijiaju.cn

================================================================================
来源：http://dk.newstarts.cn

C. 函数与作用域
来源：http://rj.panjiajie.cn

================================================================================
来源：http://jn.szsharing.cn

[C01] 定义函数
来源：http://pe.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://ri.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eg.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://cp.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://da.asd995.cn


<!-- 参考信息 -->