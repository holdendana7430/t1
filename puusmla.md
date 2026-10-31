代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ki.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://et.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://hv.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://ix.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lq.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://bj.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://ff.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ib.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://pe.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://pl.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://bi.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://fi.lnxyls.cn

Java: "第一行\n第二行"
来源：http://ni.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://yv.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://qu.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://re.asd995.cn

[A14] 注释写法
来源：http://at.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ca.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://il.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://fs.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://eo.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sq.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://of.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zt.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://ir.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://sq.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://fi.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://nu.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://pp.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://lb.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wi.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://bn.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://xr.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://bt.asd995.cn

[A16] 真假值判断规则
来源：http://jp.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nn.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fk.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nz.muxihuayi.cn

TS:   if (!x) {}
来源：http://ln.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lh.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vb.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zn.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hk.nszjky.cn

[A17] 位运算
来源：http://ub.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xs.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ex.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yw.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oq.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jm.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ct.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cj.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cj.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://aa.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://qe.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://ld.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ia.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pv.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://me.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qs.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://hc.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://lz.huixiangedu.cn

[A19] 交换两个变量
来源：http://ls.521024.cn

Py:   a, b = b, a
来源：http://ui.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fs.colortex.cn

JS:   [a, b] = [b, a];
来源：http://ni.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://em.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://jh.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://kz.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://zb.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://af.huanxung.cn

[A20] 读取标准输入
来源：http://pj.asd995.cn

Py:   name = input("请输入：")
来源：http://nc.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lp.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sx.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://zp.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://yi.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uq.521024.cn

Ruby: gets.chomp
来源：http://fd.lnxyls.cn

C#:   Console.ReadLine();
来源：http://om.nicolike.cn

[A21] 保留指定小数位输出
来源：http://we.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://sf.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vl.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://jc.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://ui.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://qn.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yh.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://fc.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://fs.muxihuayi.cn

[A22] 获取字符串长度
来源：http://xc.colortex.cn

Py:   len(s)
来源：http://sf.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dw.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eh.colortex.cn

TS:   s.length
来源：http://zj.yuexingan06.cn

Java: s.length()
来源：http://lc.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yj.newstarts.cn

Ruby: s.length
来源：http://tf.asd995.cn

C#:   s.Length
来源：http://qv.bjjhwx.cn

[A23] 大小写转换
来源：http://eh.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jb.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ny.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xe.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lc.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://su.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zr.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://em.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ik.lnxyls.cn

[A24] 去除首尾空白
来源：http://tx.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ni.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bw.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ag.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gb.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zu.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://sb.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ll.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fl.yuexingan06.cn

[A25] 字符串比较
来源：http://jf.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://xx.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bx.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://of.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fs.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bz.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zx.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://me.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://la.bookmarksfly.cn

[A26] 类型转换总览
来源：http://qm.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://un.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rl.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ls.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://rn.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ws.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gb.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ym.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qw.asd995.cn

================================================================================
来源：http://oc.gzmigu.cn

B. 流程控制
来源：http://cu.newstarts.cn

================================================================================
来源：http://wc.gzmigu.cn

[B01] 条件判断 if / else
来源：http://jm.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mm.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xe.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nz.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fq.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ks.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ix.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://na.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hy.newstarts.cn

[B02] 多分支 else if / elif
来源：http://zt.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wz.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ld.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bk.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ib.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jp.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kx.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ok.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qs.nicolike.cn

[B03] switch / match / case
来源：http://sa.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qy.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bf.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://po.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xs.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bt.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://at.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gr.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://id.wgjwhj.cn

[B04] for 计数循环
来源：http://yw.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://nx.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eo.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yv.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ps.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ir.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ap.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://pl.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nb.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://ls.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://xm.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://le.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://la.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://am.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eg.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cz.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://ir.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ae.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://sb.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kr.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lp.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ke.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kr.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qb.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yt.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oa.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hb.bookmarksfly.cn

[B07] while 循环
来源：http://qu.nicolike.cn

Py:   while i < 10: i += 1
来源：http://or.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yk.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://uq.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://tw.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://bc.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://by.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://ff.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://zp.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://ap.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://sr.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sm.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://jk.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://jf.521024.cn

Java: do { i++; } while (i < 10);
来源：http://bx.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wk.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ry.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://kg.hahajie.cn

[B09] break 与 continue
来源：http://xh.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fa.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ur.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sk.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zi.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://te.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://if.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dj.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ur.nicolike.cn

[B10] 遍历同时拿索引
来源：http://cc.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qe.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://re.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gb.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iy.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://it.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bv.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vm.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://by.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ig.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://xz.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://im.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cf.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dz.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://py.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ry.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://ci.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nk.nicolike.cn

[B12] 跳出多层循环
来源：http://cr.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ht.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sk.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jp.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kx.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hw.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nq.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vf.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fu.newstarts.cn

[B13] 判断是否为数字
来源：http://wn.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://iw.lnxyls.cn

PHP:  is_numeric($x)
来源：http://xu.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ok.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nr.muxihuayi.cn

Java: x instanceof Number
来源：http://dp.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oo.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://hl.lnxyls.cn

C#:   x is int or double or decimal
来源：http://oj.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://pk.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jn.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aa.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://ag.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://za.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uo.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dt.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rq.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://im.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://fq.nszjky.cn

Py:   a and b or not c
来源：http://ux.szsharing.cn

PHP:  $a && $b || !$c
来源：http://ku.haigaiapp.cn

JS:   a && b || !c
来源：http://yw.muxihuayi.cn

TS:   a && b || !c
来源：http://ij.newstarts.cn

Java: a && b || !c
来源：http://ko.9csxet.cn

Go:   a && b || !c
来源：http://qp.shxzukj.cn

Ruby: a && b || !c
来源：http://wf.huixiangedu.cn

C#:   a && b || !c
来源：http://kk.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xl.huixiangedu.cn

Py:   if not data: return
来源：http://nv.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://my.szsharing.cn

JS:   if (!data) return;
来源：http://yx.hahajie.cn

TS:   if (!data) return;
来源：http://mh.nszjky.cn

Java: if (data == null) return;
来源：http://vk.nszjky.cn

Go:   if data == nil { return }
来源：http://rd.haigaiapp.cn

Ruby: return if data.nil?
来源：http://rv.jctech888.com.cn

C#:   if (data == null) return;
来源：http://it.huixinmuqiang.cn

================================================================================
来源：http://cr.huixinmuqiang.cn

C. 函数与作用域
来源：http://nm.newstarts.cn

================================================================================
来源：http://on.shxzskj.cn

[C01] 定义函数
来源：http://xx.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://ze.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://se.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://en.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xd.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eb.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ei.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://jb.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mq.wgjwhj.cn

[C02] 默认参数
来源：http://zo.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://xz.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ay.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://yu.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hy.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qn.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bz.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://mo.panjiajie.cn


<!-- 参考信息 -->