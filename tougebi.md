代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vf.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://vf.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tn.haigaiapp.cn

Ruby: rand(1..100)
来源：http://re.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://vn.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://pw.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://dm.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://in.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vm.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vo.yuntaijiaju.cn

Java: x > 0 ? "yes" : "no"
来源：http://np.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zx.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jd.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cy.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://sj.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://of.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iz.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://yc.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://fh.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://li.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ai.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://fu.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://jq.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gy.nszjky.cn

Py:   "第一行\n第二行"
来源：http://zw.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://af.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://np.nszjky.cn

TS:   "第一行\n第二行"
来源：http://xz.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://nl.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://ui.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://wt.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://if.asd995.cn

[A14] 注释写法
来源：http://tv.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sf.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lu.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://bw.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://xd.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bq.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://wb.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gq.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://yi.newstarts.cn

[A15] 空值判断与默认值
来源：http://ae.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://fc.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://in.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://yr.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://jn.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ck.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://cs.9csxet.cn

Ruby: value = data || "默认值"
来源：http://us.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ft.gzmigu.cn

[A16] 真假值判断规则
来源：http://vv.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fd.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kp.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://so.bookmarksfly.cn

TS:   if (!x) {}
来源：http://pc.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://go.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hl.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ba.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vn.hnjuh.cn

[A17] 位运算
来源：http://vu.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://om.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xn.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uj.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://es.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mx.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vd.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ss.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qn.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://ih.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://bj.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://ax.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://if.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wd.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://mo.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nq.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://gr.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://ai.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://ul.jctech888.com.cn

Py:   a, b = b, a
来源：http://mp.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zv.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://mm.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://or.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://cb.huanxung.cn

Go:   a, b = b, a
来源：http://yl.szxytkj.cn

Ruby: a, b = b, a
来源：http://jt.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://pz.bjjhwx.cn

[A20] 读取标准输入
来源：http://mt.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://ms.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://um.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jk.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://vm.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://tx.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fn.nicolike.cn

Ruby: gets.chomp
来源：http://ot.hahajie.cn

C#:   Console.ReadLine();
来源：http://dn.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://pn.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://pw.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ap.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://lg.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://tl.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://rh.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uw.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://el.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://sw.bjjhwx.cn

[A22] 获取字符串长度
来源：http://yp.jianghongdianzi.cn

Py:   len(s)
来源：http://ft.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ez.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lz.hahajie.cn

TS:   s.length
来源：http://fm.newstarts.cn

Java: s.length()
来源：http://my.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iu.gzmigu.cn

Ruby: s.length
来源：http://py.haigaiapp.cn

C#:   s.Length
来源：http://he.chemitech.net.cn

[A23] 大小写转换
来源：http://qt.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qu.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rf.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tr.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gn.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gj.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iy.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vp.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zd.nszjky.cn

[A24] 去除首尾空白
来源：http://gc.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cv.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://be.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vl.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ma.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fy.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://bv.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cs.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fg.haigaiapp.cn

[A25] 字符串比较
来源：http://cr.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://md.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ry.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cp.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xf.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yh.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pf.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zs.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yf.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://uy.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ln.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yo.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oh.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://uh.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fs.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hf.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rv.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qx.huanxung.cn

================================================================================
来源：http://lr.bookmarksfly.cn

B. 流程控制
来源：http://ul.gzmigu.cn

================================================================================
来源：http://ou.shxzukj.cn

[B01] 条件判断 if / else
来源：http://zb.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ru.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ac.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zc.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jf.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ok.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uk.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lf.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sz.colortex.cn

[B02] 多分支 else if / elif
来源：http://ss.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kk.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://io.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mu.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ra.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jl.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gh.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lk.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jj.nicolike.cn

[B03] switch / match / case
来源：http://ib.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gm.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yv.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sx.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kb.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://la.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dg.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ma.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lo.9csxet.cn

[B04] for 计数循环
来源：http://vt.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://yg.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bp.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ty.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qk.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mm.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ip.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://mz.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ng.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://gr.9csxet.cn

Py:   for item in arr: print(item)
来源：http://vu.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nq.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://if.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rp.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lv.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gs.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://ud.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qa.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://ac.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yv.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iw.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nf.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uf.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iq.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qn.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wp.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ef.hnjuh.cn

[B07] while 循环
来源：http://ys.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://mv.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://om.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://dc.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://xt.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://cw.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kz.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://zn.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://ha.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://pw.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://jh.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://af.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://yt.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://tp.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://fb.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rz.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dx.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://rs.shxzukj.cn

[B09] break 与 continue
来源：http://ax.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ut.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nc.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xp.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vg.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://im.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lf.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ka.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mx.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://hm.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bg.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tm.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bp.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oj.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cc.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yd.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xf.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bj.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://re.521024.cn

Py:   list(range(0, 10, 2))
来源：http://eg.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://fj.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ai.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ln.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ni.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uq.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://ij.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wc.szxytkj.cn

[B12] 跳出多层循环
来源：http://qx.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qq.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uq.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gg.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://br.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fj.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pc.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nb.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mc.shxzukj.cn

[B13] 判断是否为数字
来源：http://up.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://xz.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://dh.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://us.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xg.newstarts.cn

Java: x instanceof Number
来源：http://jt.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dz.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://vz.9csxet.cn

C#:   x is int or double or decimal
来源：http://ml.huanxung.cn

[B14] 判断值是否在集合内
来源：http://bs.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ws.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wb.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://yg.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://fv.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ya.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lq.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://km.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fd.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://ie.yuexingan06.cn

Py:   a and b or not c
来源：http://pb.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://yy.yuntaijiaju.cn

JS:   a && b || !c
来源：http://go.jianghongdianzi.cn

TS:   a && b || !c
来源：http://pz.shxzskj.cn

Java: a && b || !c
来源：http://da.bookmarksfly.cn

Go:   a && b || !c
来源：http://tx.wgjwhj.cn

Ruby: a && b || !c
来源：http://vo.bjjhwx.cn

C#:   a && b || !c
来源：http://zm.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://db.asd995.cn

Py:   if not data: return
来源：http://my.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://id.newstarts.cn

JS:   if (!data) return;
来源：http://hg.9csxet.cn

TS:   if (!data) return;
来源：http://we.muxihuayi.cn

Java: if (data == null) return;
来源：http://mv.szsharing.cn

Go:   if data == nil { return }
来源：http://rl.szxytkj.cn

Ruby: return if data.nil?
来源：http://ve.wgjwhj.cn

C#:   if (data == null) return;
来源：http://wo.521024.cn

================================================================================
来源：http://hw.asd995.cn

C. 函数与作用域
来源：http://yp.521024.cn

================================================================================
来源：http://xt.bjjhwx.cn

[C01] 定义函数
来源：http://uf.shxzukj.cn


<!-- 参考信息 -->