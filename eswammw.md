代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://cj.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://is.nszjky.cn

Py:   value = data or "默认值"
来源：http://cw.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://fj.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://mo.521024.cn

TS:   const value = data ?? "默认值";
来源：http://db.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ih.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://hj.asd995.cn

Ruby: value = data || "默认值"
来源：http://ih.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://aq.szsharing.cn

[A16] 真假值判断规则
来源：http://ax.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ov.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lu.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gn.shxzskj.cn

TS:   if (!x) {}
来源：http://ly.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vj.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bn.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gl.huixinmuqiang.cn

[A17] 位运算
来源：http://rs.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bs.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://us.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://je.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dn.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zd.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ra.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jx.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ed.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://op.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://at.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://fd.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mw.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ye.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://fd.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zn.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://uz.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://th.yuexingan06.cn

[A19] 交换两个变量
来源：http://tp.szsharing.cn

Py:   a, b = b, a
来源：http://zv.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sx.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://yu.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://fd.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://vl.haigaiapp.cn

Go:   a, b = b, a
来源：http://vk.nszjky.cn

Ruby: a, b = b, a
来源：http://ad.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://rc.hnjuh.cn

[A20] 读取标准输入
来源：http://hf.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://at.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ut.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ug.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://yd.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://dl.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://un.gzmigu.cn

Ruby: gets.chomp
来源：http://ot.hnjuh.cn

C#:   Console.ReadLine();
来源：http://un.newstarts.cn

[A21] 保留指定小数位输出
来源：http://kw.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://nb.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xd.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://wt.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://re.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://ps.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qo.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://wp.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://vx.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://ev.shxzukj.cn

Py:   len(s)
来源：http://ml.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://is.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://og.muxihuayi.cn

TS:   s.length
来源：http://tl.colortex.cn

Java: s.length()
来源：http://hu.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ms.panjiajie.cn

Ruby: s.length
来源：http://dz.szxytkj.cn

C#:   s.Length
来源：http://go.jctech888.com.cn

[A23] 大小写转换
来源：http://gf.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://us.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bb.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zj.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ih.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fd.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sa.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ij.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qa.panjiajie.cn

[A24] 去除首尾空白
来源：http://ui.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://de.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vi.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yp.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nt.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cc.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://sx.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ck.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kh.huixinmuqiang.cn

[A25] 字符串比较
来源：http://yz.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://su.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ek.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://og.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kc.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pl.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ns.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gd.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zc.huixiangedu.cn

[A26] 类型转换总览
来源：http://km.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pz.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ct.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ih.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://wa.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fi.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zf.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sc.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wq.muxihuayi.cn

================================================================================
来源：http://ms.huanxung.cn

B. 流程控制
来源：http://eb.asd995.cn

================================================================================
来源：http://bw.521024.cn

[B01] 条件判断 if / else
来源：http://in.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ry.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ql.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gn.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nf.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ya.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pt.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wj.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ro.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://ip.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ym.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ti.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uh.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sj.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oi.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hd.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eh.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bt.yuntaijiaju.cn

[B03] switch / match / case
来源：http://hs.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xy.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wt.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ik.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ny.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xn.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mu.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ot.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mt.yuntaijiaju.cn

[B04] for 计数循环
来源：http://fa.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://hp.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rv.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qq.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ra.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eh.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nu.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://nz.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://py.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://oy.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://zh.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://po.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pv.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qm.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sq.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wl.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://ra.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kr.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://gp.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sg.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dx.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qx.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mv.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ln.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yf.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zn.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fz.bookmarksfly.cn

[B07] while 循环
来源：http://cy.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://kh.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sf.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://tn.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://sj.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://fy.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sv.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://kp.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://wr.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://ck.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ey.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mh.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://us.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://da.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://gy.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ev.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jq.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://dx.newstarts.cn

[B09] break 与 continue
来源：http://sr.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fr.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mr.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ro.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ng.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ma.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sm.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kz.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kp.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://an.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gd.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wp.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vd.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ym.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mu.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jf.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qm.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://om.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://nl.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://ba.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://ig.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sv.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ar.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nu.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ak.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://ip.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ji.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://pk.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rr.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xg.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tw.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kj.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://td.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://el.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xr.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hy.colortex.cn

[B13] 判断是否为数字
来源：http://uj.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://iy.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://qf.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ho.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qm.panjiajie.cn

Java: x instanceof Number
来源：http://ln.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ar.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://je.newstarts.cn

C#:   x is int or double or decimal
来源：http://ts.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://ls.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nq.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ly.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://fb.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://wc.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qk.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tv.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ew.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ul.9csxet.cn

[B15] 布尔运算与取反
来源：http://ey.521024.cn

Py:   a and b or not c
来源：http://ic.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://pv.bookmarksfly.cn

JS:   a && b || !c
来源：http://xb.huixiangedu.cn

TS:   a && b || !c
来源：http://ip.gzmigu.cn

Java: a && b || !c
来源：http://ep.huanxung.cn

Go:   a && b || !c
来源：http://is.yuexingan06.cn

Ruby: a && b || !c
来源：http://mu.yuntaijiaju.cn

C#:   a && b || !c
来源：http://zx.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ws.szxytkj.cn

Py:   if not data: return
来源：http://zx.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://vv.bjjhwx.cn

JS:   if (!data) return;
来源：http://vl.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://mv.huanxung.cn

Java: if (data == null) return;
来源：http://hb.9csxet.cn

Go:   if data == nil { return }
来源：http://oi.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://zf.nszjky.cn

C#:   if (data == null) return;
来源：http://bf.newstarts.cn

================================================================================
来源：http://gz.bjjhwx.cn

C. 函数与作用域
来源：http://vx.yuexingan06.cn

================================================================================
来源：http://xu.lnxyls.cn

[C01] 定义函数
来源：http://gj.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://qy.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sr.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://ph.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xd.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dn.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://af.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://qk.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hv.newstarts.cn

[C02] 默认参数
来源：http://kl.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://qz.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://df.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://yu.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xz.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zw.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://su.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://ys.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://en.nszjky.cn

[C03] 可变参数
来源：http://io.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://mj.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vr.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fb.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://as.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mx.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kb.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cq.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nm.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://qv.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ru.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zg.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pg.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ax.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://ug.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://wf.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://ee.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://cs.yuexingan06.cn

[C05] 返回多个值
来源：http://jb.bookmarksfly.cn

Py:   return a, b
来源：http://jy.shxzskj.cn

PHP:  return [$a, $b];
来源：http://md.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://se.hahajie.cn

TS:   return { a, b };
来源：http://mv.bookmarksfly.cn


<!-- 参考信息 -->