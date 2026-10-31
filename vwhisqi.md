代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://wk.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ps.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://ry.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mg.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ba.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ji.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://xi.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qb.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bd.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://da.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://hz.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://eh.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lz.521024.cn

Ruby: "Hello, #{name}!"
来源：http://qn.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://fs.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rb.hahajie.cn

Py:   "第一行\n第二行"
来源：http://vx.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://ji.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://vh.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://of.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://cj.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://ui.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://nj.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://ng.yuexingan06.cn

[A14] 注释写法
来源：http://gh.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qm.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ux.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://da.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://ec.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wm.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://nf.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uv.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://mx.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://jy.szsharing.cn

Py:   value = data or "默认值"
来源：http://mg.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://kw.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://wx.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://di.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wz.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://wj.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://xe.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://va.gzmigu.cn

[A16] 真假值判断规则
来源：http://of.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rd.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aj.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bw.hnjuh.cn

TS:   if (!x) {}
来源：http://xw.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iw.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yp.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zb.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fl.nicolike.cn

[A17] 位运算
来源：http://ke.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qv.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qz.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xt.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qu.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ke.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lh.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ds.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vn.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://zx.colortex.cn

Py:   ord("A"); chr(65)
来源：http://xv.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://ct.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rw.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fp.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://dk.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ov.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://xg.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://xl.bjjhwx.cn

[A19] 交换两个变量
来源：http://ha.wgjwhj.cn

Py:   a, b = b, a
来源：http://on.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fy.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://ym.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://pk.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://db.521024.cn

Go:   a, b = b, a
来源：http://kc.haigaiapp.cn

Ruby: a, b = b, a
来源：http://by.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://jb.9csxet.cn

[A20] 读取标准输入
来源：http://lb.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://ye.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oz.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xm.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://pr.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://ph.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ji.gzmigu.cn

Ruby: gets.chomp
来源：http://ow.nszjky.cn

C#:   Console.ReadLine();
来源：http://if.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://tk.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://yg.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zg.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://ny.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://tw.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://af.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://re.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://bn.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://cs.shxzskj.cn

[A22] 获取字符串长度
来源：http://wp.yuexingan06.cn

Py:   len(s)
来源：http://gn.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uj.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ge.521024.cn

TS:   s.length
来源：http://bn.muxihuayi.cn

Java: s.length()
来源：http://it.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zn.huixinmuqiang.cn

Ruby: s.length
来源：http://ny.szxytkj.cn

C#:   s.Length
来源：http://sk.nszjky.cn

[A23] 大小写转换
来源：http://jh.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mx.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tx.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gl.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tt.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dz.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uu.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jx.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qp.bjjhwx.cn

[A24] 去除首尾空白
来源：http://gw.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ia.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hh.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ob.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lg.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xd.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://jg.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qu.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pq.haigaiapp.cn

[A25] 字符串比较
来源：http://im.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://pm.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bs.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fd.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bk.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yt.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nt.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gr.yuexingan06.cn

[A26] 类型转换总览
来源：http://fw.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ku.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rk.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yb.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://km.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://db.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mm.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ef.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ub.nszjky.cn

================================================================================
来源：http://jy.jctech888.com.cn

B. 流程控制
来源：http://ux.huanxung.cn

================================================================================
来源：http://cb.szxytkj.cn

[B01] 条件判断 if / else
来源：http://td.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mh.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ag.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://om.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dk.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fr.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fw.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fz.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vi.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://ml.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sc.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aa.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zo.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ci.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qu.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oc.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://np.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zb.shxzskj.cn

[B03] switch / match / case
来源：http://wm.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ps.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ga.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cq.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tn.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zq.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://md.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jr.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ux.chemitech.net.cn

[B04] for 计数循环
来源：http://yi.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://rv.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wy.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mu.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pa.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tr.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ga.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://mt.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zw.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://uk.521024.cn

Py:   for item in arr: print(item)
来源：http://bk.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://id.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dn.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nq.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rd.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cb.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://er.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sv.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://dv.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xv.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jo.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nu.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zn.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ij.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://le.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nq.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cc.521024.cn

[B07] while 循环
来源：http://hl.huanxung.cn

Py:   while i < 10: i += 1
来源：http://yg.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xn.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://yy.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://ld.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://oi.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zc.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://md.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://kl.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://qk.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://tp.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://px.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://ej.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://ja.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://je.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bn.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pc.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://nf.bjjhwx.cn

[B09] break 与 continue
来源：http://wr.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hc.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jm.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://je.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wp.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jc.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fb.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tl.hahajie.cn

[B10] 遍历同时拿索引
来源：http://yj.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gn.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yy.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dp.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hm.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ea.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wx.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ro.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ki.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://vp.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://aw.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://yx.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ur.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bm.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://by.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tq.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://ug.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ki.muxihuayi.cn

[B12] 跳出多层循环
来源：http://fy.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vl.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ho.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gx.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wi.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ar.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pk.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xb.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vl.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://fh.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://yg.nszjky.cn

PHP:  is_numeric($x)
来源：http://kn.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ft.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pi.shxzukj.cn

Java: x instanceof Number
来源：http://xs.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iz.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://me.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://hk.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://id.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uh.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kf.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ae.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://is.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xd.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tr.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jy.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://la.gzmigu.cn

[B15] 布尔运算与取反
来源：http://ce.panjiajie.cn

Py:   a and b or not c
来源：http://gf.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://fs.huanxung.cn

JS:   a && b || !c
来源：http://kx.yuntaijiaju.cn

TS:   a && b || !c
来源：http://db.wgjwhj.cn

Java: a && b || !c
来源：http://ep.hnjuh.cn

Go:   a && b || !c
来源：http://it.shxzukj.cn

Ruby: a && b || !c
来源：http://oh.chemitech.net.cn

C#:   a && b || !c
来源：http://xa.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fm.newstarts.cn

Py:   if not data: return
来源：http://xv.asd995.cn

PHP:  if (!$data) { return; }
来源：http://iw.hahajie.cn

JS:   if (!data) return;
来源：http://ls.nszjky.cn

TS:   if (!data) return;
来源：http://cn.lnxyls.cn

Java: if (data == null) return;
来源：http://du.shtwfgs.cn

Go:   if data == nil { return }
来源：http://lp.nszjky.cn

Ruby: return if data.nil?
来源：http://fy.9csxet.cn

C#:   if (data == null) return;
来源：http://xc.huixinmuqiang.cn

================================================================================
来源：http://ji.szxytkj.cn

C. 函数与作用域
来源：http://wb.chemitech.net.cn

================================================================================
来源：http://gp.chemitech.net.cn

[C01] 定义函数
来源：http://ek.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://ey.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eh.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://jd.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ig.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yt.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://by.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://tu.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ni.lnxyls.cn


<!-- 参考信息 -->