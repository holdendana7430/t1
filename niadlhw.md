代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://tz.hahajie.cn

[A15] 空值判断与默认值
来源：http://zk.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://tm.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://yo.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://qb.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://sy.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oy.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://wt.hahajie.cn

Ruby: value = data || "默认值"
来源：http://zu.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://of.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://jd.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jz.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tt.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vm.szxytkj.cn

TS:   if (!x) {}
来源：http://tf.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://up.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jw.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hm.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ho.yuntaijiaju.cn

[A17] 位运算
来源：http://al.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mr.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zv.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nh.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dn.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://px.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zb.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vr.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ly.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://gx.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://sv.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://ch.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ig.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://es.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://ni.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wz.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://nw.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://jf.jctech888.com.cn

[A19] 交换两个变量
来源：http://lg.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://mp.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ej.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://ru.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://dr.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://es.hnjuh.cn

Go:   a, b = b, a
来源：http://dk.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://ar.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://xb.newstarts.cn

[A20] 读取标准输入
来源：http://jw.521024.cn

Py:   name = input("请输入：")
来源：http://ie.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iq.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ai.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://qn.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://yq.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dp.haigaiapp.cn

Ruby: gets.chomp
来源：http://xu.asd995.cn

C#:   Console.ReadLine();
来源：http://bn.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://ip.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://xh.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fs.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://sd.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://mh.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://uv.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nk.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ap.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://nd.hahajie.cn

[A22] 获取字符串长度
来源：http://vo.lnxyls.cn

Py:   len(s)
来源：http://lu.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qc.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://de.huanxung.cn

TS:   s.length
来源：http://jh.szsharing.cn

Java: s.length()
来源：http://tk.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://al.asd995.cn

Ruby: s.length
来源：http://zs.huixinmuqiang.cn

C#:   s.Length
来源：http://iv.huixinmuqiang.cn

[A23] 大小写转换
来源：http://av.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kj.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qh.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cz.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pj.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lz.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bf.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dh.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tu.gzmigu.cn

[A24] 去除首尾空白
来源：http://vv.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ad.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sn.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cs.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ev.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xq.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://jt.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pn.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iy.haigaiapp.cn

[A25] 字符串比较
来源：http://hx.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://lf.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ra.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://re.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sl.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tj.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yq.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mj.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pp.huixiangedu.cn

[A26] 类型转换总览
来源：http://vn.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iw.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ok.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ug.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://iy.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qu.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dq.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sx.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gg.asd995.cn

================================================================================
来源：http://al.shxzukj.cn

B. 流程控制
来源：http://mx.wgjwhj.cn

================================================================================
来源：http://ua.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://fe.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dc.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ne.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ts.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vz.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jk.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sx.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ji.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ye.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://ik.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kd.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fk.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rh.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vo.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dp.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lu.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yo.shxzskj.cn

[B03] switch / match / case
来源：http://rv.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oo.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nh.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://no.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ua.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qr.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uw.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bu.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gy.colortex.cn

[B04] for 计数循环
来源：http://xk.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://hd.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://np.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vu.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ml.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ul.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ce.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://xp.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jr.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://wz.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://pe.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nt.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ec.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gq.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hc.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ty.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://ae.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ar.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://ht.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://km.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vf.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wc.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ns.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vl.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qd.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tv.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jianghongdianzi.cn

[B07] while 循环
来源：http://ln.szsharing.cn

Py:   while i < 10: i += 1
来源：http://js.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xg.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://us.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://zl.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://gd.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ik.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://px.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://ox.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://pc.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://hw.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ay.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://ja.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://wc.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://hu.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zm.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pk.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://yz.lnxyls.cn

[B09] break 与 continue
来源：http://le.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fz.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mt.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xc.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fn.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ku.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jn.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gi.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oa.9csxet.cn

[B10] 遍历同时拿索引
来源：http://pv.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gq.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wx.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://au.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kh.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rz.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xj.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gb.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ps.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://lv.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://ok.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://nq.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wv.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lo.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pd.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hc.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://wt.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ty.nszjky.cn

[B12] 跳出多层循环
来源：http://et.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lj.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hh.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://di.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ql.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tl.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gm.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ou.wgjwhj.cn

[B13] 判断是否为数字
来源：http://nk.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://yk.newstarts.cn

PHP:  is_numeric($x)
来源：http://ec.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bt.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tu.panjiajie.cn

Java: x instanceof Number
来源：http://et.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lb.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://gy.hnjuh.cn

C#:   x is int or double or decimal
来源：http://ct.asd995.cn

[B14] 判断值是否在集合内
来源：http://mn.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fs.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ot.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://jz.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://bq.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nh.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rx.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bb.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yr.gzmigu.cn

[B15] 布尔运算与取反
来源：http://is.yuexingan06.cn

Py:   a and b or not c
来源：http://zs.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://rq.colortex.cn

JS:   a && b || !c
来源：http://sk.huixinmuqiang.cn

TS:   a && b || !c
来源：http://aw.nicolike.cn

Java: a && b || !c
来源：http://dd.huixinmuqiang.cn

Go:   a && b || !c
来源：http://uh.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://rb.bjjhwx.cn

C#:   a && b || !c
来源：http://qz.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rs.shtwfgs.cn

Py:   if not data: return
来源：http://ia.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://yh.bjjhwx.cn

JS:   if (!data) return;
来源：http://ui.panjiajie.cn

TS:   if (!data) return;
来源：http://ao.bookmarksfly.cn

Java: if (data == null) return;
来源：http://il.colortex.cn

Go:   if data == nil { return }
来源：http://ux.szsharing.cn

Ruby: return if data.nil?
来源：http://zk.shxzskj.cn

C#:   if (data == null) return;
来源：http://xz.jctech888.com.cn

================================================================================
来源：http://xu.wgjwhj.cn

C. 函数与作用域
来源：http://oi.szsharing.cn

================================================================================
来源：http://hx.521024.cn

[C01] 定义函数
来源：http://ba.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://ub.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wh.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://aj.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dy.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ke.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qp.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://ix.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mw.muxihuayi.cn

[C02] 默认参数
来源：http://gi.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://tf.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fz.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://dl.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rt.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mh.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kq.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://mk.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ee.panjiajie.cn

[C03] 可变参数
来源：http://ta.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://xy.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lg.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://im.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fb.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kt.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://so.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qm.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lo.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://mp.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tx.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xg.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ih.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ts.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ym.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://xf.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://jv.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://yo.jctech888.com.cn

[C05] 返回多个值
来源：http://df.lnxyls.cn

Py:   return a, b
来源：http://mw.newstarts.cn

PHP:  return [$a, $b];
来源：http://do.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uk.muxihuayi.cn

TS:   return { a, b };
来源：http://al.szsharing.cn


<!-- 参考信息 -->