代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hm.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://ld.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://ie.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mu.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://in.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jh.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://gw.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ot.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jd.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zm.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://wh.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rp.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ld.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://po.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://jc.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://nk.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ae.521024.cn

Ruby: "Hello, #{name}!"
来源：http://rd.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://mz.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://do.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://vb.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://rv.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://jl.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://wk.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://am.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://ra.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://fe.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://im.chemitech.net.cn

[A14] 注释写法
来源：http://cj.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://di.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wh.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://ob.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://ny.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hi.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://rp.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ud.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://en.521024.cn

[A15] 空值判断与默认值
来源：http://gx.lnxyls.cn

Py:   value = data or "默认值"
来源：http://no.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://dn.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://bz.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://qw.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hc.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://mc.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://tx.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://ta.wgjwhj.cn

[A16] 真假值判断规则
来源：http://bj.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fw.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ub.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dn.szxytkj.cn

TS:   if (!x) {}
来源：http://lg.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ot.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://am.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ka.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qe.huanxung.cn

[A17] 位运算
来源：http://mu.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tj.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eh.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qg.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zr.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fi.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://us.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vg.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vl.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://mg.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://bv.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://tf.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xo.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gc.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://gm.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aw.521024.cn

Ruby: "A".ord; 65.chr
来源：http://bu.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://mq.shxzskj.cn

[A19] 交换两个变量
来源：http://dj.colortex.cn

Py:   a, b = b, a
来源：http://bk.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://we.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://qy.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://gs.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://yz.shxzskj.cn

Go:   a, b = b, a
来源：http://ix.chemitech.net.cn

Ruby: a, b = b, a
来源：http://qh.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://no.nszjky.cn

[A20] 读取标准输入
来源：http://he.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://jm.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eh.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lx.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://mo.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://oq.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eq.szsharing.cn

Ruby: gets.chomp
来源：http://pl.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://lw.newstarts.cn

[A21] 保留指定小数位输出
来源：http://rm.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://kt.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cj.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://up.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://rb.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://lx.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zv.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://hy.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://ce.newstarts.cn

[A22] 获取字符串长度
来源：http://vu.gzmigu.cn

Py:   len(s)
来源：http://lo.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bi.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aw.yuexingan06.cn

TS:   s.length
来源：http://kw.huixiangedu.cn

Java: s.length()
来源：http://sq.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bg.hnjuh.cn

Ruby: s.length
来源：http://mr.lnxyls.cn

C#:   s.Length
来源：http://qt.wgjwhj.cn

[A23] 大小写转换
来源：http://gn.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uy.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tz.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hc.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://to.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ve.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ss.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hm.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xy.wgjwhj.cn

[A24] 去除首尾空白
来源：http://ry.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vw.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ga.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jd.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nc.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kw.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://or.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bd.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ts.huixinmuqiang.cn

[A25] 字符串比较
来源：http://xl.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://zx.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qp.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zm.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ss.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xq.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ns.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pk.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bl.nszjky.cn

[A26] 类型转换总览
来源：http://ga.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lf.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fh.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nx.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://am.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ln.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ec.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ow.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bt.hahajie.cn

================================================================================
来源：http://gc.wgjwhj.cn

B. 流程控制
来源：http://no.9csxet.cn

================================================================================
来源：http://lf.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://mp.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://us.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tq.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qu.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dk.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xz.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xx.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vf.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://og.asd995.cn

[B02] 多分支 else if / elif
来源：http://jh.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jj.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://el.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rj.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ga.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bu.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tq.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hl.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qh.jianghongdianzi.cn

[B03] switch / match / case
来源：http://iq.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vv.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ur.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://df.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gx.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wm.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pf.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rp.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ua.jianghongdianzi.cn

[B04] for 计数循环
来源：http://vx.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://zc.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bm.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nn.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kz.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xg.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ug.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://wn.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uv.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://du.hahajie.cn

Py:   for item in arr: print(item)
来源：http://hv.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lu.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://up.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dm.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sw.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vv.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://au.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vk.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://bt.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cv.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zg.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ps.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xk.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gc.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kx.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yj.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xx.huixiangedu.cn

[B07] while 循环
来源：http://gx.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://xg.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rw.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://kl.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://nv.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://wd.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ce.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://gf.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://ls.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://nc.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://tc.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://am.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://ai.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://jh.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://il.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wp.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hn.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://lz.huixiangedu.cn

[B09] break 与 continue
来源：http://li.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vv.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nn.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lq.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://og.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hg.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wi.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qs.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ty.521024.cn

[B10] 遍历同时拿索引
来源：http://hd.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dx.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xz.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dt.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qd.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vx.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ni.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bw.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cm.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://qu.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://di.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://ab.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ab.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ut.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ed.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hr.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://ld.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pd.szsharing.cn

[B12] 跳出多层循环
来源：http://rl.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xz.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bd.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://re.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ov.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://do.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kv.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://df.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vh.haigaiapp.cn

[B13] 判断是否为数字
来源：http://xr.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://sd.hnjuh.cn

PHP:  is_numeric($x)
来源：http://zs.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sd.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lg.bookmarksfly.cn

Java: x instanceof Number
来源：http://ga.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xl.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://fz.hahajie.cn

C#:   x is int or double or decimal
来源：http://zz.asd995.cn

[B14] 判断值是否在集合内
来源：http://sw.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vq.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qi.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://hv.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://le.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jz.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wz.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ng.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://td.newstarts.cn

[B15] 布尔运算与取反
来源：http://ow.szxytkj.cn

Py:   a and b or not c
来源：http://jd.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://ys.newstarts.cn

JS:   a && b || !c
来源：http://kg.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ep.huixinmuqiang.cn

Java: a && b || !c
来源：http://au.yuexingan06.cn

Go:   a && b || !c
来源：http://mf.521024.cn

Ruby: a && b || !c
来源：http://aw.yuexingan06.cn

C#:   a && b || !c
来源：http://sj.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cy.asd995.cn

Py:   if not data: return
来源：http://ev.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://da.colortex.cn

JS:   if (!data) return;
来源：http://rk.huanxung.cn

TS:   if (!data) return;
来源：http://lr.yuexingan06.cn

Java: if (data == null) return;
来源：http://gv.panjiajie.cn

Go:   if data == nil { return }
来源：http://bo.yuexingan06.cn

Ruby: return if data.nil?
来源：http://ou.9csxet.cn

C#:   if (data == null) return;
来源：http://ub.haigaiapp.cn

================================================================================
来源：http://yt.lnxyls.cn

C. 函数与作用域
来源：http://xf.nicolike.cn

================================================================================
来源：http://hf.9csxet.cn

[C01] 定义函数
来源：http://an.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://xn.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://us.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://ez.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fh.yuntaijiaju.cn


<!-- 参考信息 -->