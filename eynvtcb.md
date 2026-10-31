代发 wailian999

Py:   "第一行\n第二行"
来源：http://hk.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://vn.colortex.cn

JS:   "第一行\n第二行"
来源：http://aq.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://kz.szxytkj.cn

Java: "第一行\n第二行"
来源：http://xk.colortex.cn

Go:   "第一行\n第二行"
来源：http://ia.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://tq.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://mt.panjiajie.cn

[A14] 注释写法
来源：http://av.hnjuh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gt.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dd.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://ai.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://ii.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iy.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://ty.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sa.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://hc.9csxet.cn

[A15] 空值判断与默认值
来源：http://qq.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://pc.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://rj.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://go.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://sn.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pq.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://bd.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://wk.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://di.lnxyls.cn

[A16] 真假值判断规则
来源：http://bs.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wv.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://es.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ub.jctech888.com.cn

TS:   if (!x) {}
来源：http://oe.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cv.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gf.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oz.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bm.bjjhwx.cn

[A17] 位运算
来源：http://xh.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ra.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ay.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ji.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cn.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lo.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://au.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mj.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ye.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://bh.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://pz.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://ff.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ue.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xq.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://sp.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jz.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://qz.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://kj.bookmarksfly.cn

[A19] 交换两个变量
来源：http://qj.szxytkj.cn

Py:   a, b = b, a
来源：http://aq.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pn.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://ko.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://pi.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://vb.bookmarksfly.cn

Go:   a, b = b, a
来源：http://vg.hahajie.cn

Ruby: a, b = b, a
来源：http://oq.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://xu.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://pt.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://pr.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sl.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ng.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://ne.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ue.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ya.lnxyls.cn

Ruby: gets.chomp
来源：http://aj.colortex.cn

C#:   Console.ReadLine();
来源：http://qm.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://jw.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://qv.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jt.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://km.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://jh.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://ri.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jl.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://rm.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://xc.huixiangedu.cn

[A22] 获取字符串长度
来源：http://wq.huixiangedu.cn

Py:   len(s)
来源：http://ev.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pc.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rk.9csxet.cn

TS:   s.length
来源：http://lj.szsharing.cn

Java: s.length()
来源：http://nj.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lm.szxytkj.cn

Ruby: s.length
来源：http://ho.panjiajie.cn

C#:   s.Length
来源：http://nw.huixiangedu.cn

[A23] 大小写转换
来源：http://fb.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dz.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yg.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://po.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tk.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bk.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vf.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xc.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vu.jctech888.com.cn

[A24] 去除首尾空白
来源：http://mt.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bl.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hb.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pd.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bm.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zf.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://nm.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ky.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nq.huixinmuqiang.cn

[A25] 字符串比较
来源：http://wv.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://fg.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://db.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nm.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xy.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://st.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mj.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mf.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sm.521024.cn

[A26] 类型转换总览
来源：http://gg.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yz.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pn.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hm.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://uo.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://av.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mp.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tw.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rr.jctech888.com.cn

================================================================================
来源：http://wc.huanxung.cn

B. 流程控制
来源：http://gt.asd995.cn

================================================================================
来源：http://fq.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://sh.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zc.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hp.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pa.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fk.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://it.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fc.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ix.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xp.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://uo.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ps.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ka.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ru.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://op.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wl.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aj.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://er.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qp.lnxyls.cn

[B03] switch / match / case
来源：http://yp.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://df.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hm.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gu.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tn.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ml.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ua.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cq.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mj.bjjhwx.cn

[B04] for 计数循环
来源：http://qc.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://rq.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zc.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ee.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qt.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zm.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://si.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://wv.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ha.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://ca.521024.cn

Py:   for item in arr: print(item)
来源：http://mw.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gv.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://su.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fa.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tb.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oi.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://eq.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uc.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://po.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://br.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ew.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qe.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fr.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bl.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ut.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ep.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fc.chemitech.net.cn

[B07] while 循环
来源：http://qo.nszjky.cn

Py:   while i < 10: i += 1
来源：http://ob.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://an.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://yc.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://qs.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://xw.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aw.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://tf.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://hj.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://un.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://qr.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pf.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://jc.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://he.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://eh.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ve.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bi.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://hg.lnxyls.cn

[B09] break 与 continue
来源：http://yl.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://av.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://im.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rc.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oo.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://df.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pr.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nb.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://vz.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ow.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bk.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wr.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ry.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mx.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bl.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mp.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ve.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://hk.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://om.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://up.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mo.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yz.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uz.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wk.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://tl.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tu.gzmigu.cn

[B12] 跳出多层循环
来源：http://jt.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hf.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ap.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uq.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ac.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jg.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oc.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xm.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oa.haigaiapp.cn

[B13] 判断是否为数字
来源：http://tk.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://az.nszjky.cn

PHP:  is_numeric($x)
来源：http://gl.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://am.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xs.hnjuh.cn

Java: x instanceof Number
来源：http://jm.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hc.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://jj.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://bt.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://ir.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vf.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iq.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://uo.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://sc.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://aj.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ps.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zm.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ni.shxzskj.cn

[B15] 布尔运算与取反
来源：http://fv.panjiajie.cn

Py:   a and b or not c
来源：http://jd.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://sg.bookmarksfly.cn

JS:   a && b || !c
来源：http://gi.newstarts.cn

TS:   a && b || !c
来源：http://uo.shxzukj.cn

Java: a && b || !c
来源：http://br.chemitech.net.cn

Go:   a && b || !c
来源：http://am.szxytkj.cn

Ruby: a && b || !c
来源：http://ni.huanxung.cn

C#:   a && b || !c
来源：http://ff.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uc.muxihuayi.cn

Py:   if not data: return
来源：http://nv.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://cv.szxytkj.cn

JS:   if (!data) return;
来源：http://tm.lnxyls.cn

TS:   if (!data) return;
来源：http://ti.9csxet.cn

Java: if (data == null) return;
来源：http://cr.gzmigu.cn

Go:   if data == nil { return }
来源：http://fa.shxzukj.cn

Ruby: return if data.nil?
来源：http://sw.haigaiapp.cn

C#:   if (data == null) return;
来源：http://dv.szxytkj.cn

================================================================================
来源：http://qq.asd995.cn

C. 函数与作用域
来源：http://rz.huixinmuqiang.cn

================================================================================
来源：http://qm.shtwfgs.cn

[C01] 定义函数
来源：http://or.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://ag.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hp.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://ym.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pq.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uc.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://it.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://fh.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lz.bjjhwx.cn

[C02] 默认参数
来源：http://jm.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://ig.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lm.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://yy.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ls.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xg.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dh.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://cr.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://lq.jctech888.com.cn

[C03] 可变参数
来源：http://mb.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://gs.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hj.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nw.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dh.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://is.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fv.huixiangedu.cn


<!-- 参考信息 -->