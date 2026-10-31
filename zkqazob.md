代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://ko.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fg.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://yq.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hk.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://la.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wh.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://ag.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kg.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zg.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://ao.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://su.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://zt.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qq.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://fm.521024.cn

C#:   $"Hello, {name}!"
来源：http://vi.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://py.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://ko.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://sk.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://iz.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://dz.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://xt.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ui.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://gy.asd995.cn

C#:   "第一行\n第二行"
来源：http://ig.szsharing.cn

[A14] 注释写法
来源：http://wm.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hg.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ac.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://ik.521024.cn

TS:   // 单行；/* 多行 */
来源：http://hv.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nc.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://di.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wc.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://ky.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://xb.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://pr.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://oy.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://ys.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://gv.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://le.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://pu.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://vc.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://pw.9csxet.cn

[A16] 真假值判断规则
来源：http://uu.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ij.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qe.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://li.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://vg.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ag.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yf.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sq.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vc.jianghongdianzi.cn

[A17] 位运算
来源：http://rt.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wj.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wa.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fb.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vj.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gi.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lo.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ci.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vs.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://sj.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://xx.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://vy.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tj.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hf.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://qb.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mg.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://yq.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://oj.shxzskj.cn

[A19] 交换两个变量
来源：http://xu.panjiajie.cn

Py:   a, b = b, a
来源：http://on.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qj.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://ws.colortex.cn

TS:   [a, b] = [b, a];
来源：http://vk.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://my.lnxyls.cn

Go:   a, b = b, a
来源：http://iz.newstarts.cn

Ruby: a, b = b, a
来源：http://il.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://lp.asd995.cn

[A20] 读取标准输入
来源：http://gj.shxzukj.cn

Py:   name = input("请输入：")
来源：http://dh.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tv.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yn.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://qq.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://ao.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sp.panjiajie.cn

Ruby: gets.chomp
来源：http://uz.gzmigu.cn

C#:   Console.ReadLine();
来源：http://mw.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://wp.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://cs.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eb.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://qk.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://yl.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://lm.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xn.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://fe.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://ak.hahajie.cn

[A22] 获取字符串长度
来源：http://fy.nicolike.cn

Py:   len(s)
来源：http://la.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rm.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dm.shtwfgs.cn

TS:   s.length
来源：http://fv.lnxyls.cn

Java: s.length()
来源：http://om.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ka.bjjhwx.cn

Ruby: s.length
来源：http://xh.jianghongdianzi.cn

C#:   s.Length
来源：http://mb.shxzskj.cn

[A23] 大小写转换
来源：http://rq.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ox.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nc.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://as.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tn.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dg.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ae.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xs.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sg.bjjhwx.cn

[A24] 去除首尾空白
来源：http://iu.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zk.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qm.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jl.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://db.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mi.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://uh.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dy.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hi.521024.cn

[A25] 字符串比较
来源：http://df.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://gr.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://td.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kq.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ss.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ic.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kx.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://el.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qk.asd995.cn

[A26] 类型转换总览
来源：http://mu.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qi.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gi.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ej.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://ax.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://li.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kw.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lf.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gd.haigaiapp.cn

================================================================================
来源：http://kn.bookmarksfly.cn

B. 流程控制
来源：http://lr.yuntaijiaju.cn

================================================================================
来源：http://ct.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://ch.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ao.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qv.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://he.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oy.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pa.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tl.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qm.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ca.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://kb.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wx.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aq.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gf.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uj.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yx.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://et.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sx.asd995.cn

[B03] switch / match / case
来源：http://tc.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nq.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ej.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jp.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kq.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ia.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gr.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nf.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sa.yuntaijiaju.cn

[B04] for 计数循环
来源：http://dd.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://ke.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dq.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dj.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nd.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cw.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sj.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://ws.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gn.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://ab.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://hg.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pq.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ru.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fz.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zk.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ij.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://ar.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://do.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://cn.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xi.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vn.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://no.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vp.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://st.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yp.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zp.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bs.521024.cn

[B07] while 循环
来源：http://tf.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://cb.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ga.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://uo.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://mg.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://vi.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kl.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://se.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ae.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://ul.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://wh.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dp.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://va.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://iv.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://xv.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gx.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tf.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://ov.colortex.cn

[B09] break 与 continue
来源：http://gt.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://au.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jy.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zf.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://av.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fx.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sv.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ip.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kx.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://po.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vj.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jg.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gx.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pw.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ol.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kt.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ie.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iy.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://az.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://hg.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://la.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qo.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nt.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lx.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ac.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://hf.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dl.nicolike.cn

[B12] 跳出多层循环
来源：http://ri.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ju.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ru.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sd.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://md.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://id.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qa.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gp.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oo.nszjky.cn

[B13] 判断是否为数字
来源：http://sp.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://ha.9csxet.cn

PHP:  is_numeric($x)
来源：http://ey.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://by.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fw.wgjwhj.cn

Java: x instanceof Number
来源：http://co.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uo.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://tu.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://es.newstarts.cn

[B14] 判断值是否在集合内
来源：http://iz.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://we.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bw.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://an.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://zf.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eu.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tj.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gr.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ur.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://uf.lnxyls.cn

Py:   a and b or not c
来源：http://kl.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://ol.panjiajie.cn

JS:   a && b || !c
来源：http://kx.chemitech.net.cn

TS:   a && b || !c
来源：http://if.muxihuayi.cn

Java: a && b || !c
来源：http://ib.521024.cn

Go:   a && b || !c
来源：http://xb.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://py.jianghongdianzi.cn

C#:   a && b || !c
来源：http://bg.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fy.yuexingan06.cn

Py:   if not data: return
来源：http://ir.521024.cn

PHP:  if (!$data) { return; }
来源：http://mh.521024.cn

JS:   if (!data) return;
来源：http://ew.bjjhwx.cn

TS:   if (!data) return;
来源：http://bm.haigaiapp.cn

Java: if (data == null) return;
来源：http://jo.shtwfgs.cn

Go:   if data == nil { return }
来源：http://wh.huixiangedu.cn

Ruby: return if data.nil?
来源：http://nx.yuexingan06.cn

C#:   if (data == null) return;
来源：http://cz.yuexingan06.cn

================================================================================
来源：http://th.shxzskj.cn

C. 函数与作用域
来源：http://rc.9csxet.cn

================================================================================
来源：http://ab.shxzukj.cn

[C01] 定义函数
来源：http://eg.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://fx.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qe.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://zk.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qd.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hn.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cs.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://nb.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ib.yuntaijiaju.cn


<!-- 参考信息 -->