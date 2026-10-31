代发 wailian999

[A14] 注释写法
来源：http://eh.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nh.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hh.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://to.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://if.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tg.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://bp.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mh.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://xu.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://qp.hnjuh.cn

Py:   value = data or "默认值"
来源：http://to.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://yj.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://wz.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://cz.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cp.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://by.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://zu.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://sz.newstarts.cn

[A16] 真假值判断规则
来源：http://av.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ax.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://og.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kp.panjiajie.cn

TS:   if (!x) {}
来源：http://kj.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iq.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pz.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://eb.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ig.nszjky.cn

[A17] 位运算
来源：http://be.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pn.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rf.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://es.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pp.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://it.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jy.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rq.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yy.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://ei.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://tr.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://uh.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xm.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vt.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://ab.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ie.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://zu.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://gr.bookmarksfly.cn

[A19] 交换两个变量
来源：http://yt.hnjuh.cn

Py:   a, b = b, a
来源：http://dm.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://td.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://mt.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://zf.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://vm.muxihuayi.cn

Go:   a, b = b, a
来源：http://cv.bjjhwx.cn

Ruby: a, b = b, a
来源：http://ip.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://kr.shtwfgs.cn

[A20] 读取标准输入
来源：http://zj.lnxyls.cn

Py:   name = input("请输入：")
来源：http://nt.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wa.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pi.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://cv.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://ci.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xg.bookmarksfly.cn

Ruby: gets.chomp
来源：http://al.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://ky.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://uv.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://tj.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rr.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://wu.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://gw.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://ai.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yn.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ru.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://vp.nicolike.cn

[A22] 获取字符串长度
来源：http://sj.shtwfgs.cn

Py:   len(s)
来源：http://ni.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uw.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gw.asd995.cn

TS:   s.length
来源：http://vo.asd995.cn

Java: s.length()
来源：http://rv.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pn.huixinmuqiang.cn

Ruby: s.length
来源：http://jk.yuntaijiaju.cn

C#:   s.Length
来源：http://ws.huixiangedu.cn

[A23] 大小写转换
来源：http://cs.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ah.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oo.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dc.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hn.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ew.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oh.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ih.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wd.chemitech.net.cn

[A24] 去除首尾空白
来源：http://sp.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ay.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://az.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bh.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mo.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ng.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://an.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wu.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dq.9csxet.cn

[A25] 字符串比较
来源：http://so.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://tt.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sa.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yi.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ht.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qi.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wm.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nu.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vd.shxzukj.cn

[A26] 类型转换总览
来源：http://zd.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bx.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ut.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bz.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://hj.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gk.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rb.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://le.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ny.yuexingan06.cn

================================================================================
来源：http://ya.shtwfgs.cn

B. 流程控制
来源：http://au.gzmigu.cn

================================================================================
来源：http://ex.shxzskj.cn

[B01] 条件判断 if / else
来源：http://bf.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zf.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fc.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dd.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ty.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sr.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ju.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wt.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ue.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://ts.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lh.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bl.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ay.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://he.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ud.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vc.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uh.9csxet.cn

[B03] switch / match / case
来源：http://ds.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cm.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zb.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dq.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ay.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lh.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rs.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hx.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hi.hahajie.cn

[B04] for 计数循环
来源：http://rf.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://vy.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://px.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tl.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ye.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wx.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ii.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://sw.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vt.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://mj.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://bq.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zd.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qu.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://od.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yo.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ce.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://ku.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kt.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://zz.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yy.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vs.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cd.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ud.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zr.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zj.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ix.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vh.shtwfgs.cn

[B07] while 循环
来源：http://bm.521024.cn

Py:   while i < 10: i += 1
来源：http://nw.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fs.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://dj.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://my.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://gi.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cr.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://yd.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://hr.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://rn.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://nw.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hr.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://he.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://qj.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://ce.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ki.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jk.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://pl.hnjuh.cn

[B09] break 与 continue
来源：http://hn.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ix.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ga.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gz.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vo.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gy.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wp.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tf.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bl.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://qe.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aj.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ls.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ac.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://co.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yc.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mw.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cs.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xz.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://ox.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://oh.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://ee.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lt.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vw.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uq.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jx.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://rz.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gp.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://ov.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yw.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jb.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pr.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tg.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ny.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dd.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://be.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mc.lnxyls.cn

[B13] 判断是否为数字
来源：http://ep.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ss.nicolike.cn

PHP:  is_numeric($x)
来源：http://dx.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yn.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jc.szxytkj.cn

Java: x instanceof Number
来源：http://tv.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zr.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://pt.panjiajie.cn

C#:   x is int or double or decimal
来源：http://dr.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://si.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fa.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://by.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://oe.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://cc.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ht.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dq.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wc.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ds.asd995.cn

[B15] 布尔运算与取反
来源：http://pa.bookmarksfly.cn

Py:   a and b or not c
来源：http://dp.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://vn.szxytkj.cn

JS:   a && b || !c
来源：http://rp.huanxung.cn

TS:   a && b || !c
来源：http://sn.nicolike.cn

Java: a && b || !c
来源：http://uo.521024.cn

Go:   a && b || !c
来源：http://oq.panjiajie.cn

Ruby: a && b || !c
来源：http://wr.colortex.cn

C#:   a && b || !c
来源：http://zh.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xl.bookmarksfly.cn

Py:   if not data: return
来源：http://so.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://fz.shxzukj.cn

JS:   if (!data) return;
来源：http://bu.jctech888.com.cn

TS:   if (!data) return;
来源：http://ze.bookmarksfly.cn

Java: if (data == null) return;
来源：http://lw.asd995.cn

Go:   if data == nil { return }
来源：http://la.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://wi.shtwfgs.cn

C#:   if (data == null) return;
来源：http://vw.shxzukj.cn

================================================================================
来源：http://wc.huanxung.cn

C. 函数与作用域
来源：http://ep.newstarts.cn

================================================================================
来源：http://gd.shtwfgs.cn

[C01] 定义函数
来源：http://fb.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://da.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qw.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://dh.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ef.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ik.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wi.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://mh.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fn.bjjhwx.cn

[C02] 默认参数
来源：http://bu.colortex.cn

Py:   def greet(name="World"): return name
来源：http://gl.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hq.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://bd.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fr.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ei.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://za.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://be.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://rv.szxytkj.cn

[C03] 可变参数
来源：http://bq.521024.cn

Py:   def total(*args): return sum(args)
来源：http://tg.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qu.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mh.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://it.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hp.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sc.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ms.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gl.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://bs.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hb.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xl.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cs.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qs.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://py.muxihuayi.cn


<!-- 参考信息 -->