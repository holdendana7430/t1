代发 wailian999

Py:   "第一行\n第二行"
来源：http://vq.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://un.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://ve.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://dp.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://au.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://df.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://vm.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://za.colortex.cn

[A14] 注释写法
来源：http://rt.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yf.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dd.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://id.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://oi.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ts.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://he.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pe.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://qn.colortex.cn

[A15] 空值判断与默认值
来源：http://dc.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://pv.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://as.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://wr.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://jq.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://or.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://ww.asd995.cn

Ruby: value = data || "默认值"
来源：http://oj.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://tp.panjiajie.cn

[A16] 真假值判断规则
来源：http://eg.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hg.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://np.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tv.jctech888.com.cn

TS:   if (!x) {}
来源：http://jy.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://la.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xj.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yd.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ho.huanxung.cn

[A17] 位运算
来源：http://kq.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rd.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xq.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://my.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rc.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bi.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ru.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vq.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wp.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://jr.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://ef.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://ap.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hf.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://um.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://uc.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://va.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://wl.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://ac.shxzskj.cn

[A19] 交换两个变量
来源：http://ao.nszjky.cn

Py:   a, b = b, a
来源：http://ne.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yj.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://ft.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://bw.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://cn.9csxet.cn

Go:   a, b = b, a
来源：http://lz.nszjky.cn

Ruby: a, b = b, a
来源：http://gu.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://yf.shxzskj.cn

[A20] 读取标准输入
来源：http://nm.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://te.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bx.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qo.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://ik.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://ye.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fr.shxzukj.cn

Ruby: gets.chomp
来源：http://is.shxzskj.cn

C#:   Console.ReadLine();
来源：http://vf.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://eb.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://wp.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sc.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://gx.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://oz.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://hc.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yw.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://qv.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://tt.shxzukj.cn

[A22] 获取字符串长度
来源：http://bl.haigaiapp.cn

Py:   len(s)
来源：http://ht.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gk.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fy.asd995.cn

TS:   s.length
来源：http://mn.9csxet.cn

Java: s.length()
来源：http://qh.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gl.bjjhwx.cn

Ruby: s.length
来源：http://la.wgjwhj.cn

C#:   s.Length
来源：http://jk.hnjuh.cn

[A23] 大小写转换
来源：http://pq.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ks.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yq.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zv.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qw.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ja.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cp.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ix.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nc.newstarts.cn

[A24] 去除首尾空白
来源：http://ry.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zr.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://am.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cu.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mt.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://da.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://bm.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zl.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zo.huixinmuqiang.cn

[A25] 字符串比较
来源：http://ja.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://mq.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dt.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lp.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wy.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nm.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ub.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ui.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pv.nszjky.cn

[A26] 类型转换总览
来源：http://qy.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uu.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pv.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xt.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://yt.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fk.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ac.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ai.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wn.szxytkj.cn

================================================================================
来源：http://zy.hahajie.cn

B. 流程控制
来源：http://nl.bookmarksfly.cn

================================================================================
来源：http://ae.szsharing.cn

[B01] 条件判断 if / else
来源：http://mg.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ln.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fp.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tg.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vu.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jo.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jh.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ma.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ia.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://pa.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vr.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fi.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rc.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fb.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rx.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bj.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pt.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vl.yuexingan06.cn

[B03] switch / match / case
来源：http://go.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eo.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ul.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wp.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eg.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vx.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sn.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zq.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://az.nszjky.cn

[B04] for 计数循环
来源：http://uq.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://ug.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ex.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ox.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bw.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hn.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qi.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://ma.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pl.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://ct.newstarts.cn

Py:   for item in arr: print(item)
来源：http://ai.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vg.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sp.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wj.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zi.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kr.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://fz.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sg.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://wj.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ld.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gl.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vp.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mu.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vj.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jp.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ao.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://at.muxihuayi.cn

[B07] while 循环
来源：http://pc.asd995.cn

Py:   while i < 10: i += 1
来源：http://ce.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://av.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://gu.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://wf.colortex.cn

Java: while (i < 10) { i++; }
来源：http://la.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://se.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://rs.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://fi.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://nv.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://do.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ql.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://aq.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://nf.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://kf.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xf.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sx.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://ij.shtwfgs.cn

[B09] break 与 continue
来源：http://fk.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hf.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ex.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vs.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ck.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rm.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nt.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ey.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hv.asd995.cn

[B10] 遍历同时拿索引
来源：http://sw.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ss.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ey.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ew.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dg.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zd.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hn.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kg.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jl.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://mf.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ef.521024.cn

PHP:  range(0, 10, 2);
来源：http://rl.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yu.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sm.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mq.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bg.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://ez.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mv.colortex.cn

[B12] 跳出多层循环
来源：http://yy.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iv.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fy.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nr.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qp.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ws.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zl.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zd.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xh.colortex.cn

[B13] 判断是否为数字
来源：http://jx.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://yy.gzmigu.cn

PHP:  is_numeric($x)
来源：http://iw.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ma.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wc.lnxyls.cn

Java: x instanceof Number
来源：http://tn.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cg.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://se.shxzskj.cn

C#:   x is int or double or decimal
来源：http://mr.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://ex.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://my.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vb.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://vy.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://nj.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tj.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nt.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gc.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fy.asd995.cn

[B15] 布尔运算与取反
来源：http://zp.lnxyls.cn

Py:   a and b or not c
来源：http://rh.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://kd.gzmigu.cn

JS:   a && b || !c
来源：http://tn.521024.cn

TS:   a && b || !c
来源：http://op.shtwfgs.cn

Java: a && b || !c
来源：http://lc.shxzukj.cn

Go:   a && b || !c
来源：http://by.colortex.cn

Ruby: a && b || !c
来源：http://wb.newstarts.cn

C#:   a && b || !c
来源：http://qj.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eo.asd995.cn

Py:   if not data: return
来源：http://vt.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://ne.lnxyls.cn

JS:   if (!data) return;
来源：http://ek.hnjuh.cn

TS:   if (!data) return;
来源：http://sv.lnxyls.cn

Java: if (data == null) return;
来源：http://lw.hahajie.cn

Go:   if data == nil { return }
来源：http://if.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://nb.jctech888.com.cn

C#:   if (data == null) return;
来源：http://ct.yuntaijiaju.cn

================================================================================
来源：http://ni.huixiangedu.cn

C. 函数与作用域
来源：http://hm.szxytkj.cn

================================================================================
来源：http://dc.nszjky.cn

[C01] 定义函数
来源：http://co.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://rp.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ra.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://oq.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://do.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wr.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://no.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://ob.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://px.newstarts.cn

[C02] 默认参数
来源：http://ph.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://kw.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ka.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://cq.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ty.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://su.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bd.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://rc.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ui.shxzskj.cn

[C03] 可变参数
来源：http://bb.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://ex.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rm.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bx.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mz.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fp.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://po.yuexingan06.cn


<!-- 参考信息 -->