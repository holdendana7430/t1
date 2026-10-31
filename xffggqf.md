代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://ru.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://at.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://oz.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ry.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://pj.nicolike.cn

[A15] 空值判断与默认值
来源：http://nq.hahajie.cn

Py:   value = data or "默认值"
来源：http://iw.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://qn.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://do.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://iw.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gd.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://fo.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://fj.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://lc.shxzukj.cn

[A16] 真假值判断规则
来源：http://sn.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wm.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oi.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ib.shxzukj.cn

TS:   if (!x) {}
来源：http://wi.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qg.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dc.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mb.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oa.wgjwhj.cn

[A17] 位运算
来源：http://bi.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uy.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://so.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sh.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zi.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ij.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fm.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pq.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qa.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://we.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://bb.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://ys.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://me.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://to.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://yv.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cd.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://vs.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://nu.jctech888.com.cn

[A19] 交换两个变量
来源：http://cp.panjiajie.cn

Py:   a, b = b, a
来源：http://gh.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bp.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://nz.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://cy.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://cf.colortex.cn

Go:   a, b = b, a
来源：http://qt.panjiajie.cn

Ruby: a, b = b, a
来源：http://ox.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://yi.521024.cn

[A20] 读取标准输入
来源：http://rq.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://nr.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qs.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://on.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://yf.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://gg.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ru.9csxet.cn

Ruby: gets.chomp
来源：http://xl.panjiajie.cn

C#:   Console.ReadLine();
来源：http://ij.szsharing.cn

[A21] 保留指定小数位输出
来源：http://yf.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://io.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jm.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://di.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ef.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://zw.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jv.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://vs.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://zv.wgjwhj.cn

[A22] 获取字符串长度
来源：http://mw.lnxyls.cn

Py:   len(s)
来源：http://pw.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wm.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sz.hnjuh.cn

TS:   s.length
来源：http://cm.muxihuayi.cn

Java: s.length()
来源：http://ob.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pe.jctech888.com.cn

Ruby: s.length
来源：http://mg.9csxet.cn

C#:   s.Length
来源：http://qn.nicolike.cn

[A23] 大小写转换
来源：http://cz.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://di.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wc.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ar.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://us.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hk.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xf.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ro.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dn.bjjhwx.cn

[A24] 去除首尾空白
来源：http://nd.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hb.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zr.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ti.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cn.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vi.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://lf.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mj.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cn.bjjhwx.cn

[A25] 字符串比较
来源：http://xz.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://me.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ng.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://un.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://za.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://js.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qh.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uk.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vu.colortex.cn

[A26] 类型转换总览
来源：http://ge.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mc.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iz.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hw.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://sd.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ob.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aw.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zn.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fu.hahajie.cn

================================================================================
来源：http://gi.wgjwhj.cn

B. 流程控制
来源：http://mc.szxytkj.cn

================================================================================
来源：http://aw.shxzskj.cn

[B01] 条件判断 if / else
来源：http://fw.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bm.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rk.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iq.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mt.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vz.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kj.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sc.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://ga.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rm.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hs.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nk.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rc.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ec.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mj.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mx.9csxet.cn

[B03] switch / match / case
来源：http://vl.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qo.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mv.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rd.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ut.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ri.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sj.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ez.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tq.yuexingan06.cn

[B04] for 计数循环
来源：http://eo.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://fk.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mw.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://no.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ft.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lw.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://et.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://bo.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lc.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://mr.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://wc.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qu.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wq.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ih.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ww.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ru.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://ak.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fy.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://az.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ic.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cq.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fh.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hp.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kt.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pg.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iw.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zq.wgjwhj.cn

[B07] while 循环
来源：http://wx.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://ua.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vh.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://rh.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://na.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://yn.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pw.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://xn.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://rv.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://qh.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://jp.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hc.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://fy.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://fr.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://jm.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://it.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ld.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://vz.nszjky.cn

[B09] break 与 continue
来源：http://ur.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mj.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zt.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cg.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bu.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yi.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lc.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dz.colortex.cn

[B10] 遍历同时拿索引
来源：http://bz.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vq.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sr.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mm.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kn.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wp.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qg.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pg.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xw.521024.cn

[B11] 生成数字序列 / 区间
来源：http://sa.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://az.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://ep.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://st.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://so.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bp.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jk.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://kf.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wd.szxytkj.cn

[B12] 跳出多层循环
来源：http://sg.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wm.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zm.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eh.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gh.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tc.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nk.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cz.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ey.bjjhwx.cn

[B13] 判断是否为数字
来源：http://dh.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://lm.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://wx.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cj.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://we.nszjky.cn

Java: x instanceof Number
来源：http://uk.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ws.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://rd.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://iw.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://db.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kx.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ow.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://mn.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://ig.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nv.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ec.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jf.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://by.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://gj.haigaiapp.cn

Py:   a and b or not c
来源：http://xe.hahajie.cn

PHP:  $a && $b || !$c
来源：http://mw.jctech888.com.cn

JS:   a && b || !c
来源：http://qx.huixinmuqiang.cn

TS:   a && b || !c
来源：http://zb.szsharing.cn

Java: a && b || !c
来源：http://ps.jianghongdianzi.cn

Go:   a && b || !c
来源：http://ho.huanxung.cn

Ruby: a && b || !c
来源：http://lr.yuntaijiaju.cn

C#:   a && b || !c
来源：http://mv.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qv.chemitech.net.cn

Py:   if not data: return
来源：http://cb.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://ds.bookmarksfly.cn

JS:   if (!data) return;
来源：http://zp.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://kp.wgjwhj.cn

Java: if (data == null) return;
来源：http://vm.shtwfgs.cn

Go:   if data == nil { return }
来源：http://xa.yuexingan06.cn

Ruby: return if data.nil?
来源：http://rd.panjiajie.cn

C#:   if (data == null) return;
来源：http://sg.asd995.cn

================================================================================
来源：http://hu.hahajie.cn

C. 函数与作用域
来源：http://to.szxytkj.cn

================================================================================
来源：http://hf.panjiajie.cn

[C01] 定义函数
来源：http://nw.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://bu.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uu.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://nm.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wq.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fp.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fn.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://yy.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://il.lnxyls.cn

[C02] 默认参数
来源：http://ym.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://ft.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kf.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://kl.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ki.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nm.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wa.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://oo.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ez.wgjwhj.cn

[C03] 可变参数
来源：http://jt.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://dg.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wi.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://st.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://av.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xg.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yr.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ol.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jw.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://tn.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://le.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qk.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://id.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fs.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://nl.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://up.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://ab.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://hu.panjiajie.cn

[C05] 返回多个值
来源：http://ze.hnjuh.cn


<!-- 参考信息 -->