代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://wd.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ea.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://ax.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zh.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://wj.hahajie.cn

[A15] 空值判断与默认值
来源：http://li.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://wd.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://xe.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://ew.521024.cn

TS:   const value = data ?? "默认值";
来源：http://tg.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rl.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://la.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://fb.521024.cn

C#:   var value = data ?? "默认值";
来源：http://za.shxzukj.cn

[A16] 真假值判断规则
来源：http://qt.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dj.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ph.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lr.shxzukj.cn

TS:   if (!x) {}
来源：http://dg.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ww.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rr.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gy.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vp.yuntaijiaju.cn

[A17] 位运算
来源：http://dc.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qx.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ly.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vw.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qe.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tg.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vp.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hq.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pf.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://pk.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://tv.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://ou.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qw.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zc.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://fx.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oa.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://cf.colortex.cn

C#:   (int)'A'; (char)65
来源：http://qb.shxzskj.cn

[A19] 交换两个变量
来源：http://pn.szxytkj.cn

Py:   a, b = b, a
来源：http://od.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sv.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://oq.521024.cn

TS:   [a, b] = [b, a];
来源：http://wr.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://td.haigaiapp.cn

Go:   a, b = b, a
来源：http://yd.shtwfgs.cn

Ruby: a, b = b, a
来源：http://of.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://hy.shxzskj.cn

[A20] 读取标准输入
来源：http://js.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://qj.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cw.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gx.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://yj.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://fe.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ea.chemitech.net.cn

Ruby: gets.chomp
来源：http://mk.newstarts.cn

C#:   Console.ReadLine();
来源：http://oi.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://en.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://ju.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cs.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://lx.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://rm.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://lu.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dm.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://pr.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://jv.9csxet.cn

[A22] 获取字符串长度
来源：http://oc.shtwfgs.cn

Py:   len(s)
来源：http://ym.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ri.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hh.bookmarksfly.cn

TS:   s.length
来源：http://ga.shxzskj.cn

Java: s.length()
来源：http://sk.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aw.hnjuh.cn

Ruby: s.length
来源：http://cf.jianghongdianzi.cn

C#:   s.Length
来源：http://eu.szsharing.cn

[A23] 大小写转换
来源：http://wk.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ds.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wh.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hw.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wi.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hs.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cb.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mo.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jv.shtwfgs.cn

[A24] 去除首尾空白
来源：http://sf.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mb.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://po.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://og.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zp.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vz.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://jc.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://op.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pt.hahajie.cn

[A25] 字符串比较
来源：http://yf.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://et.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yt.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vk.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hx.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zc.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gi.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fc.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ct.szxytkj.cn

[A26] 类型转换总览
来源：http://sq.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sa.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yv.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://no.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://jy.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jo.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dx.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nd.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zp.colortex.cn

================================================================================
来源：http://ao.nszjky.cn

B. 流程控制
来源：http://gn.wgjwhj.cn

================================================================================
来源：http://hz.hnjuh.cn

[B01] 条件判断 if / else
来源：http://xh.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cj.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://df.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qd.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rg.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lp.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tu.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yo.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cg.newstarts.cn

[B02] 多分支 else if / elif
来源：http://gx.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ff.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pp.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zp.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qw.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://na.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ti.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oz.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rt.shxzukj.cn

[B03] switch / match / case
来源：http://wi.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nd.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://en.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uz.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ni.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://it.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lc.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qn.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zu.gzmigu.cn

[B04] for 计数循环
来源：http://wz.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://xu.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bt.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://re.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tc.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jk.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vv.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://wv.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wx.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://hh.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://cv.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xy.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://go.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hp.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ql.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://za.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://no.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bv.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://tm.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hg.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nl.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qf.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://im.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nq.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wg.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dv.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qe.haigaiapp.cn

[B07] while 循环
来源：http://ca.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://gc.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rz.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://ai.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://is.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://dk.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ct.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://kl.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://jm.521024.cn

[B08] do-while（至少执行一次）
来源：http://ri.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://se.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ue.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://sg.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://ew.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://tv.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jm.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ue.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://jd.521024.cn

[B09] break 与 continue
来源：http://cm.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pv.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wf.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gj.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qi.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dd.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ye.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zt.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.nicolike.cn

[B10] 遍历同时拿索引
来源：http://mb.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zb.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://az.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ap.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ac.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bt.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qc.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ak.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rs.521024.cn

[B11] 生成数字序列 / 区间
来源：http://vl.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://op.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://qz.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ke.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cx.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lr.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mc.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://ts.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lz.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://iy.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ix.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fm.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xh.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pi.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://as.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yp.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ty.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tb.9csxet.cn

[B13] 判断是否为数字
来源：http://it.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://sp.521024.cn

PHP:  is_numeric($x)
来源：http://dc.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qd.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ne.lnxyls.cn

Java: x instanceof Number
来源：http://xt.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ra.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://jw.nszjky.cn

C#:   x is int or double or decimal
来源：http://vz.9csxet.cn

[B14] 判断值是否在集合内
来源：http://tt.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qh.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pf.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://vh.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://cq.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ms.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zc.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zx.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qo.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://nt.shxzukj.cn

Py:   a and b or not c
来源：http://np.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://pa.521024.cn

JS:   a && b || !c
来源：http://wv.shxzukj.cn

TS:   a && b || !c
来源：http://cm.szxytkj.cn

Java: a && b || !c
来源：http://ps.521024.cn

Go:   a && b || !c
来源：http://yo.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://ay.9csxet.cn

C#:   a && b || !c
来源：http://xy.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nn.haigaiapp.cn

Py:   if not data: return
来源：http://fs.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://yc.szsharing.cn

JS:   if (!data) return;
来源：http://ux.asd995.cn

TS:   if (!data) return;
来源：http://qz.newstarts.cn

Java: if (data == null) return;
来源：http://xr.newstarts.cn

Go:   if data == nil { return }
来源：http://uo.huanxung.cn

Ruby: return if data.nil?
来源：http://zc.lnxyls.cn

C#:   if (data == null) return;
来源：http://ka.bjjhwx.cn

================================================================================
来源：http://eo.hahajie.cn

C. 函数与作用域
来源：http://mu.jctech888.com.cn

================================================================================
来源：http://ja.yuexingan06.cn

[C01] 定义函数
来源：http://yy.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://bd.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kl.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://xs.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ql.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fd.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ct.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://zj.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sk.nicolike.cn

[C02] 默认参数
来源：http://sq.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://qg.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yn.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://dd.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hl.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vf.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fk.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://xb.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://ve.nicolike.cn

[C03] 可变参数
来源：http://vo.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://rp.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://es.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rr.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kx.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ol.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://je.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bp.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ge.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://tp.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nh.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://px.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://se.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ut.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://by.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://uf.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://fa.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://bd.521024.cn

[C05] 返回多个值
来源：http://mi.haigaiapp.cn


<!-- 参考信息 -->