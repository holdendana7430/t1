代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yl.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://qk.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://ra.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qk.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://go.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://oj.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://fp.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://ex.gzmigu.cn

Java: "第一行\n第二行"
来源：http://ol.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://ec.colortex.cn

Ruby: "第一行\n第二行"
来源：http://ub.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://ow.shxzskj.cn

[A14] 注释写法
来源：http://lf.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xa.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ze.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://pj.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://yc.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oi.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://ax.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xy.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://tc.lnxyls.cn

[A15] 空值判断与默认值
来源：http://xv.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://gz.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://au.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://xa.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://qj.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xp.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://aq.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://tc.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://ig.shtwfgs.cn

[A16] 真假值判断规则
来源：http://uq.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ir.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://re.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://an.huanxung.cn

TS:   if (!x) {}
来源：http://qp.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rj.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pn.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gq.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://up.lnxyls.cn

[A17] 位运算
来源：http://kg.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hb.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lt.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fy.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ts.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://so.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vm.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ma.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://cx.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://yu.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://kc.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pb.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xu.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://be.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://um.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://ah.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://ti.huanxung.cn

[A19] 交换两个变量
来源：http://qt.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://wh.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://id.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://tb.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://cf.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://dy.asd995.cn

Go:   a, b = b, a
来源：http://qy.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://fh.colortex.cn

C#:   (a, b) = (b, a);
来源：http://ml.muxihuayi.cn

[A20] 读取标准输入
来源：http://hu.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://bz.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zz.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cr.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://pr.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://hk.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hk.shxzukj.cn

Ruby: gets.chomp
来源：http://gr.newstarts.cn

C#:   Console.ReadLine();
来源：http://py.nszjky.cn

[A21] 保留指定小数位输出
来源：http://kw.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://ku.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wj.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://no.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://op.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://wo.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xx.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://hz.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://re.9csxet.cn

[A22] 获取字符串长度
来源：http://bd.lnxyls.cn

Py:   len(s)
来源：http://bt.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nj.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zz.huixinmuqiang.cn

TS:   s.length
来源：http://dm.asd995.cn

Java: s.length()
来源：http://rw.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qx.szxytkj.cn

Ruby: s.length
来源：http://ky.bookmarksfly.cn

C#:   s.Length
来源：http://zf.szsharing.cn

[A23] 大小写转换
来源：http://ju.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://el.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sc.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zw.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xs.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ru.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lz.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xi.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mz.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://tj.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gf.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xu.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pm.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://av.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://go.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://qa.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qv.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qi.huanxung.cn

[A25] 字符串比较
来源：http://dp.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://zc.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wj.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lx.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dw.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ev.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pu.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yt.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eq.wgjwhj.cn

[A26] 类型转换总览
来源：http://bv.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ea.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://re.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fi.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://tx.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ui.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eq.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hq.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mn.asd995.cn

================================================================================
来源：http://hi.jianghongdianzi.cn

B. 流程控制
来源：http://zh.hahajie.cn

================================================================================
来源：http://eg.521024.cn

[B01] 条件判断 if / else
来源：http://yh.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cn.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uj.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qj.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bj.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://to.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://di.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uy.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ie.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://vz.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://up.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oa.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wa.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ii.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fn.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ca.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lp.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oy.colortex.cn

[B03] switch / match / case
来源：http://rb.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hu.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ws.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ob.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bz.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rl.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wn.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ye.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qr.yuntaijiaju.cn

[B04] for 计数循环
来源：http://rw.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://vb.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cn.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cs.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ky.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pj.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uq.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://fo.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cf.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://vv.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://dd.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jl.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rt.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lv.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yt.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ue.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://pw.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://om.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://lh.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xj.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jq.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ec.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ih.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ni.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xn.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kp.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xm.shxzskj.cn

[B07] while 循环
来源：http://tj.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://bn.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oz.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://oh.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://kk.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://je.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://au.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://ze.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://si.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://jq.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://rg.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cd.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://ys.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://ll.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://fx.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xq.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rj.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://qt.szxytkj.cn

[B09] break 与 continue
来源：http://kx.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xa.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ri.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ft.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mb.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xh.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://km.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kd.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cp.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://qh.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jw.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wl.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ko.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sa.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ce.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://px.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zn.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yu.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://oi.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://rb.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://md.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nk.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dq.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tv.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jz.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://mb.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jg.asd995.cn

[B12] 跳出多层循环
来源：http://yq.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lg.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ue.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hw.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://na.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cd.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mk.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xz.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gy.huanxung.cn

[B13] 判断是否为数字
来源：http://nl.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://ub.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://vb.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gn.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lc.szxytkj.cn

Java: x instanceof Number
来源：http://yc.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nf.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://kw.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://hh.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://wu.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iu.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ta.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://uc.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://qn.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zo.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://go.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kh.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jf.nszjky.cn

[B15] 布尔运算与取反
来源：http://rs.hnjuh.cn

Py:   a and b or not c
来源：http://ym.newstarts.cn

PHP:  $a && $b || !$c
来源：http://km.jctech888.com.cn

JS:   a && b || !c
来源：http://wr.muxihuayi.cn

TS:   a && b || !c
来源：http://zm.yuexingan06.cn

Java: a && b || !c
来源：http://dr.shtwfgs.cn

Go:   a && b || !c
来源：http://ik.bookmarksfly.cn

Ruby: a && b || !c
来源：http://ea.wgjwhj.cn

C#:   a && b || !c
来源：http://pu.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hg.bjjhwx.cn

Py:   if not data: return
来源：http://az.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://nz.panjiajie.cn

JS:   if (!data) return;
来源：http://hv.nszjky.cn

TS:   if (!data) return;
来源：http://ir.gzmigu.cn

Java: if (data == null) return;
来源：http://tf.shtwfgs.cn

Go:   if data == nil { return }
来源：http://hc.yuexingan06.cn

Ruby: return if data.nil?
来源：http://oy.521024.cn

C#:   if (data == null) return;
来源：http://mg.yuexingan06.cn

================================================================================
来源：http://nd.asd995.cn

C. 函数与作用域
来源：http://wa.newstarts.cn

================================================================================
来源：http://ym.muxihuayi.cn

[C01] 定义函数
来源：http://xp.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://pj.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pr.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://od.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xf.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sj.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yd.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://xx.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wb.gzmigu.cn

[C02] 默认参数
来源：http://hw.asd995.cn

Py:   def greet(name="World"): return name
来源：http://sl.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nw.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://zr.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zj.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kz.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vg.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://bj.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://en.szsharing.cn

[C03] 可变参数
来源：http://ti.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://ic.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sx.9csxet.cn


<!-- 参考信息 -->