代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://be.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yy.shtwfgs.cn

TS:   if (!x) {}
来源：http://ct.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://be.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ea.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kb.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ny.huixiangedu.cn

[A17] 位运算
来源：http://yj.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qv.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rz.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gi.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ie.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fn.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nz.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ur.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qq.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://cy.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://je.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://uh.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qv.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vn.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://ua.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dd.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://la.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://qq.huanxung.cn

[A19] 交换两个变量
来源：http://hr.nicolike.cn

Py:   a, b = b, a
来源：http://lb.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pj.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://nv.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://sb.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://hq.shxzskj.cn

Go:   a, b = b, a
来源：http://rw.shtwfgs.cn

Ruby: a, b = b, a
来源：http://zx.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://cz.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://tf.szsharing.cn

Py:   name = input("请输入：")
来源：http://mx.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tg.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lg.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://cf.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://yk.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yx.bookmarksfly.cn

Ruby: gets.chomp
来源：http://km.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://kh.newstarts.cn

[A21] 保留指定小数位输出
来源：http://wa.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://te.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gc.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://lm.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://jv.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://en.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://or.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://ia.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://gg.huixiangedu.cn

[A22] 获取字符串长度
来源：http://dx.yuexingan06.cn

Py:   len(s)
来源：http://ee.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mu.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bk.hnjuh.cn

TS:   s.length
来源：http://tb.hahajie.cn

Java: s.length()
来源：http://od.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bu.lnxyls.cn

Ruby: s.length
来源：http://zv.jianghongdianzi.cn

C#:   s.Length
来源：http://ms.szxytkj.cn

[A23] 大小写转换
来源：http://uy.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wz.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aw.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yv.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cj.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tf.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pc.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ci.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pk.lnxyls.cn

[A24] 去除首尾空白
来源：http://tr.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ao.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rd.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ec.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cv.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wi.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://el.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zk.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vu.haigaiapp.cn

[A25] 字符串比较
来源：http://lm.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://gs.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oh.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://of.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rd.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bj.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zk.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yg.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nl.szsharing.cn

[A26] 类型转换总览
来源：http://kt.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bp.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wg.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://et.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://eg.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kp.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wu.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fv.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uh.gzmigu.cn

================================================================================
来源：http://id.hahajie.cn

B. 流程控制
来源：http://rh.521024.cn

================================================================================
来源：http://sx.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://qm.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dp.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://im.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nr.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vu.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://na.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yc.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kn.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cp.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://tw.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://on.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uk.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kg.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pa.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vz.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yb.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zl.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ma.newstarts.cn

[B03] switch / match / case
来源：http://yy.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://px.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ta.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mm.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uv.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dk.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sm.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ca.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ox.lnxyls.cn

[B04] for 计数循环
来源：http://ch.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://vw.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ez.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rm.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rb.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://in.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gf.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://uk.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://up.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://us.huanxung.cn

Py:   for item in arr: print(item)
来源：http://ei.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wa.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gt.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qi.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zt.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xh.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://ak.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dk.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://ef.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tg.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oz.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cg.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hb.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rr.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wm.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gq.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hx.shxzskj.cn

[B07] while 循环
来源：http://ku.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://pm.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://od.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://th.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://rt.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://ym.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ip.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://wd.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://sy.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://qy.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://bu.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cf.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ar.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://ms.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://dj.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xm.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yn.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://yx.szsharing.cn

[B09] break 与 continue
来源：http://bf.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ey.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://af.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kg.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uq.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cn.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bh.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pt.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wc.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://qy.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://by.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mh.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kt.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zx.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uv.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wh.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xf.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://te.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://fs.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://jv.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://ph.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ly.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xc.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jh.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bv.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://jl.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cp.521024.cn

[B12] 跳出多层循环
来源：http://fa.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jh.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vl.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ac.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pr.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zq.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ae.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ts.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ov.muxihuayi.cn

[B13] 判断是否为数字
来源：http://im.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://by.panjiajie.cn

PHP:  is_numeric($x)
来源：http://wm.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://my.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sr.newstarts.cn

Java: x instanceof Number
来源：http://ko.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mt.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://hf.panjiajie.cn

C#:   x is int or double or decimal
来源：http://ik.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://hz.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yu.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hy.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://ag.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://ey.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ko.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xd.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://li.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qb.nszjky.cn

[B15] 布尔运算与取反
来源：http://sb.yuexingan06.cn

Py:   a and b or not c
来源：http://uq.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://de.bjjhwx.cn

JS:   a && b || !c
来源：http://cx.yuexingan06.cn

TS:   a && b || !c
来源：http://ln.bookmarksfly.cn

Java: a && b || !c
来源：http://qx.9csxet.cn

Go:   a && b || !c
来源：http://sl.lnxyls.cn

Ruby: a && b || !c
来源：http://vm.gzmigu.cn

C#:   a && b || !c
来源：http://yp.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ov.hahajie.cn

Py:   if not data: return
来源：http://tp.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://zg.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://ul.521024.cn

TS:   if (!data) return;
来源：http://zs.hahajie.cn

Java: if (data == null) return;
来源：http://bz.lnxyls.cn

Go:   if data == nil { return }
来源：http://ok.hahajie.cn

Ruby: return if data.nil?
来源：http://du.nicolike.cn

C#:   if (data == null) return;
来源：http://xw.hnjuh.cn

================================================================================
来源：http://lu.shxzskj.cn

C. 函数与作用域
来源：http://jd.shxzskj.cn

================================================================================
来源：http://zw.jctech888.com.cn

[C01] 定义函数
来源：http://fa.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://qh.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nn.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://oa.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wb.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qp.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zq.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://cm.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hp.colortex.cn

[C02] 默认参数
来源：http://mu.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://yf.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gi.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://rf.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zs.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sg.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://is.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://gz.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ma.huixiangedu.cn

[C03] 可变参数
来源：http://sh.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://pr.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yq.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ai.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://es.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pk.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nj.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nz.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ot.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://tl.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ci.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qc.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zc.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://hb.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://bc.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://hf.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://ah.nicolike.cn

[C05] 返回多个值
来源：http://mw.huixiangedu.cn

Py:   return a, b
来源：http://yb.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://ag.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sb.wgjwhj.cn

TS:   return { a, b };
来源：http://pj.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hu.521024.cn

Go:   return a, b
来源：http://rg.jctech888.com.cn

Ruby: return a, b
来源：http://mq.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://hy.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://oy.huanxung.cn

Py:   square = lambda x: x * x
来源：http://ax.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qt.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://vj.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://au.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hv.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gw.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://rc.gzmigu.cn


<!-- 参考信息 -->