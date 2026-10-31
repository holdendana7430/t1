代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://ad.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qk.521024.cn

[A12] 字符串插值 / 格式化
来源：http://db.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zg.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xh.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://le.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://tw.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://tf.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nj.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://bn.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://cg.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oe.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://po.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://om.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://yn.asd995.cn

TS:   "第一行\n第二行"
来源：http://pk.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://mu.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://jh.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://hz.asd995.cn

C#:   "第一行\n第二行"
来源：http://ly.colortex.cn

[A14] 注释写法
来源：http://ca.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wj.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yx.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://vj.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://fr.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qm.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://mb.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://go.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://tm.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://op.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://ip.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://pr.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://hj.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://va.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xe.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://hy.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://mc.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://vj.gzmigu.cn

[A16] 真假值判断规则
来源：http://hh.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mf.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ip.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bi.gzmigu.cn

TS:   if (!x) {}
来源：http://ae.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kw.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://em.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cw.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bc.chemitech.net.cn

[A17] 位运算
来源：http://hh.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bh.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sm.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zz.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vi.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nk.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cb.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dc.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nm.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://hi.asd995.cn

Py:   ord("A"); chr(65)
来源：http://yu.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://rk.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hm.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://go.521024.cn

Java: (int) 'A'; (char) 65
来源：http://vh.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pl.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://kp.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://xf.hahajie.cn

[A19] 交换两个变量
来源：http://vp.nszjky.cn

Py:   a, b = b, a
来源：http://ga.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ft.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://cs.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://hd.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://it.bjjhwx.cn

Go:   a, b = b, a
来源：http://qt.asd995.cn

Ruby: a, b = b, a
来源：http://gd.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://ku.haigaiapp.cn

[A20] 读取标准输入
来源：http://dp.szsharing.cn

Py:   name = input("请输入：")
来源：http://da.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cd.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kv.colortex.cn

TS:   // Node.js：readline 模块
来源：http://po.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ob.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jb.nicolike.cn

Ruby: gets.chomp
来源：http://it.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://pe.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://mr.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://yr.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ua.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://qf.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://sq.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://dc.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zb.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://nx.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://mt.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://xd.nszjky.cn

Py:   len(s)
来源：http://ad.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cp.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rz.lnxyls.cn

TS:   s.length
来源：http://dd.bjjhwx.cn

Java: s.length()
来源：http://ln.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ct.newstarts.cn

Ruby: s.length
来源：http://dq.nicolike.cn

C#:   s.Length
来源：http://zo.newstarts.cn

[A23] 大小写转换
来源：http://hy.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://iu.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dv.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ni.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hl.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fc.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aw.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vv.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://om.muxihuayi.cn

[A24] 去除首尾空白
来源：http://ou.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ct.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oe.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://di.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cm.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://va.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://yg.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vr.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uj.lnxyls.cn

[A25] 字符串比较
来源：http://mh.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://bp.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ll.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fy.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ta.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fg.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lj.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qn.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dd.nicolike.cn

[A26] 类型转换总览
来源：http://qu.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zg.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yw.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://db.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://fa.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://db.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zc.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hi.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pt.huixinmuqiang.cn

================================================================================
来源：http://fp.colortex.cn

B. 流程控制
来源：http://fb.jctech888.com.cn

================================================================================
来源：http://cs.newstarts.cn

[B01] 条件判断 if / else
来源：http://te.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://se.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gl.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yi.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ru.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://me.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cw.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xm.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://al.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://nm.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yp.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sv.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sj.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ky.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mo.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pb.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pe.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ot.panjiajie.cn

[B03] switch / match / case
来源：http://uf.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sw.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xc.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nu.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gu.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ft.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yq.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fj.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pi.huanxung.cn

[B04] for 计数循环
来源：http://gn.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://zh.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lt.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rw.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ha.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bv.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cd.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://tq.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ki.asd995.cn

[B05] 遍历数组 / 列表
来源：http://yi.9csxet.cn

Py:   for item in arr: print(item)
来源：http://nk.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ln.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eb.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pk.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://on.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ev.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://fq.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cr.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://mt.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pl.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zt.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tp.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ig.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cn.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ik.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xj.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ou.shxzukj.cn

[B07] while 循环
来源：http://nc.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://am.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mf.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://cz.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://eq.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://ke.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zm.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://me.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://hc.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://nl.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://az.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mw.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://nm.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://lx.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://fb.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pj.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yi.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://yb.szsharing.cn

[B09] break 与 continue
来源：http://bn.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ai.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hi.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ba.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ni.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tt.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fa.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ln.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fh.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://lj.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wl.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nv.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pz.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://am.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pk.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rw.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tn.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ai.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://nn.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://wg.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://kp.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sl.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bd.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oc.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ev.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://vh.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ld.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://on.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hy.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tg.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dg.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kk.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ky.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fl.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ch.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bu.newstarts.cn

[B13] 判断是否为数字
来源：http://wg.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://mb.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://no.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ey.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dr.jianghongdianzi.cn

Java: x instanceof Number
来源：http://em.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qv.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://ks.nicolike.cn

C#:   x is int or double or decimal
来源：http://om.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://lh.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ww.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zt.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://qt.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://se.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jv.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wg.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mr.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ne.colortex.cn

[B15] 布尔运算与取反
来源：http://te.nszjky.cn

Py:   a and b or not c
来源：http://zs.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://xd.jctech888.com.cn

JS:   a && b || !c
来源：http://vi.lnxyls.cn

TS:   a && b || !c
来源：http://jt.yuntaijiaju.cn

Java: a && b || !c
来源：http://mh.haigaiapp.cn

Go:   a && b || !c
来源：http://kz.gzmigu.cn

Ruby: a && b || !c
来源：http://wx.bjjhwx.cn

C#:   a && b || !c
来源：http://jh.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yd.9csxet.cn

Py:   if not data: return
来源：http://de.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://mk.panjiajie.cn

JS:   if (!data) return;
来源：http://lb.newstarts.cn

TS:   if (!data) return;
来源：http://um.shxzskj.cn

Java: if (data == null) return;
来源：http://hb.shxzskj.cn

Go:   if data == nil { return }
来源：http://si.muxihuayi.cn

Ruby: return if data.nil?
来源：http://yk.yuexingan06.cn

C#:   if (data == null) return;
来源：http://rx.bookmarksfly.cn

================================================================================
来源：http://hp.jctech888.com.cn

C. 函数与作用域
来源：http://gb.bookmarksfly.cn

================================================================================
来源：http://yc.521024.cn

[C01] 定义函数
来源：http://kt.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://gf.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vl.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://pa.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rs.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zs.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mi.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://wp.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yf.jianghongdianzi.cn

[C02] 默认参数
来源：http://ct.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://fs.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xd.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://md.9csxet.cn


<!-- 参考信息 -->