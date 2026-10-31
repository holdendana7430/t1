代发 wailian999

Py:   "第一行\n第二行"
来源：http://sf.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://ew.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://tf.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://dn.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://rs.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://qm.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://ex.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://eb.nicolike.cn

[A14] 注释写法
来源：http://xz.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kp.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ca.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://ir.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://rv.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fy.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://gd.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ld.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://aq.hnjuh.cn

[A15] 空值判断与默认值
来源：http://nm.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://ot.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://rk.521024.cn

JS:   const value = data ?? "默认值";
来源：http://an.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://gm.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vn.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://rv.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://bq.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://ny.9csxet.cn

[A16] 真假值判断规则
来源：http://np.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://we.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xq.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ab.newstarts.cn

TS:   if (!x) {}
来源：http://vr.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ee.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bu.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ve.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oi.muxihuayi.cn

[A17] 位运算
来源：http://zg.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fx.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qp.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xx.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ds.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wj.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vy.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cq.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ga.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://ir.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://ab.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://te.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ha.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mv.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://jj.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zv.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://tr.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://ij.huixiangedu.cn

[A19] 交换两个变量
来源：http://es.9csxet.cn

Py:   a, b = b, a
来源：http://ww.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qy.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://dm.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://yu.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://kk.asd995.cn

Go:   a, b = b, a
来源：http://zh.shtwfgs.cn

Ruby: a, b = b, a
来源：http://bk.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://jo.shxzskj.cn

[A20] 读取标准输入
来源：http://hh.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://kh.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xz.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ah.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://zi.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://fd.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://da.shxzskj.cn

Ruby: gets.chomp
来源：http://ga.nszjky.cn

C#:   Console.ReadLine();
来源：http://dn.hahajie.cn

[A21] 保留指定小数位输出
来源：http://ca.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://zh.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ly.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://fe.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://xe.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://ch.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://by.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://gk.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://qg.jctech888.com.cn

[A22] 获取字符串长度
来源：http://uj.huixiangedu.cn

Py:   len(s)
来源：http://tq.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bp.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dx.asd995.cn

TS:   s.length
来源：http://ow.hahajie.cn

Java: s.length()
来源：http://jf.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uq.bjjhwx.cn

Ruby: s.length
来源：http://cz.hnjuh.cn

C#:   s.Length
来源：http://mr.jianghongdianzi.cn

[A23] 大小写转换
来源：http://zr.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dl.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lu.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xx.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nj.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://do.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nm.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rk.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kr.chemitech.net.cn

[A24] 去除首尾空白
来源：http://fp.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zv.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bg.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dt.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://im.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qb.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://us.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xl.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://op.hahajie.cn

[A25] 字符串比较
来源：http://zf.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://ao.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ii.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dc.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ua.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rb.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lr.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ds.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pp.huanxung.cn

[A26] 类型转换总览
来源：http://gr.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bu.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lf.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vi.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://wk.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bt.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mr.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fi.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vq.bookmarksfly.cn

================================================================================
来源：http://qm.shxzskj.cn

B. 流程控制
来源：http://ac.jctech888.com.cn

================================================================================
来源：http://zg.9csxet.cn

[B01] 条件判断 if / else
来源：http://xh.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lz.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lz.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bq.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ie.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://md.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ze.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ql.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zr.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://yx.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xk.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rp.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://al.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hn.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ic.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ii.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xt.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yy.newstarts.cn

[B03] switch / match / case
来源：http://by.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nz.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fv.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cy.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wi.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ow.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zj.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ki.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pu.szxytkj.cn

[B04] for 计数循环
来源：http://zu.asd995.cn

Py:   for i in range(10): print(i)
来源：http://lg.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eu.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ag.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tt.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gj.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ua.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://zf.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nh.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://lt.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://fb.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ue.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hw.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vq.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lo.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jw.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://cp.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qy.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://tv.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ot.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fu.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qp.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ga.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fn.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sz.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ej.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ym.asd995.cn

[B07] while 循环
来源：http://ry.nszjky.cn

Py:   while i < 10: i += 1
来源：http://lj.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hv.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://tt.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://il.521024.cn

Java: while (i < 10) { i++; }
来源：http://gs.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wq.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://my.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://eu.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://en.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://on.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qy.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://gc.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://yb.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://jh.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ko.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jm.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://qw.shxzukj.cn

[B09] break 与 continue
来源：http://xh.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zo.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yt.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://na.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fo.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mt.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qm.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pm.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ll.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://wz.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aw.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ub.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://am.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mq.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zv.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://et.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ng.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://as.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://fu.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://ms.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://lb.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lm.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dg.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pd.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lm.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://zh.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://os.huixiangedu.cn

[B12] 跳出多层循环
来源：http://np.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://te.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gv.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xt.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vz.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://al.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hs.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jl.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jo.asd995.cn

[B13] 判断是否为数字
来源：http://vv.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://ga.szsharing.cn

PHP:  is_numeric($x)
来源：http://ob.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://re.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sw.wgjwhj.cn

Java: x instanceof Number
来源：http://zp.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://il.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://uu.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://sv.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://mw.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ov.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ze.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://lq.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://yr.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yc.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yk.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://go.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vo.asd995.cn

[B15] 布尔运算与取反
来源：http://zi.shxzukj.cn

Py:   a and b or not c
来源：http://cf.hahajie.cn

PHP:  $a && $b || !$c
来源：http://ya.szsharing.cn

JS:   a && b || !c
来源：http://oz.yuexingan06.cn

TS:   a && b || !c
来源：http://fd.yuntaijiaju.cn

Java: a && b || !c
来源：http://sv.szsharing.cn

Go:   a && b || !c
来源：http://fl.colortex.cn

Ruby: a && b || !c
来源：http://hg.shxzukj.cn

C#:   a && b || !c
来源：http://cr.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nz.jctech888.com.cn

Py:   if not data: return
来源：http://bo.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://pb.szxytkj.cn

JS:   if (!data) return;
来源：http://wx.nszjky.cn

TS:   if (!data) return;
来源：http://xn.nicolike.cn

Java: if (data == null) return;
来源：http://gw.haigaiapp.cn

Go:   if data == nil { return }
来源：http://sn.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://la.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://ex.asd995.cn

================================================================================
来源：http://ke.nicolike.cn

C. 函数与作用域
来源：http://ak.wgjwhj.cn

================================================================================
来源：http://up.9csxet.cn

[C01] 定义函数
来源：http://dp.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://cg.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fc.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://ml.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ql.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qu.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nq.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://kp.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sk.521024.cn

[C02] 默认参数
来源：http://ex.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://in.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tc.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://xs.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ik.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kh.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kb.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://pz.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://zi.haigaiapp.cn

[C03] 可变参数
来源：http://lz.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://gq.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yy.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lg.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://si.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://go.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gb.wgjwhj.cn


<!-- 参考信息 -->