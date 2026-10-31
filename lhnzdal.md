代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ev.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://hv.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://nm.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mh.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://zp.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://pk.521024.cn

JS:   "第一行\n第二行"
来源：http://px.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://sd.hahajie.cn

Java: "第一行\n第二行"
来源：http://cn.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://he.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://ke.colortex.cn

C#:   "第一行\n第二行"
来源：http://hl.szxytkj.cn

[A14] 注释写法
来源：http://fs.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ni.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qs.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://qs.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://ak.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wi.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://mj.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fm.521024.cn

C#:   // 单行；/* 多行 */
来源：http://km.colortex.cn

[A15] 空值判断与默认值
来源：http://vj.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://vh.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://oe.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://sc.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://qw.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rf.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://co.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://jk.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://ju.shtwfgs.cn

[A16] 真假值判断规则
来源：http://qh.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ny.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kb.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ju.nicolike.cn

TS:   if (!x) {}
来源：http://ot.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qi.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ha.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rh.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ii.huixiangedu.cn

[A17] 位运算
来源：http://qa.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ff.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jg.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lo.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qi.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hm.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ks.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vd.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pf.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://dt.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://oe.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://be.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pj.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ta.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://md.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://at.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://qx.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://pf.bjjhwx.cn

[A19] 交换两个变量
来源：http://se.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://bs.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ro.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://mt.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://za.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://qe.jctech888.com.cn

Go:   a, b = b, a
来源：http://vm.nicolike.cn

Ruby: a, b = b, a
来源：http://tp.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://fi.szxytkj.cn

[A20] 读取标准输入
来源：http://zw.shxzukj.cn

Py:   name = input("请输入：")
来源：http://zc.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rw.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fd.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://nd.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://ul.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sm.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://lj.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://ur.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://jb.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://lw.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xy.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://re.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://zz.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://zx.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cy.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://dk.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://hh.panjiajie.cn

[A22] 获取字符串长度
来源：http://fg.nicolike.cn

Py:   len(s)
来源：http://lc.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gk.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ur.jianghongdianzi.cn

TS:   s.length
来源：http://sp.shxzukj.cn

Java: s.length()
来源：http://ua.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ke.huixinmuqiang.cn

Ruby: s.length
来源：http://kg.bjjhwx.cn

C#:   s.Length
来源：http://ai.huanxung.cn

[A23] 大小写转换
来源：http://hz.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mc.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ja.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pw.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wp.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cj.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dj.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rb.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ee.shxzskj.cn

[A24] 去除首尾空白
来源：http://qf.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vf.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ug.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lp.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ud.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bf.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://ge.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://td.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vj.haigaiapp.cn

[A25] 字符串比较
来源：http://sm.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://mw.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jb.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hn.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mq.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ll.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hl.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://em.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ua.huixiangedu.cn

[A26] 类型转换总览
来源：http://au.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hk.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eo.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://va.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://to.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pu.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nu.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yi.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jt.lnxyls.cn

================================================================================
来源：http://ky.bookmarksfly.cn

B. 流程控制
来源：http://fa.szsharing.cn

================================================================================
来源：http://hy.hahajie.cn

[B01] 条件判断 if / else
来源：http://zc.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pu.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ft.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bx.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ig.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zo.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://db.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lc.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eu.9csxet.cn

[B02] 多分支 else if / elif
来源：http://zx.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bc.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xr.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sf.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qp.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vq.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dl.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gv.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mm.panjiajie.cn

[B03] switch / match / case
来源：http://yx.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ka.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cv.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ub.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vk.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jq.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pj.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wp.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yb.huixinmuqiang.cn

[B04] for 计数循环
来源：http://ww.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://nz.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fi.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kp.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fz.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ee.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://iv.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xm.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://yk.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://fu.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qq.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oz.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rk.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pl.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gz.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://sn.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rb.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://wy.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zs.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fq.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rg.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zi.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jv.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yu.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hm.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dv.bjjhwx.cn

[B07] while 循环
来源：http://tw.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://rq.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fu.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://sw.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://wc.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://of.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yt.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://gu.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://bd.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://bq.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://wx.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ja.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://ai.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://cy.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://gn.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zz.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cp.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://bo.chemitech.net.cn

[B09] break 与 continue
来源：http://bc.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xu.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sd.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bz.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jv.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zu.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xl.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ca.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ch.colortex.cn

[B10] 遍历同时拿索引
来源：http://mo.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hs.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fk.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dx.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ml.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://it.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rp.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vl.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sv.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://po.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://vk.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://kp.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ok.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ao.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fy.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tc.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://hj.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ds.hahajie.cn

[B12] 跳出多层循环
来源：http://dj.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fx.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://es.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ui.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://af.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dm.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bc.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cg.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ed.gzmigu.cn

[B13] 判断是否为数字
来源：http://rm.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://nb.9csxet.cn

PHP:  is_numeric($x)
来源：http://im.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jq.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ht.9csxet.cn

Java: x instanceof Number
来源：http://bc.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fw.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://ff.shxzukj.cn

C#:   x is int or double or decimal
来源：http://cx.hahajie.cn

[B14] 判断值是否在集合内
来源：http://cq.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ro.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ri.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://lw.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://yw.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://te.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yy.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mp.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pm.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://xs.9csxet.cn

Py:   a and b or not c
来源：http://ar.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://sy.shxzskj.cn

JS:   a && b || !c
来源：http://pm.szxytkj.cn

TS:   a && b || !c
来源：http://gc.huanxung.cn

Java: a && b || !c
来源：http://lx.bjjhwx.cn

Go:   a && b || !c
来源：http://ot.521024.cn

Ruby: a && b || !c
来源：http://rd.haigaiapp.cn

C#:   a && b || !c
来源：http://hf.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ck.haigaiapp.cn

Py:   if not data: return
来源：http://ox.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://cd.nicolike.cn

JS:   if (!data) return;
来源：http://wq.szxytkj.cn

TS:   if (!data) return;
来源：http://hg.shxzukj.cn

Java: if (data == null) return;
来源：http://hy.panjiajie.cn

Go:   if data == nil { return }
来源：http://nf.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://lo.huixiangedu.cn

C#:   if (data == null) return;
来源：http://cw.colortex.cn

================================================================================
来源：http://gy.panjiajie.cn

C. 函数与作用域
来源：http://da.jianghongdianzi.cn

================================================================================
来源：http://or.szxytkj.cn

[C01] 定义函数
来源：http://jc.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://kl.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rt.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://ev.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dc.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qx.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://su.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://vy.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qa.jianghongdianzi.cn

[C02] 默认参数
来源：http://qr.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://nl.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zm.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://hv.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tr.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ft.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vk.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://vp.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://bh.colortex.cn

[C03] 可变参数
来源：http://tk.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://hu.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lc.hahajie.cn


<!-- 参考信息 -->