代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://bk.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://na.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://tm.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tp.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wz.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xt.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://gn.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zu.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yr.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://en.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://tw.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hd.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://td.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://fh.521024.cn

TS:   `Hello, ${name}!`
来源：http://db.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://ta.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ra.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://iv.asd995.cn

C#:   $"Hello, {name}!"
来源：http://vw.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jn.nszjky.cn

Py:   "第一行\n第二行"
来源：http://zr.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://qb.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://vt.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://sf.hnjuh.cn

Java: "第一行\n第二行"
来源：http://gk.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://so.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://yr.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://tp.hahajie.cn

[A14] 注释写法
来源：http://ai.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mb.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ic.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://pw.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://ft.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sa.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://om.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pt.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://gs.shxzskj.cn

[A15] 空值判断与默认值
来源：http://tf.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://qv.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://rm.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://wd.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://nj.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yn.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ci.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://rd.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://wk.haigaiapp.cn

[A16] 真假值判断规则
来源：http://ff.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sf.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rf.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ya.huanxung.cn

TS:   if (!x) {}
来源：http://az.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vo.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iw.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ek.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fq.hnjuh.cn

[A17] 位运算
来源：http://xa.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xw.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mj.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://li.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pt.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ns.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kh.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://je.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nt.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://bk.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://wr.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://ev.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zl.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uf.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://mk.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://my.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://ri.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://sq.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://gd.panjiajie.cn

Py:   a, b = b, a
来源：http://fb.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vv.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://zd.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://yl.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://kq.9csxet.cn

Go:   a, b = b, a
来源：http://xf.huanxung.cn

Ruby: a, b = b, a
来源：http://ec.521024.cn

C#:   (a, b) = (b, a);
来源：http://iw.lnxyls.cn

[A20] 读取标准输入
来源：http://qh.nszjky.cn

Py:   name = input("请输入：")
来源：http://ax.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vq.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yp.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://gi.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://yr.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ry.huanxung.cn

Ruby: gets.chomp
来源：http://dy.asd995.cn

C#:   Console.ReadLine();
来源：http://ig.nicolike.cn

[A21] 保留指定小数位输出
来源：http://ow.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://cj.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ve.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://jl.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://zt.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://ud.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ql.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://fo.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://bd.haigaiapp.cn

[A22] 获取字符串长度
来源：http://oy.szxytkj.cn

Py:   len(s)
来源：http://uy.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gw.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ul.yuntaijiaju.cn

TS:   s.length
来源：http://et.shxzukj.cn

Java: s.length()
来源：http://gz.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jo.shxzskj.cn

Ruby: s.length
来源：http://vr.jianghongdianzi.cn

C#:   s.Length
来源：http://mr.newstarts.cn

[A23] 大小写转换
来源：http://lf.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://om.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aw.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ni.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yz.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gr.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nr.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sx.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ln.haigaiapp.cn

[A24] 去除首尾空白
来源：http://zj.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cf.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sh.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zh.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wv.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wi.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://nz.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mx.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nm.wgjwhj.cn

[A25] 字符串比较
来源：http://mi.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://zo.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iu.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fu.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kf.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zr.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vv.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wn.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wz.9csxet.cn

[A26] 类型转换总览
来源：http://lx.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gr.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://we.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ol.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://qt.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pe.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xc.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nq.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fq.shtwfgs.cn

================================================================================
来源：http://fd.gzmigu.cn

B. 流程控制
来源：http://al.nicolike.cn

================================================================================
来源：http://bt.nszjky.cn

[B01] 条件判断 if / else
来源：http://db.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://as.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mb.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ub.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bp.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://un.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gj.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ap.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bp.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://yz.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wx.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vp.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sz.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fe.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xh.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zi.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://md.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://er.hnjuh.cn

[B03] switch / match / case
来源：http://vv.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fl.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qr.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ka.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xz.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nu.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://du.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oj.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ic.lnxyls.cn

[B04] for 计数循环
来源：http://cs.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://cp.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aj.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oy.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://un.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xx.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://cb.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tq.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://ou.nicolike.cn

Py:   for item in arr: print(item)
来源：http://tj.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ol.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ar.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jn.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zc.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iw.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://gi.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bu.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://fb.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kg.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sj.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tz.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://av.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ms.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ch.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://im.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gg.panjiajie.cn

[B07] while 循环
来源：http://ff.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://nw.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wx.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://tt.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://mv.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://qc.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ap.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ak.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://li.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://uy.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://wb.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wj.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://hw.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://wv.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://zw.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tu.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qs.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://mm.huixinmuqiang.cn

[B09] break 与 continue
来源：http://hk.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ri.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uq.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rq.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://op.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ty.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bj.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fg.nszjky.cn

[B10] 遍历同时拿索引
来源：http://ey.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bg.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fm.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ua.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bj.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jj.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ee.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zp.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cl.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://mx.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://jz.asd995.cn

PHP:  range(0, 10, 2);
来源：http://gn.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tg.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mk.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qi.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nu.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://zv.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ag.yuexingan06.cn

[B12] 跳出多层循环
来源：http://hm.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ie.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tg.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hf.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://up.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://co.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jm.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://un.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wv.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://vb.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://jx.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://jj.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rk.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rh.jianghongdianzi.cn

Java: x instanceof Number
来源：http://pd.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ct.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://bx.lnxyls.cn

C#:   x is int or double or decimal
来源：http://dj.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://kc.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kq.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ez.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://op.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://qi.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://at.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wp.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ib.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://td.521024.cn

[B15] 布尔运算与取反
来源：http://gg.asd995.cn

Py:   a and b or not c
来源：http://uf.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://cr.shtwfgs.cn

JS:   a && b || !c
来源：http://uo.jctech888.com.cn

TS:   a && b || !c
来源：http://yi.bookmarksfly.cn

Java: a && b || !c
来源：http://vj.hahajie.cn

Go:   a && b || !c
来源：http://gx.szxytkj.cn

Ruby: a && b || !c
来源：http://aw.9csxet.cn

C#:   a && b || !c
来源：http://ji.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://je.jianghongdianzi.cn

Py:   if not data: return
来源：http://hb.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://ri.szsharing.cn

JS:   if (!data) return;
来源：http://jf.haigaiapp.cn

TS:   if (!data) return;
来源：http://bq.asd995.cn

Java: if (data == null) return;
来源：http://kk.gzmigu.cn

Go:   if data == nil { return }
来源：http://sn.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://pw.jctech888.com.cn

C#:   if (data == null) return;
来源：http://jo.yuexingan06.cn

================================================================================
来源：http://xu.szxytkj.cn

C. 函数与作用域
来源：http://fv.shxzukj.cn

================================================================================
来源：http://cf.panjiajie.cn

[C01] 定义函数
来源：http://wj.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://tq.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uw.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://wj.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vk.wgjwhj.cn


<!-- 参考信息 -->