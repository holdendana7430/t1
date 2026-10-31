代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ct.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ts.shxzskj.cn

TS:   if (!x) {}
来源：http://gv.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ar.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ze.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xv.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://li.muxihuayi.cn

[A17] 位运算
来源：http://lx.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hr.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bn.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cy.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ls.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ly.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://de.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ze.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pd.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://cq.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://yv.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://pv.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://se.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iw.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://uq.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wg.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://pn.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://lh.hnjuh.cn

[A19] 交换两个变量
来源：http://nr.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://ao.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mx.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://ll.521024.cn

TS:   [a, b] = [b, a];
来源：http://et.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://mn.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://cn.lnxyls.cn

Ruby: a, b = b, a
来源：http://vv.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://tr.szsharing.cn

[A20] 读取标准输入
来源：http://zx.gzmigu.cn

Py:   name = input("请输入：")
来源：http://cc.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zq.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ed.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://da.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://hr.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ma.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://yn.newstarts.cn

C#:   Console.ReadLine();
来源：http://ji.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://tn.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://zf.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mq.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://ku.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://yj.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://cb.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yx.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://os.521024.cn

C#:   3.14159.ToString("F2")
来源：http://wh.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://wm.hnjuh.cn

Py:   len(s)
来源：http://nb.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yl.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kp.huixiangedu.cn

TS:   s.length
来源：http://rk.huixiangedu.cn

Java: s.length()
来源：http://gd.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kv.szxytkj.cn

Ruby: s.length
来源：http://pw.jctech888.com.cn

C#:   s.Length
来源：http://ax.szxytkj.cn

[A23] 大小写转换
来源：http://fi.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ny.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yf.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ju.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jt.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bc.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xh.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oy.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pi.muxihuayi.cn

[A24] 去除首尾空白
来源：http://wg.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vt.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rt.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ut.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://te.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oq.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://yo.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ar.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://at.asd995.cn

[A25] 字符串比较
来源：http://lg.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://aw.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cy.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xg.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zd.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tw.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qp.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nz.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fs.gzmigu.cn

[A26] 类型转换总览
来源：http://cr.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fm.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ov.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mb.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://sg.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fp.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ar.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dg.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zt.bjjhwx.cn

================================================================================
来源：http://ra.bookmarksfly.cn

B. 流程控制
来源：http://un.hnjuh.cn

================================================================================
来源：http://ip.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://ro.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dx.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ro.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ck.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hl.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gb.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kt.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eh.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dw.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://lw.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ka.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jq.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gp.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ks.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oq.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fr.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lt.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qy.9csxet.cn

[B03] switch / match / case
来源：http://xz.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ma.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gj.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gp.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ao.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://il.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cd.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qj.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cy.hnjuh.cn

[B04] for 计数循环
来源：http://ql.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://kg.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ep.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tg.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rl.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nw.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zr.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://uj.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://il.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://qq.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://da.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dr.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vj.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tf.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kq.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zn.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://dn.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sa.asd995.cn

[B06] 遍历字典 / 对象
来源：http://pw.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://no.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hv.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tm.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fg.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kh.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://td.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ds.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ks.newstarts.cn

[B07] while 循环
来源：http://st.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://bd.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ww.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://wm.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://re.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://wa.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bv.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://oo.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://zy.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://sa.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://rd.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ml.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://pt.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://kt.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://cd.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tn.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ln.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://gq.newstarts.cn

[B09] break 与 continue
来源：http://qc.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://le.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://su.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ah.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hu.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yi.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mt.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qk.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fy.521024.cn

[B10] 遍历同时拿索引
来源：http://qn.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sl.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://md.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mr.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wb.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://at.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mc.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jk.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wf.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://ey.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://fg.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://rj.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sd.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kp.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://au.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fd.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://nq.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kd.nszjky.cn

[B12] 跳出多层循环
来源：http://qn.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zn.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gn.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gy.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mf.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://la.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fg.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ib.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dd.colortex.cn

[B13] 判断是否为数字
来源：http://sh.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://ft.gzmigu.cn

PHP:  is_numeric($x)
来源：http://vg.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ic.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aq.colortex.cn

Java: x instanceof Number
来源：http://re.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uu.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://wx.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://tv.colortex.cn

[B14] 判断值是否在集合内
来源：http://mq.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ft.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ni.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://lj.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://zv.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://we.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xl.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://io.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ep.huanxung.cn

[B15] 布尔运算与取反
来源：http://ke.huixinmuqiang.cn

Py:   a and b or not c
来源：http://lr.colortex.cn

PHP:  $a && $b || !$c
来源：http://ak.chemitech.net.cn

JS:   a && b || !c
来源：http://qb.521024.cn

TS:   a && b || !c
来源：http://dy.muxihuayi.cn

Java: a && b || !c
来源：http://pk.nszjky.cn

Go:   a && b || !c
来源：http://ra.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://ku.wgjwhj.cn

C#:   a && b || !c
来源：http://wd.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cv.panjiajie.cn

Py:   if not data: return
来源：http://cx.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://ct.huanxung.cn

JS:   if (!data) return;
来源：http://db.nicolike.cn

TS:   if (!data) return;
来源：http://lq.521024.cn

Java: if (data == null) return;
来源：http://fl.shxzukj.cn

Go:   if data == nil { return }
来源：http://ow.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://tl.haigaiapp.cn

C#:   if (data == null) return;
来源：http://ic.hahajie.cn

================================================================================
来源：http://dr.nszjky.cn

C. 函数与作用域
来源：http://ye.shxzskj.cn

================================================================================
来源：http://vk.huixinmuqiang.cn

[C01] 定义函数
来源：http://ma.521024.cn

Py:   def add(a, b): return a + b
来源：http://od.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ra.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://si.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dt.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nx.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cd.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://fy.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qb.szxytkj.cn

[C02] 默认参数
来源：http://kh.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://hr.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cc.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://lj.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ai.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dl.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://na.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://wk.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://ex.nicolike.cn

[C03] 可变参数
来源：http://mv.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://uo.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zl.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lm.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fk.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kr.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://da.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xo.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jj.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://bs.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lr.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sr.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zw.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ey.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://uz.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://bj.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://zq.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://lb.yuexingan06.cn

[C05] 返回多个值
来源：http://pf.szxytkj.cn

Py:   return a, b
来源：http://kw.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://kj.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://la.huixiangedu.cn

TS:   return { a, b };
来源：http://jp.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uu.yuntaijiaju.cn

Go:   return a, b
来源：http://fp.szsharing.cn

Ruby: return a, b
来源：http://ha.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://iz.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://pp.nszjky.cn

Py:   square = lambda x: x * x
来源：http://uh.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sw.hahajie.cn

JS:   const square = x => x * x;
来源：http://yt.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://uj.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nt.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ls.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://eh.nicolike.cn


<!-- 参考信息 -->