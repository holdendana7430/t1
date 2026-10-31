代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://of.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://ww.colortex.cn

C#:   $"Hello, {name}!"
来源：http://mt.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yl.9csxet.cn

Py:   "第一行\n第二行"
来源：http://cr.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://ng.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://to.newstarts.cn

TS:   "第一行\n第二行"
来源：http://st.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://vx.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://hs.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://wh.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://wi.szxytkj.cn

[A14] 注释写法
来源：http://ox.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mn.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yf.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://ag.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://zz.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nc.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://lt.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yn.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://am.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://uq.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://li.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://tp.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://ay.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://no.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bk.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://bx.hahajie.cn

Ruby: value = data || "默认值"
来源：http://aa.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://ce.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://xy.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jk.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qi.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fg.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://kn.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nt.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zu.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vv.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hm.nszjky.cn

[A17] 位运算
来源：http://qi.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fs.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hm.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fp.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sy.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vu.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://si.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ol.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wu.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://gj.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://mc.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://ly.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wx.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mc.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://gx.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vh.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://xi.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://dp.nszjky.cn

[A19] 交换两个变量
来源：http://ra.newstarts.cn

Py:   a, b = b, a
来源：http://rg.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pj.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://jj.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://ms.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://ug.gzmigu.cn

Go:   a, b = b, a
来源：http://sx.521024.cn

Ruby: a, b = b, a
来源：http://kb.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://wt.shxzukj.cn

[A20] 读取标准输入
来源：http://qq.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://ea.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uz.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uc.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://qa.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://cv.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cv.panjiajie.cn

Ruby: gets.chomp
来源：http://mh.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://st.colortex.cn

[A21] 保留指定小数位输出
来源：http://ez.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://dr.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nv.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://pe.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://kq.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://jk.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gv.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://hb.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://fa.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://fy.jianghongdianzi.cn

Py:   len(s)
来源：http://ii.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ig.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lv.newstarts.cn

TS:   s.length
来源：http://ef.panjiajie.cn

Java: s.length()
来源：http://nt.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://me.yuexingan06.cn

Ruby: s.length
来源：http://kv.nicolike.cn

C#:   s.Length
来源：http://ln.haigaiapp.cn

[A23] 大小写转换
来源：http://dm.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ic.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aj.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cz.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bw.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oa.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://di.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zh.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ut.gzmigu.cn

[A24] 去除首尾空白
来源：http://vm.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mz.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xe.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ll.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ql.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ra.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://mc.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kp.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://br.asd995.cn

[A25] 字符串比较
来源：http://zo.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://wv.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tg.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://id.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ol.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hl.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pk.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dd.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sl.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://xp.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://id.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wg.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ms.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://fz.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yj.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rc.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kg.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lb.521024.cn

================================================================================
来源：http://dy.jctech888.com.cn

B. 流程控制
来源：http://ur.newstarts.cn

================================================================================
来源：http://dd.szxytkj.cn

[B01] 条件判断 if / else
来源：http://kh.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vy.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nx.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qd.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zu.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zo.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://op.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nq.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oa.521024.cn

[B02] 多分支 else if / elif
来源：http://et.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yg.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oj.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gs.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dy.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://op.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ly.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uo.nicolike.cn

[B03] switch / match / case
来源：http://an.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iu.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tx.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jp.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iv.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wg.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xi.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zy.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kv.chemitech.net.cn

[B04] for 计数循环
来源：http://qn.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://vm.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dt.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qn.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zn.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://de.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ha.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://uo.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bz.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://kr.colortex.cn

Py:   for item in arr: print(item)
来源：http://mf.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://us.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bw.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ul.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kt.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jz.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://ng.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zo.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://ec.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pe.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://co.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ys.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rt.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hh.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vv.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vb.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zv.huixiangedu.cn

[B07] while 循环
来源：http://wa.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://bh.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fp.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://nw.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://gd.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://ca.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bc.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://ve.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://bb.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://nj.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://gu.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vr.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://xk.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://xm.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://he.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zj.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kh.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://lu.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ii.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://io.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://em.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mb.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://we.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zq.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ho.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oc.521024.cn

[B10] 遍历同时拿索引
来源：http://ub.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://af.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zy.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vb.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ee.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xt.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://px.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://la.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://td.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://df.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://ot.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://gm.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bi.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://js.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ka.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qy.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://qv.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rk.shxzukj.cn

[B12] 跳出多层循环
来源：http://ea.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bx.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qo.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://im.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vw.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bp.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kq.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qt.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fh.hnjuh.cn

[B13] 判断是否为数字
来源：http://st.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://su.panjiajie.cn

PHP:  is_numeric($x)
来源：http://xn.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uq.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fj.muxihuayi.cn

Java: x instanceof Number
来源：http://bm.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fq.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://kw.shxzukj.cn

C#:   x is int or double or decimal
来源：http://ux.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://wq.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lo.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yg.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://mm.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://db.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pj.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jd.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://av.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ks.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://rx.9csxet.cn

Py:   a and b or not c
来源：http://tq.9csxet.cn

PHP:  $a && $b || !$c
来源：http://jp.yuntaijiaju.cn

JS:   a && b || !c
来源：http://sr.bjjhwx.cn

TS:   a && b || !c
来源：http://mf.huanxung.cn

Java: a && b || !c
来源：http://sh.asd995.cn

Go:   a && b || !c
来源：http://jw.szxytkj.cn

Ruby: a && b || !c
来源：http://hs.shxzukj.cn

C#:   a && b || !c
来源：http://jv.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ao.jctech888.com.cn

Py:   if not data: return
来源：http://ew.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://cj.nicolike.cn

JS:   if (!data) return;
来源：http://jr.chemitech.net.cn

TS:   if (!data) return;
来源：http://gg.wgjwhj.cn

Java: if (data == null) return;
来源：http://mf.huanxung.cn

Go:   if data == nil { return }
来源：http://hi.shtwfgs.cn

Ruby: return if data.nil?
来源：http://sk.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://qw.hahajie.cn

================================================================================
来源：http://hd.szsharing.cn

C. 函数与作用域
来源：http://lj.haigaiapp.cn

================================================================================
来源：http://vb.shxzskj.cn

[C01] 定义函数
来源：http://hg.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://ja.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tg.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://hk.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dc.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ju.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fr.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://lm.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yx.chemitech.net.cn

[C02] 默认参数
来源：http://ts.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://zj.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lh.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://gy.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nq.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pf.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://je.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://en.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://xg.gzmigu.cn

[C03] 可变参数
来源：http://zf.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://dz.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://su.huixinmuqiang.cn


<!-- 参考信息 -->