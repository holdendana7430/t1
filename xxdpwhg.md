代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://tm.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ux.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://so.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ea.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sf.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uj.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://mt.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pc.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://px.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://dp.asd995.cn

TS:   `Hello, ${name}!`
来源：http://tm.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://si.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rt.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://xk.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://qc.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xv.colortex.cn

Py:   "第一行\n第二行"
来源：http://de.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://xr.nicolike.cn

JS:   "第一行\n第二行"
来源：http://ih.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://pc.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://xx.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://bn.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://ek.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://jh.haigaiapp.cn

[A14] 注释写法
来源：http://nc.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gp.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ap.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://ae.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://ew.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ap.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://sv.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tq.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://db.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://fr.lnxyls.cn

Py:   value = data or "默认值"
来源：http://mf.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ft.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://lq.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://vn.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jr.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://ny.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://cx.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://eo.jctech888.com.cn

[A16] 真假值判断规则
来源：http://yo.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sm.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ea.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tz.9csxet.cn

TS:   if (!x) {}
来源：http://yi.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bv.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://up.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ou.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vf.yuexingan06.cn

[A17] 位运算
来源：http://vh.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vd.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lv.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oi.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ht.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yt.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ee.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ux.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://cb.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://lh.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://kj.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jf.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ji.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://yc.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xc.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://lt.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://kj.yuexingan06.cn

[A19] 交换两个变量
来源：http://of.wgjwhj.cn

Py:   a, b = b, a
来源：http://rj.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://id.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://jb.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://jg.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://gm.shxzskj.cn

Go:   a, b = b, a
来源：http://wx.huixiangedu.cn

Ruby: a, b = b, a
来源：http://jm.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://tx.huixiangedu.cn

[A20] 读取标准输入
来源：http://jy.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://tn.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pu.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://np.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://eq.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://ow.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rm.haigaiapp.cn

Ruby: gets.chomp
来源：http://tj.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://fu.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://tc.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://sr.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mi.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://nv.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://sm.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://cx.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iy.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://gm.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://ip.huanxung.cn

[A22] 获取字符串长度
来源：http://jp.nicolike.cn

Py:   len(s)
来源：http://ei.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bm.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qy.asd995.cn

TS:   s.length
来源：http://ww.shxzskj.cn

Java: s.length()
来源：http://uo.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wm.panjiajie.cn

Ruby: s.length
来源：http://iv.lnxyls.cn

C#:   s.Length
来源：http://kp.huixinmuqiang.cn

[A23] 大小写转换
来源：http://kg.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://do.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ea.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hs.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wq.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lp.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mp.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://od.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dy.nicolike.cn

[A24] 去除首尾空白
来源：http://kx.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xn.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kl.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eb.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wd.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vd.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://am.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://an.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ii.panjiajie.cn

[A25] 字符串比较
来源：http://rn.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://be.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zf.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mv.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ht.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pp.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hn.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bq.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ln.nszjky.cn

[A26] 类型转换总览
来源：http://hb.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yw.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://db.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hx.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://dh.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uh.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ik.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lx.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hn.nicolike.cn

================================================================================
来源：http://kj.jianghongdianzi.cn

B. 流程控制
来源：http://ou.hahajie.cn

================================================================================
来源：http://hq.colortex.cn

[B01] 条件判断 if / else
来源：http://bo.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lu.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oz.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oy.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rt.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hj.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ez.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vt.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sd.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://jp.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vh.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ts.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vm.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ty.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wm.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lv.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yx.wgjwhj.cn

[B03] switch / match / case
来源：http://tz.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ut.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jz.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://do.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tj.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vz.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yp.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yd.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fd.521024.cn

[B04] for 计数循环
来源：http://nm.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://hm.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aa.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hu.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rq.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://di.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bv.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://wp.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://do.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://ku.colortex.cn

Py:   for item in arr: print(item)
来源：http://pd.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ta.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ee.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jd.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gl.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ei.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://hq.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://au.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://th.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lj.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sr.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pf.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jz.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pm.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cs.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ea.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pn.nszjky.cn

[B07] while 循环
来源：http://ja.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://ue.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ik.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://bp.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://ib.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://as.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ci.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://fg.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://zd.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://ni.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://cp.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lc.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://my.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://ge.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://gt.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://da.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://an.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://sp.huanxung.cn

[B09] break 与 continue
来源：http://lm.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ut.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pz.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kg.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lv.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://od.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xq.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rs.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fy.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://io.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cs.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bk.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ek.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sd.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xn.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ns.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zk.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sx.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://bc.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://cr.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://fh.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wq.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ga.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ya.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://so.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://hb.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://le.hnjuh.cn

[B12] 跳出多层循环
来源：http://ls.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gu.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wy.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ar.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nd.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ea.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uw.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qa.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hb.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://bt.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://pz.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://wg.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xg.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://do.yuexingan06.cn

Java: x instanceof Number
来源：http://ht.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lx.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://zf.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://qg.huanxung.cn

[B14] 判断值是否在集合内
来源：http://ew.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vj.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://be.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://lw.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://xs.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mu.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kh.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ql.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ty.newstarts.cn

[B15] 布尔运算与取反
来源：http://gd.jianghongdianzi.cn

Py:   a and b or not c
来源：http://gc.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://ln.colortex.cn

JS:   a && b || !c
来源：http://yu.nicolike.cn

TS:   a && b || !c
来源：http://na.bookmarksfly.cn

Java: a && b || !c
来源：http://vg.nszjky.cn

Go:   a && b || !c
来源：http://vc.wgjwhj.cn

Ruby: a && b || !c
来源：http://ue.panjiajie.cn

C#:   a && b || !c
来源：http://mz.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rg.gzmigu.cn

Py:   if not data: return
来源：http://kj.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://oa.yuexingan06.cn

JS:   if (!data) return;
来源：http://ea.nicolike.cn

TS:   if (!data) return;
来源：http://zz.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://rv.lnxyls.cn

Go:   if data == nil { return }
来源：http://zt.hnjuh.cn

Ruby: return if data.nil?
来源：http://lj.szxytkj.cn

C#:   if (data == null) return;
来源：http://pq.jctech888.com.cn

================================================================================
来源：http://mt.nszjky.cn

C. 函数与作用域
来源：http://jg.wgjwhj.cn

================================================================================
来源：http://kr.huanxung.cn

[C01] 定义函数
来源：http://kp.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://wu.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dw.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://od.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uf.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qh.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bp.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://km.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ou.shxzukj.cn


<!-- 参考信息 -->