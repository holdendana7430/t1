代发 wailian999

[A14] 注释写法
来源：http://pv.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wq.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gt.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://on.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://mi.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nd.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://sg.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uk.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://jf.shxzskj.cn

[A15] 空值判断与默认值
来源：http://tk.9csxet.cn

Py:   value = data or "默认值"
来源：http://uk.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://pq.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://ad.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://rj.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ll.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://cs.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://bb.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://ol.nicolike.cn

[A16] 真假值判断规则
来源：http://qj.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tv.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bf.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tw.newstarts.cn

TS:   if (!x) {}
来源：http://xt.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kb.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xr.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vv.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gk.bookmarksfly.cn

[A17] 位运算
来源：http://qp.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://py.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ty.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mp.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cf.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fy.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ia.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qr.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tz.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://gd.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://ec.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://nk.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lo.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ji.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://ro.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dh.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://ty.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://gr.szsharing.cn

[A19] 交换两个变量
来源：http://iy.521024.cn

Py:   a, b = b, a
来源：http://hx.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hr.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://ti.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://fg.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://sd.shtwfgs.cn

Go:   a, b = b, a
来源：http://qj.shxzskj.cn

Ruby: a, b = b, a
来源：http://dq.521024.cn

C#:   (a, b) = (b, a);
来源：http://xv.nszjky.cn

[A20] 读取标准输入
来源：http://ja.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://zx.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pl.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ft.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://bw.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://ej.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mx.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://pi.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://kl.newstarts.cn

[A21] 保留指定小数位输出
来源：http://qu.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://yq.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hm.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://sy.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://pq.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://hy.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bk.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://nz.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://iy.jctech888.com.cn

[A22] 获取字符串长度
来源：http://wi.muxihuayi.cn

Py:   len(s)
来源：http://jz.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vh.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ra.hahajie.cn

TS:   s.length
来源：http://iw.muxihuayi.cn

Java: s.length()
来源：http://bp.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gu.jianghongdianzi.cn

Ruby: s.length
来源：http://gf.yuexingan06.cn

C#:   s.Length
来源：http://cv.shtwfgs.cn

[A23] 大小写转换
来源：http://dc.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zs.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nq.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lc.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vy.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cu.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yb.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uy.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://as.haigaiapp.cn

[A24] 去除首尾空白
来源：http://ol.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vi.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xr.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qr.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://af.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ax.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://gc.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ao.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tk.szxytkj.cn

[A25] 字符串比较
来源：http://yl.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://ox.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cv.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uz.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ol.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ut.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kd.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://do.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ej.szxytkj.cn

[A26] 类型转换总览
来源：http://xx.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mg.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dj.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mc.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://ux.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wm.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qh.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vi.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mf.bjjhwx.cn

================================================================================
来源：http://qg.gzmigu.cn

B. 流程控制
来源：http://or.bjjhwx.cn

================================================================================
来源：http://gy.521024.cn

[B01] 条件判断 if / else
来源：http://ln.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vy.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rh.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ts.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kv.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vx.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zg.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uc.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://me.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://na.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lr.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kn.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rc.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ri.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wa.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hu.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mc.colortex.cn

[B03] switch / match / case
来源：http://hv.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hk.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ez.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gn.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tu.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xm.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sy.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jz.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qc.haigaiapp.cn

[B04] for 计数循环
来源：http://ul.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://rm.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oi.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lj.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ws.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uv.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tl.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://wn.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zc.colortex.cn

[B05] 遍历数组 / 列表
来源：http://xu.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://db.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pp.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ra.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bt.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zi.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gd.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://oi.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rr.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://qd.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zl.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dt.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iq.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iu.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://il.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ih.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bc.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://he.bjjhwx.cn

[B07] while 循环
来源：http://uh.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://zb.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ln.521024.cn

JS:   while (i < 10) { i++; }
来源：http://qq.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://qa.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://mv.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tf.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://cn.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://ja.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://ki.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://za.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pz.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://dk.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://kz.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://cr.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qg.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xq.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://xa.chemitech.net.cn

[B09] break 与 continue
来源：http://tm.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cg.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://by.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uo.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mg.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fj.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ss.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fo.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rp.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://ou.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nu.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://se.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cp.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ab.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wj.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mx.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://em.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ll.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://za.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://ot.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://wu.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://li.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://em.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wv.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fj.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://wt.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dw.hahajie.cn

[B12] 跳出多层循环
来源：http://sr.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pm.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lk.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ff.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iy.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bf.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dx.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rk.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xa.muxihuayi.cn

[B13] 判断是否为数字
来源：http://lq.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://op.szsharing.cn

PHP:  is_numeric($x)
来源：http://wf.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://br.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pm.shtwfgs.cn

Java: x instanceof Number
来源：http://im.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://am.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://ry.lnxyls.cn

C#:   x is int or double or decimal
来源：http://cl.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://tb.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nr.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ax.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://xd.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://tf.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kh.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cx.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gk.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nz.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://un.haigaiapp.cn

Py:   a and b or not c
来源：http://qg.nicolike.cn

PHP:  $a && $b || !$c
来源：http://ay.bjjhwx.cn

JS:   a && b || !c
来源：http://ma.wgjwhj.cn

TS:   a && b || !c
来源：http://em.shtwfgs.cn

Java: a && b || !c
来源：http://wy.nicolike.cn

Go:   a && b || !c
来源：http://pn.lnxyls.cn

Ruby: a && b || !c
来源：http://wu.huixiangedu.cn

C#:   a && b || !c
来源：http://so.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gr.521024.cn

Py:   if not data: return
来源：http://pk.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://wh.wgjwhj.cn

JS:   if (!data) return;
来源：http://wo.huixiangedu.cn

TS:   if (!data) return;
来源：http://wo.gzmigu.cn

Java: if (data == null) return;
来源：http://nh.gzmigu.cn

Go:   if data == nil { return }
来源：http://sa.chemitech.net.cn

Ruby: return if data.nil?
来源：http://hp.521024.cn

C#:   if (data == null) return;
来源：http://fv.hahajie.cn

================================================================================
来源：http://dj.shxzukj.cn

C. 函数与作用域
来源：http://ow.huixinmuqiang.cn

================================================================================
来源：http://rq.nszjky.cn

[C01] 定义函数
来源：http://xc.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://bf.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nt.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://tb.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fq.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ly.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nr.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://st.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kg.shtwfgs.cn

[C02] 默认参数
来源：http://vc.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://dt.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nz.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://ln.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ur.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sx.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ei.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://nu.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://md.colortex.cn

[C03] 可变参数
来源：http://nl.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://gp.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fn.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://df.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rq.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tc.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://be.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wc.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://we.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://ru.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://od.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vh.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hk.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bg.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://zg.hnjuh.cn


<!-- 参考信息 -->