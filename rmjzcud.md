代发 wailian999

Py:   "第一行\n第二行"
来源：http://hw.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://aq.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://ko.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://oy.gzmigu.cn

Java: "第一行\n第二行"
来源：http://sq.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://vl.colortex.cn

Ruby: "第一行\n第二行"
来源：http://nt.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://pa.panjiajie.cn

[A14] 注释写法
来源：http://ns.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ad.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nl.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://lw.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://zl.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yy.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://gl.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cl.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://aj.szxytkj.cn

[A15] 空值判断与默认值
来源：http://jm.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://mh.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://pj.521024.cn

JS:   const value = data ?? "默认值";
来源：http://lt.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://gx.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qz.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://jp.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://hu.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://ft.jctech888.com.cn

[A16] 真假值判断规则
来源：http://xg.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wq.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xl.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://er.huixiangedu.cn

TS:   if (!x) {}
来源：http://vr.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nn.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://an.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bt.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tc.shxzskj.cn

[A17] 位运算
来源：http://zb.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://em.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ob.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kr.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qz.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ow.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vj.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qf.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iz.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://im.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://pf.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://mo.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cs.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pu.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://jm.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kj.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://ni.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://jj.jctech888.com.cn

[A19] 交换两个变量
来源：http://sv.yuntaijiaju.cn

Py:   a, b = b, a
来源：http://fe.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ds.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://zh.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://jy.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://tf.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://pv.muxihuayi.cn

Ruby: a, b = b, a
来源：http://ln.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://ic.huanxung.cn

[A20] 读取标准输入
来源：http://sc.nicolike.cn

Py:   name = input("请输入：")
来源：http://pd.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dq.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ou.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://ms.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://em.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dp.shtwfgs.cn

Ruby: gets.chomp
来源：http://ib.gzmigu.cn

C#:   Console.ReadLine();
来源：http://jd.521024.cn

[A21] 保留指定小数位输出
来源：http://gs.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://mm.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ri.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://tk.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://ov.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://ph.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://op.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://df.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://sh.shxzskj.cn

[A22] 获取字符串长度
来源：http://hj.shxzskj.cn

Py:   len(s)
来源：http://wk.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nq.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pw.shtwfgs.cn

TS:   s.length
来源：http://em.9csxet.cn

Java: s.length()
来源：http://kw.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eh.hnjuh.cn

Ruby: s.length
来源：http://as.colortex.cn

C#:   s.Length
来源：http://or.asd995.cn

[A23] 大小写转换
来源：http://jp.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vr.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dv.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nx.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zq.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lk.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hb.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qj.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ab.nicolike.cn

[A24] 去除首尾空白
来源：http://xp.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tb.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kk.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nj.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nc.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tw.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://ib.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gn.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pz.yuntaijiaju.cn

[A25] 字符串比较
来源：http://lb.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://ih.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dj.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rh.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vq.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ti.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cy.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fl.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dw.jctech888.com.cn

[A26] 类型转换总览
来源：http://is.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sg.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://us.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bg.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://cd.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pe.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ay.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wu.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nz.huixiangedu.cn

================================================================================
来源：http://go.haigaiapp.cn

B. 流程控制
来源：http://iz.bookmarksfly.cn

================================================================================
来源：http://bq.nszjky.cn

[B01] 条件判断 if / else
来源：http://nk.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sy.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lh.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://to.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qv.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lu.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qi.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://en.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vc.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://qu.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ce.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nh.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hs.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pl.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ge.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ol.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://af.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vq.yuexingan06.cn

[B03] switch / match / case
来源：http://na.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hm.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mk.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sr.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jw.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qu.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lb.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oj.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eq.shxzskj.cn

[B04] for 计数循环
来源：http://gz.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://cp.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yl.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vo.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gg.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zj.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://od.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://ky.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zo.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://rh.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://de.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uf.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://og.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://we.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qq.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fl.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://no.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vh.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://gi.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gy.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gg.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ce.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hn.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://im.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jz.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lq.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bv.yuexingan06.cn

[B07] while 循环
来源：http://za.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://jd.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lr.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://hm.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://cv.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://nk.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jj.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://nx.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://yx.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://je.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://hf.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cj.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://ay.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://zn.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://vu.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rb.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xe.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://in.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ug.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dh.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xp.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ex.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gj.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ps.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mk.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sa.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://vc.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xk.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gq.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vt.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wk.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tv.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kf.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xu.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lm.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://ds.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://nv.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://yh.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uf.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gz.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mz.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yd.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://yf.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gc.nicolike.cn

[B12] 跳出多层循环
来源：http://me.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://om.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dm.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kl.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wy.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://on.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kh.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wl.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jp.chemitech.net.cn

[B13] 判断是否为数字
来源：http://rv.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://jz.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://ke.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cs.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ta.shtwfgs.cn

Java: x instanceof Number
来源：http://mp.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fl.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://jm.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://to.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://di.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kn.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tz.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ul.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://hh.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wi.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wc.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ek.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ku.nszjky.cn

[B15] 布尔运算与取反
来源：http://li.huanxung.cn

Py:   a and b or not c
来源：http://ue.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://ae.nszjky.cn

JS:   a && b || !c
来源：http://oo.huixinmuqiang.cn

TS:   a && b || !c
来源：http://wk.shtwfgs.cn

Java: a && b || !c
来源：http://bd.newstarts.cn

Go:   a && b || !c
来源：http://jy.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://mb.shxzskj.cn

C#:   a && b || !c
来源：http://tg.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hl.newstarts.cn

Py:   if not data: return
来源：http://fv.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://lg.panjiajie.cn

JS:   if (!data) return;
来源：http://fa.nicolike.cn

TS:   if (!data) return;
来源：http://ak.bjjhwx.cn

Java: if (data == null) return;
来源：http://ck.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://jb.huanxung.cn

Ruby: return if data.nil?
来源：http://ji.huixiangedu.cn

C#:   if (data == null) return;
来源：http://as.panjiajie.cn

================================================================================
来源：http://vd.szxytkj.cn

C. 函数与作用域
来源：http://no.haigaiapp.cn

================================================================================
来源：http://hi.szxytkj.cn

[C01] 定义函数
来源：http://gp.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://wf.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zk.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://ca.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ta.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cu.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ey.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://wc.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xi.9csxet.cn

[C02] 默认参数
来源：http://ww.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://jp.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ft.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://vy.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ei.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yb.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gg.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://vs.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://xn.gzmigu.cn

[C03] 可变参数
来源：http://dn.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://zg.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sp.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ah.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hu.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ch.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oc.hahajie.cn


<!-- 参考信息 -->