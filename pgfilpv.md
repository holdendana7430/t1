代发 wailian999

[A14] 注释写法
来源：http://gn.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gv.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wl.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://ej.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://ll.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ye.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://vz.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vt.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://xh.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://az.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://tc.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://fd.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://gu.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://qi.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ui.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://py.9csxet.cn

Ruby: value = data || "默认值"
来源：http://ee.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://mk.haigaiapp.cn

[A16] 真假值判断规则
来源：http://ff.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dc.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kb.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tr.muxihuayi.cn

TS:   if (!x) {}
来源：http://ys.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iw.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cy.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zz.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nf.521024.cn

[A17] 位运算
来源：http://xp.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://py.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bd.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://da.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sj.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pb.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hy.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yr.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://zw.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://fj.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://to.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ho.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://si.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://ea.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://or.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://pc.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://ek.huanxung.cn

[A19] 交换两个变量
来源：http://vm.lnxyls.cn

Py:   a, b = b, a
来源：http://ok.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vt.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://gp.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://tt.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://of.hnjuh.cn

Go:   a, b = b, a
来源：http://gt.muxihuayi.cn

Ruby: a, b = b, a
来源：http://ps.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://lj.yuexingan06.cn

[A20] 读取标准输入
来源：http://dp.shxzukj.cn

Py:   name = input("请输入：")
来源：http://yf.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qc.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lk.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://aa.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://yy.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hp.9csxet.cn

Ruby: gets.chomp
来源：http://xx.shxzukj.cn

C#:   Console.ReadLine();
来源：http://yg.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://tm.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://qk.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hx.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://tg.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://kq.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://eo.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yd.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://cb.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://qg.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://ri.yuexingan06.cn

Py:   len(s)
来源：http://al.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zw.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yc.wgjwhj.cn

TS:   s.length
来源：http://wz.muxihuayi.cn

Java: s.length()
来源：http://jj.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iz.bookmarksfly.cn

Ruby: s.length
来源：http://pj.shxzukj.cn

C#:   s.Length
来源：http://av.nicolike.cn

[A23] 大小写转换
来源：http://pm.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wx.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oe.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bt.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://di.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yv.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sy.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jq.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://np.szxytkj.cn

[A24] 去除首尾空白
来源：http://lg.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mw.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bc.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jx.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xv.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fz.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://kf.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yo.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rp.colortex.cn

[A25] 字符串比较
来源：http://dp.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://yz.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gh.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cy.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cz.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wb.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ti.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cm.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nb.huixiangedu.cn

[A26] 类型转换总览
来源：http://hk.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uq.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gs.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://md.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://fu.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ee.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kl.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yk.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ms.yuntaijiaju.cn

================================================================================
来源：http://rf.nszjky.cn

B. 流程控制
来源：http://wf.szxytkj.cn

================================================================================
来源：http://mi.hnjuh.cn

[B01] 条件判断 if / else
来源：http://qa.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uc.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mk.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lp.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://df.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://to.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ns.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fp.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wp.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://ka.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ie.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zd.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kf.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://du.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xo.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pj.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ct.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nr.yuntaijiaju.cn

[B03] switch / match / case
来源：http://ey.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ap.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ov.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rk.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gd.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yf.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ic.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qx.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yo.yuexingan06.cn

[B04] for 计数循环
来源：http://lh.asd995.cn

Py:   for i in range(10): print(i)
来源：http://mf.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ri.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ae.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uq.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vg.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lj.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://xo.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gh.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://aq.nicolike.cn

Py:   for item in arr: print(item)
来源：http://ny.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bx.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ty.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rk.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lv.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nf.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://yb.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dk.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://ul.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zr.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gu.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cp.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hq.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fs.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vi.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tz.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rf.asd995.cn

[B07] while 循环
来源：http://sl.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://pb.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://px.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://fn.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://de.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://mk.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zi.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://dq.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://jx.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://li.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://mu.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tj.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://aw.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://pa.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://cm.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dl.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://la.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://qi.lnxyls.cn

[B09] break 与 continue
来源：http://pl.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jb.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://am.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ux.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ff.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ee.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://je.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nz.huanxung.cn

[B10] 遍历同时拿索引
来源：http://vc.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cd.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jo.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wp.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ts.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qm.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yr.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wy.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jo.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://za.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://yo.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://ux.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wd.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://we.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mi.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fv.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://fq.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://la.nszjky.cn

[B12] 跳出多层循环
来源：http://gm.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://it.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://js.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qw.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wf.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hj.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pj.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ii.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hk.hahajie.cn

[B13] 判断是否为数字
来源：http://zk.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://ys.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://az.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fx.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pp.jianghongdianzi.cn

Java: x instanceof Number
来源：http://hq.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ep.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://du.9csxet.cn

C#:   x is int or double or decimal
来源：http://zs.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ce.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hd.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gz.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ee.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://ka.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kp.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xm.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zv.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://px.shxzskj.cn

[B15] 布尔运算与取反
来源：http://sx.panjiajie.cn

Py:   a and b or not c
来源：http://iq.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://aq.szxytkj.cn

JS:   a && b || !c
来源：http://ut.szsharing.cn

TS:   a && b || !c
来源：http://sn.gzmigu.cn

Java: a && b || !c
来源：http://gy.chemitech.net.cn

Go:   a && b || !c
来源：http://yj.shtwfgs.cn

Ruby: a && b || !c
来源：http://yg.521024.cn

C#:   a && b || !c
来源：http://qq.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ls.hahajie.cn

Py:   if not data: return
来源：http://xv.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://na.colortex.cn

JS:   if (!data) return;
来源：http://ar.huanxung.cn

TS:   if (!data) return;
来源：http://rf.bjjhwx.cn

Java: if (data == null) return;
来源：http://lx.haigaiapp.cn

Go:   if data == nil { return }
来源：http://ul.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://nj.shtwfgs.cn

C#:   if (data == null) return;
来源：http://nt.shtwfgs.cn

================================================================================
来源：http://si.hahajie.cn

C. 函数与作用域
来源：http://yz.huanxung.cn

================================================================================
来源：http://ed.panjiajie.cn

[C01] 定义函数
来源：http://qp.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://fm.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rz.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://yc.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kv.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://go.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hy.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://wv.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cg.huixiangedu.cn

[C02] 默认参数
来源：http://zo.asd995.cn

Py:   def greet(name="World"): return name
来源：http://by.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kw.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://bg.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pc.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iq.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yp.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://nz.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://wn.jianghongdianzi.cn

[C03] 可变参数
来源：http://ta.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://iv.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bx.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jt.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ms.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fk.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qt.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gz.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://md.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://ub.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fo.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jz.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yl.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://io.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://ad.521024.cn


<!-- 参考信息 -->