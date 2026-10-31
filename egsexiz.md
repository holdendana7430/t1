代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://ki.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sz.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://xb.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bl.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://ao.hahajie.cn

[A15] 空值判断与默认值
来源：http://fl.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://rw.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://ya.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://ao.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://wo.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jj.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://jb.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://fs.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://wy.nszjky.cn

[A16] 真假值判断规则
来源：http://gy.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qt.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oo.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pb.wgjwhj.cn

TS:   if (!x) {}
来源：http://ll.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ci.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://re.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://my.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rv.wgjwhj.cn

[A17] 位运算
来源：http://df.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nb.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://az.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://li.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fb.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gt.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xc.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hq.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ar.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://ed.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://sw.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://jp.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wv.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fq.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://ll.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xj.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://jx.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://fv.yuexingan06.cn

[A19] 交换两个变量
来源：http://fv.bjjhwx.cn

Py:   a, b = b, a
来源：http://ih.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bc.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://mn.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://jy.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://wo.shxzukj.cn

Go:   a, b = b, a
来源：http://ek.nszjky.cn

Ruby: a, b = b, a
来源：http://pq.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://yp.chemitech.net.cn

[A20] 读取标准输入
来源：http://yj.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://oo.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zu.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cs.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://lr.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://cn.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ai.asd995.cn

Ruby: gets.chomp
来源：http://xy.shxzukj.cn

C#:   Console.ReadLine();
来源：http://pg.nicolike.cn

[A21] 保留指定小数位输出
来源：http://hs.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://yl.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ze.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://il.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://mf.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://uh.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xi.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://xw.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://nn.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://tu.yuntaijiaju.cn

Py:   len(s)
来源：http://xv.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ne.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fh.szsharing.cn

TS:   s.length
来源：http://sh.9csxet.cn

Java: s.length()
来源：http://vz.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dn.szsharing.cn

Ruby: s.length
来源：http://mt.yuexingan06.cn

C#:   s.Length
来源：http://hc.shtwfgs.cn

[A23] 大小写转换
来源：http://oi.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ne.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bh.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bb.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bg.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ti.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fg.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vv.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lj.shtwfgs.cn

[A24] 去除首尾空白
来源：http://lq.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vx.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zj.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iz.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yq.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pk.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://gw.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jm.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fz.newstarts.cn

[A25] 字符串比较
来源：http://rf.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://nq.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qc.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xf.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ps.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rp.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wt.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tx.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hv.nicolike.cn

[A26] 类型转换总览
来源：http://re.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cr.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tg.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pp.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://mp.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://su.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ly.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nw.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oq.bookmarksfly.cn

================================================================================
来源：http://wh.gzmigu.cn

B. 流程控制
来源：http://zh.hnjuh.cn

================================================================================
来源：http://oc.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://ew.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eq.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://om.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vt.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zu.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sw.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cv.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yr.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ti.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://zi.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aw.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aa.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://is.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oy.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uw.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nt.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hq.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yb.bookmarksfly.cn

[B03] switch / match / case
来源：http://wz.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ck.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rh.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ni.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kk.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ek.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qs.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qd.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qb.hahajie.cn

[B04] for 计数循环
来源：http://nc.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://zp.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yr.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zi.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ys.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://si.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uk.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://qt.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://je.521024.cn

[B05] 遍历数组 / 列表
来源：http://zi.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://qh.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jx.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tn.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://up.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tp.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ua.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://qg.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dw.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://rd.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zq.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pm.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://me.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://df.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://am.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ua.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nt.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ce.lnxyls.cn

[B07] while 循环
来源：http://ni.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://fl.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fb.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://vc.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://pl.521024.cn

Java: while (i < 10) { i++; }
来源：http://sp.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hl.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://lb.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://ne.colortex.cn

[B08] do-while（至少执行一次）
来源：http://gb.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ef.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sv.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://sg.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://ux.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://hp.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nh.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ee.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://gk.jianghongdianzi.cn

[B09] break 与 continue
来源：http://ga.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ux.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iq.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ce.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eg.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sf.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zq.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ag.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dg.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://ek.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://po.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ms.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cs.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qm.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fo.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fn.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zp.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rt.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://tz.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://ch.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://if.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nw.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wk.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://do.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nd.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://jg.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qg.szxytkj.cn

[B12] 跳出多层循环
来源：http://zl.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xj.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://te.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kk.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fq.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vs.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kf.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wp.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dc.yuexingan06.cn

[B13] 判断是否为数字
来源：http://cn.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://we.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://rs.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ja.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wd.huixiangedu.cn

Java: x instanceof Number
来源：http://bi.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jf.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://hq.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://fj.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://bz.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://db.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bo.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://yg.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://gv.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oc.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://op.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pu.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lc.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://ac.shxzukj.cn

Py:   a and b or not c
来源：http://uw.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://og.haigaiapp.cn

JS:   a && b || !c
来源：http://ae.panjiajie.cn

TS:   a && b || !c
来源：http://yl.huixiangedu.cn

Java: a && b || !c
来源：http://aq.hnjuh.cn

Go:   a && b || !c
来源：http://lh.nszjky.cn

Ruby: a && b || !c
来源：http://rn.yuexingan06.cn

C#:   a && b || !c
来源：http://fr.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xm.colortex.cn

Py:   if not data: return
来源：http://bk.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://aa.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://wy.muxihuayi.cn

TS:   if (!data) return;
来源：http://ry.panjiajie.cn

Java: if (data == null) return;
来源：http://pu.szsharing.cn

Go:   if data == nil { return }
来源：http://mz.bjjhwx.cn

Ruby: return if data.nil?
来源：http://eq.nszjky.cn

C#:   if (data == null) return;
来源：http://bn.lnxyls.cn

================================================================================
来源：http://rr.huixinmuqiang.cn

C. 函数与作用域
来源：http://lp.panjiajie.cn

================================================================================
来源：http://bw.9csxet.cn

[C01] 定义函数
来源：http://bn.asd995.cn

Py:   def add(a, b): return a + b
来源：http://im.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ud.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://dl.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zx.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rz.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qn.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://bz.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://df.nicolike.cn

[C02] 默认参数
来源：http://ya.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://ma.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wz.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://mo.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yp.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oc.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qn.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://uu.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://lx.bjjhwx.cn

[C03] 可变参数
来源：http://vb.521024.cn

Py:   def total(*args): return sum(args)
来源：http://kh.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ny.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://en.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tg.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mv.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rm.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ex.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cx.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://ol.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://in.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nb.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ga.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ee.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://sh.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://qq.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://qp.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://ks.colortex.cn

[C05] 返回多个值
来源：http://mu.bookmarksfly.cn


<!-- 参考信息 -->