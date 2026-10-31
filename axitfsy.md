代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://lk.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://sm.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://eh.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://se.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://oc.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://yv.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wq.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://bx.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://lg.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://ot.gzmigu.cn

[A16] 真假值判断规则
来源：http://pp.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zi.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jn.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ku.nszjky.cn

TS:   if (!x) {}
来源：http://cj.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nq.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yk.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oy.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://je.szsharing.cn

[A17] 位运算
来源：http://ol.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sn.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fv.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://as.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ng.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sm.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://te.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qm.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sj.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://wg.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://wm.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://ue.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jm.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mu.521024.cn

Java: (int) 'A'; (char) 65
来源：http://wa.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ib.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://vo.521024.cn

C#:   (int)'A'; (char)65
来源：http://yr.yuexingan06.cn

[A19] 交换两个变量
来源：http://em.chemitech.net.cn

Py:   a, b = b, a
来源：http://oj.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gk.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://mc.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://rs.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://lc.shtwfgs.cn

Go:   a, b = b, a
来源：http://zw.szsharing.cn

Ruby: a, b = b, a
来源：http://xm.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://pa.colortex.cn

[A20] 读取标准输入
来源：http://xd.panjiajie.cn

Py:   name = input("请输入：")
来源：http://vh.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ky.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nn.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://pg.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://pq.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://di.shxzukj.cn

Ruby: gets.chomp
来源：http://pq.lnxyls.cn

C#:   Console.ReadLine();
来源：http://sy.9csxet.cn

[A21] 保留指定小数位输出
来源：http://ng.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://gi.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dq.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://bi.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://qd.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://dg.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bn.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://xk.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://is.shxzskj.cn

[A22] 获取字符串长度
来源：http://rn.szsharing.cn

Py:   len(s)
来源：http://ej.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://of.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wl.huixiangedu.cn

TS:   s.length
来源：http://mq.9csxet.cn

Java: s.length()
来源：http://by.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ut.lnxyls.cn

Ruby: s.length
来源：http://aw.gzmigu.cn

C#:   s.Length
来源：http://aq.bjjhwx.cn

[A23] 大小写转换
来源：http://jv.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xf.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dl.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fr.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yr.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rj.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ff.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kc.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kr.panjiajie.cn

[A24] 去除首尾空白
来源：http://px.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wg.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ro.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tr.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gx.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gx.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://wh.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vb.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wz.wgjwhj.cn

[A25] 字符串比较
来源：http://zm.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://cp.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xo.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bs.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mr.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bt.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://th.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vs.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dt.bookmarksfly.cn

[A26] 类型转换总览
来源：http://au.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://el.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vu.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pu.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://yo.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pn.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://da.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rx.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mf.szxytkj.cn

================================================================================
来源：http://kj.szxytkj.cn

B. 流程控制
来源：http://ns.hnjuh.cn

================================================================================
来源：http://hq.newstarts.cn

[B01] 条件判断 if / else
来源：http://rd.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sz.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jo.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eh.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://li.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ed.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yt.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://js.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vq.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://rg.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nu.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xe.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tm.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wy.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ru.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://po.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dc.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rx.shtwfgs.cn

[B03] switch / match / case
来源：http://fn.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://er.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://km.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dz.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://za.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xz.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fh.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://se.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ds.chemitech.net.cn

[B04] for 计数循环
来源：http://jz.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://zf.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://de.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wg.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yp.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hj.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xi.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://pl.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hf.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://ya.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://xe.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gl.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hh.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://se.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xv.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jx.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://zz.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xb.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://kp.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ap.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ae.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://me.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ho.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ys.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gc.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xm.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ig.newstarts.cn

[B07] while 循环
来源：http://dt.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://ut.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vf.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://jx.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://vn.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://vp.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dw.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://eb.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://yd.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://rg.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://dc.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ep.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://gz.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://ne.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://dv.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uh.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gv.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://yz.wgjwhj.cn

[B09] break 与 continue
来源：http://mx.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://im.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kn.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://md.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://le.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ha.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fz.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dv.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://th.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://da.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nw.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ru.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dp.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qg.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oo.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xc.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lk.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vb.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://wj.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://cp.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://an.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wf.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xq.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://db.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fw.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://xd.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rl.haigaiapp.cn

[B12] 跳出多层循环
来源：http://ld.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://az.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://am.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hr.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://br.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://at.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://is.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uy.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vf.chemitech.net.cn

[B13] 判断是否为数字
来源：http://jn.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://ro.szxytkj.cn

PHP:  is_numeric($x)
来源：http://ls.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yy.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pr.wgjwhj.cn

Java: x instanceof Number
来源：http://av.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eq.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://nj.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://km.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://ij.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eu.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ws.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://pd.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://go.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fi.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://th.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cv.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qe.shxzukj.cn

[B15] 布尔运算与取反
来源：http://cc.bookmarksfly.cn

Py:   a and b or not c
来源：http://ft.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://zj.lnxyls.cn

JS:   a && b || !c
来源：http://ib.chemitech.net.cn

TS:   a && b || !c
来源：http://mq.nicolike.cn

Java: a && b || !c
来源：http://fa.bjjhwx.cn

Go:   a && b || !c
来源：http://ad.panjiajie.cn

Ruby: a && b || !c
来源：http://ar.hahajie.cn

C#:   a && b || !c
来源：http://jv.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xa.521024.cn

Py:   if not data: return
来源：http://sj.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://fc.bjjhwx.cn

JS:   if (!data) return;
来源：http://ms.newstarts.cn

TS:   if (!data) return;
来源：http://nt.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://zy.huixiangedu.cn

Go:   if data == nil { return }
来源：http://ks.lnxyls.cn

Ruby: return if data.nil?
来源：http://ci.521024.cn

C#:   if (data == null) return;
来源：http://za.huixiangedu.cn

================================================================================
来源：http://mu.jctech888.com.cn

C. 函数与作用域
来源：http://tu.muxihuayi.cn

================================================================================
来源：http://jz.szxytkj.cn

[C01] 定义函数
来源：http://pj.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://fc.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fg.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://ac.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ei.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ua.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vd.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://cf.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://id.szsharing.cn

[C02] 默认参数
来源：http://bc.colortex.cn

Py:   def greet(name="World"): return name
来源：http://cw.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oo.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://mh.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yf.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ol.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wy.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://se.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://cp.haigaiapp.cn

[C03] 可变参数
来源：http://zj.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://em.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yq.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kw.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rt.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jn.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hl.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ei.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ml.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://wz.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fc.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cy.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://re.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tt.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://zj.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://xi.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://ii.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://ou.9csxet.cn

[C05] 返回多个值
来源：http://le.shxzukj.cn

Py:   return a, b
来源：http://ez.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://qc.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mm.yuexingan06.cn

TS:   return { a, b };
来源：http://oz.shxzskj.cn


<!-- 参考信息 -->