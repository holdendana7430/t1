代发 wailian999

Py:   "第一行\n第二行"
来源：http://xq.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://wi.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://pr.asd995.cn

TS:   "第一行\n第二行"
来源：http://kt.hnjuh.cn

Java: "第一行\n第二行"
来源：http://qr.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://vp.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://eh.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://hv.gzmigu.cn

[A14] 注释写法
来源：http://bh.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wv.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xj.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://xv.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://ot.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xg.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://ae.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gn.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://mm.panjiajie.cn

[A15] 空值判断与默认值
来源：http://ip.panjiajie.cn

Py:   value = data or "默认值"
来源：http://zb.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://bs.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://yx.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://qm.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wi.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://jp.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://un.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://ll.huixiangedu.cn

[A16] 真假值判断规则
来源：http://ou.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ta.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://di.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zs.haigaiapp.cn

TS:   if (!x) {}
来源：http://de.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rr.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jk.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fh.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jl.haigaiapp.cn

[A17] 位运算
来源：http://va.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yq.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jn.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://id.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jr.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lo.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vc.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ew.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://qf.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://cd.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://rk.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wn.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ue.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://pw.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wv.521024.cn

Ruby: "A".ord; 65.chr
来源：http://mk.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://oe.huixiangedu.cn

[A19] 交换两个变量
来源：http://qy.haigaiapp.cn

Py:   a, b = b, a
来源：http://xt.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qq.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://ei.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://ow.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://kp.huanxung.cn

Go:   a, b = b, a
来源：http://xn.nszjky.cn

Ruby: a, b = b, a
来源：http://nv.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://xt.yuexingan06.cn

[A20] 读取标准输入
来源：http://fm.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://ju.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pq.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://px.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://sn.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://kh.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qm.nicolike.cn

Ruby: gets.chomp
来源：http://gl.nszjky.cn

C#:   Console.ReadLine();
来源：http://jb.521024.cn

[A21] 保留指定小数位输出
来源：http://lw.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://rc.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hv.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://vh.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://ok.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://yw.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://td.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://zo.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://yu.hahajie.cn

[A22] 获取字符串长度
来源：http://pp.huanxung.cn

Py:   len(s)
来源：http://ut.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rn.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cz.huixiangedu.cn

TS:   s.length
来源：http://tf.huixinmuqiang.cn

Java: s.length()
来源：http://ni.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bn.shxzskj.cn

Ruby: s.length
来源：http://jm.huixiangedu.cn

C#:   s.Length
来源：http://zw.yuntaijiaju.cn

[A23] 大小写转换
来源：http://rm.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mn.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rx.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nf.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cb.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ff.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ao.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cm.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kx.panjiajie.cn

[A24] 去除首尾空白
来源：http://ww.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ad.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ej.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zc.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xc.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sr.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://nm.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dt.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tz.newstarts.cn

[A25] 字符串比较
来源：http://ib.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://jm.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://au.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xr.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bw.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uo.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zn.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pf.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lj.szxytkj.cn

[A26] 类型转换总览
来源：http://qt.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dp.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hy.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ot.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://cj.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wv.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fk.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sx.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bq.lnxyls.cn

================================================================================
来源：http://ln.wgjwhj.cn

B. 流程控制
来源：http://ic.muxihuayi.cn

================================================================================
来源：http://ob.hahajie.cn

[B01] 条件判断 if / else
来源：http://yo.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://li.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ga.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://op.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pb.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pt.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kb.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ii.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ow.colortex.cn

[B02] 多分支 else if / elif
来源：http://fz.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oq.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sl.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dl.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tb.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ff.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ja.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wa.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wm.bookmarksfly.cn

[B03] switch / match / case
来源：http://gk.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ur.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pu.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dg.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tp.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tf.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rp.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rt.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lt.huixiangedu.cn

[B04] for 计数循环
来源：http://jy.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://zj.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zw.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://md.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hk.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bt.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zj.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://io.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nv.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://jr.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ch.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aw.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ql.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rx.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://po.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://as.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://vy.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tg.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://vi.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cs.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jq.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pn.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://by.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jn.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zx.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zp.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ng.newstarts.cn

[B07] while 循环
来源：http://qt.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://me.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qz.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://qe.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://lv.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://gb.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bq.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://xz.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://xg.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://zz.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ny.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://za.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://fl.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://bz.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://vj.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jz.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vs.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://gs.yuexingan06.cn

[B09] break 与 continue
来源：http://rr.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fl.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qp.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wt.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://td.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zx.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jf.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cx.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hq.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://oy.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kp.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ce.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sn.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dx.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://om.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zh.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pl.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://qr.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://kn.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://uh.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sg.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ys.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fd.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xd.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://it.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dx.panjiajie.cn

[B12] 跳出多层循环
来源：http://nd.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sp.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ub.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://be.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bq.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vr.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ql.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://of.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ke.shxzukj.cn

[B13] 判断是否为数字
来源：http://be.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://wn.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://in.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wv.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uz.521024.cn

Java: x instanceof Number
来源：http://ev.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kv.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://dl.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://gs.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://sk.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lk.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ps.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://mm.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://ry.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bk.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vm.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yp.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tx.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://qp.colortex.cn

Py:   a and b or not c
来源：http://xm.hahajie.cn

PHP:  $a && $b || !$c
来源：http://dm.wgjwhj.cn

JS:   a && b || !c
来源：http://yq.shtwfgs.cn

TS:   a && b || !c
来源：http://pq.huanxung.cn

Java: a && b || !c
来源：http://ik.asd995.cn

Go:   a && b || !c
来源：http://dh.hnjuh.cn

Ruby: a && b || !c
来源：http://lk.huixiangedu.cn

C#:   a && b || !c
来源：http://rq.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gc.panjiajie.cn

Py:   if not data: return
来源：http://lt.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://vh.szsharing.cn

JS:   if (!data) return;
来源：http://gi.lnxyls.cn

TS:   if (!data) return;
来源：http://rl.shxzukj.cn

Java: if (data == null) return;
来源：http://xc.panjiajie.cn

Go:   if data == nil { return }
来源：http://xt.haigaiapp.cn

Ruby: return if data.nil?
来源：http://ju.lnxyls.cn

C#:   if (data == null) return;
来源：http://fo.hnjuh.cn

================================================================================
来源：http://oq.jctech888.com.cn

C. 函数与作用域
来源：http://kh.haigaiapp.cn

================================================================================
来源：http://rt.hahajie.cn

[C01] 定义函数
来源：http://dy.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://wl.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iv.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://zv.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lg.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dx.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zh.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://gu.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ss.huanxung.cn

[C02] 默认参数
来源：http://os.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://ug.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gj.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://hl.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ax.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ik.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bn.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://to.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://tj.newstarts.cn

[C03] 可变参数
来源：http://ni.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://xz.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eo.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jn.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://up.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://id.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eq.huanxung.cn


<!-- 参考信息 -->