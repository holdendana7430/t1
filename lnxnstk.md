代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://ou.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://st.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://lf.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bq.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ye.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kf.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://lf.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vh.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vz.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://px.asd995.cn

TS:   `Hello, ${name}!`
来源：http://ra.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://uw.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fe.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://tl.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://re.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oo.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://ct.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://gs.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://ne.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://qt.szsharing.cn

Java: "第一行\n第二行"
来源：http://th.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://ag.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://ed.colortex.cn

C#:   "第一行\n第二行"
来源：http://ad.521024.cn

[A14] 注释写法
来源：http://mw.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kr.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zh.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://fh.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://yz.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qh.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://js.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ud.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://qy.shxzskj.cn

[A15] 空值判断与默认值
来源：http://ke.9csxet.cn

Py:   value = data or "默认值"
来源：http://ag.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ef.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://tz.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://ao.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uo.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://gk.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://vy.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://bt.hahajie.cn

[A16] 真假值判断规则
来源：http://jt.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yg.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://og.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nj.bookmarksfly.cn

TS:   if (!x) {}
来源：http://gy.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ol.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://is.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mm.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bb.hahajie.cn

[A17] 位运算
来源：http://ca.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://we.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ka.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oh.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oa.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eo.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kc.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ma.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jw.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://xx.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://ms.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://ng.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oz.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vb.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://fz.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://st.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://ie.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://uz.jctech888.com.cn

[A19] 交换两个变量
来源：http://lr.szxytkj.cn

Py:   a, b = b, a
来源：http://uo.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kw.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://eq.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://bx.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://hr.huixiangedu.cn

Go:   a, b = b, a
来源：http://dp.lnxyls.cn

Ruby: a, b = b, a
来源：http://zo.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://pr.huixiangedu.cn

[A20] 读取标准输入
来源：http://zx.asd995.cn

Py:   name = input("请输入：")
来源：http://qq.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lj.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://os.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://gn.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://lb.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ru.shxzskj.cn

Ruby: gets.chomp
来源：http://ke.hahajie.cn

C#:   Console.ReadLine();
来源：http://nk.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://vl.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://xz.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sv.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://tl.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://fc.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://ou.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ot.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://sm.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://ap.nicolike.cn

[A22] 获取字符串长度
来源：http://ke.asd995.cn

Py:   len(s)
来源：http://ai.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hk.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vw.jianghongdianzi.cn

TS:   s.length
来源：http://cy.yuntaijiaju.cn

Java: s.length()
来源：http://qv.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wd.muxihuayi.cn

Ruby: s.length
来源：http://cu.asd995.cn

C#:   s.Length
来源：http://co.bookmarksfly.cn

[A23] 大小写转换
来源：http://sm.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dh.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ys.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sa.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vv.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ng.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bx.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zn.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zw.lnxyls.cn

[A24] 去除首尾空白
来源：http://au.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jc.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ng.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kc.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hl.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ue.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://uw.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ik.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gc.shtwfgs.cn

[A25] 字符串比较
来源：http://ox.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://cg.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://td.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://so.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ps.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kd.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wx.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://og.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xq.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://bv.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mg.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jy.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tn.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://zk.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ay.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://if.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vo.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rc.bookmarksfly.cn

================================================================================
来源：http://ag.panjiajie.cn

B. 流程控制
来源：http://xx.shxzskj.cn

================================================================================
来源：http://pd.asd995.cn

[B01] 条件判断 if / else
来源：http://rs.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cw.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ii.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ma.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yr.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iu.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ce.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xq.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wp.nszjky.cn

[B02] 多分支 else if / elif
来源：http://mq.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jh.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://li.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mv.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bm.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jf.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nk.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jn.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xd.haigaiapp.cn

[B03] switch / match / case
来源：http://fj.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ts.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dh.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://st.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tc.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cd.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sz.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tk.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rp.huanxung.cn

[B04] for 计数循环
来源：http://ra.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://ku.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dp.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ri.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jg.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://we.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rf.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://vs.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sy.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://tb.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://vp.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://db.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tq.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xn.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wb.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gy.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://lx.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ol.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://we.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ni.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ux.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aj.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sx.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ib.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sw.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nv.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tj.chemitech.net.cn

[B07] while 循环
来源：http://od.hahajie.cn

Py:   while i < 10: i += 1
来源：http://xt.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dh.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://tj.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://yn.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://at.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ej.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://xl.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://xi.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://rj.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://od.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oj.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://yn.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://gs.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://of.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vq.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ob.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://dd.asd995.cn

[B09] break 与 continue
来源：http://pz.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zt.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xm.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eb.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zg.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gv.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dp.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pl.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://im.szsharing.cn

[B10] 遍历同时拿索引
来源：http://xd.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cr.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yu.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bz.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tp.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jm.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eo.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vk.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gc.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://dq.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://qy.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://al.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fq.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://br.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mg.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ay.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://ln.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ql.hnjuh.cn

[B12] 跳出多层循环
来源：http://nq.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oe.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wl.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aw.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://om.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://my.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yb.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ct.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rf.panjiajie.cn

[B13] 判断是否为数字
来源：http://hs.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://tx.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://dm.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://az.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bs.nszjky.cn

Java: x instanceof Number
来源：http://lt.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ud.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://jv.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://ck.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://qb.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://as.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dr.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://ao.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://wi.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pg.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bo.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gs.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sw.panjiajie.cn

[B15] 布尔运算与取反
来源：http://ga.shxzskj.cn

Py:   a and b or not c
来源：http://ku.9csxet.cn

PHP:  $a && $b || !$c
来源：http://pj.wgjwhj.cn

JS:   a && b || !c
来源：http://rp.szxytkj.cn

TS:   a && b || !c
来源：http://og.521024.cn

Java: a && b || !c
来源：http://vv.gzmigu.cn

Go:   a && b || !c
来源：http://mx.chemitech.net.cn

Ruby: a && b || !c
来源：http://gy.hnjuh.cn

C#:   a && b || !c
来源：http://tg.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xl.chemitech.net.cn

Py:   if not data: return
来源：http://jm.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://sa.yuexingan06.cn

JS:   if (!data) return;
来源：http://wj.521024.cn

TS:   if (!data) return;
来源：http://nd.hnjuh.cn

Java: if (data == null) return;
来源：http://ld.huanxung.cn

Go:   if data == nil { return }
来源：http://vy.521024.cn

Ruby: return if data.nil?
来源：http://vu.haigaiapp.cn

C#:   if (data == null) return;
来源：http://tl.521024.cn

================================================================================
来源：http://hu.shtwfgs.cn

C. 函数与作用域
来源：http://yg.bookmarksfly.cn

================================================================================
来源：http://tt.nszjky.cn

[C01] 定义函数
来源：http://mz.521024.cn

Py:   def add(a, b): return a + b
来源：http://vf.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ow.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://tn.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lg.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nt.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ua.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://so.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yc.haigaiapp.cn


<!-- 参考信息 -->