代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://vo.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://pq.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://yv.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nx.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cp.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qm.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://dt.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wz.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qe.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fv.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://dx.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yz.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zw.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://sw.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://jx.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://nd.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ma.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ix.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://vx.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ev.nszjky.cn

Py:   "第一行\n第二行"
来源：http://lg.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://do.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://cz.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://rx.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://pa.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://nw.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://rd.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://sj.gzmigu.cn

[A14] 注释写法
来源：http://lp.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oy.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cv.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://vs.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://ha.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uy.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://bu.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ha.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://kj.huanxung.cn

[A15] 空值判断与默认值
来源：http://tl.lnxyls.cn

Py:   value = data or "默认值"
来源：http://de.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://wu.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://lj.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://yz.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kj.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://er.huanxung.cn

Ruby: value = data || "默认值"
来源：http://ue.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://hl.panjiajie.cn

[A16] 真假值判断规则
来源：http://ik.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bh.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rx.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hx.chemitech.net.cn

TS:   if (!x) {}
来源：http://hk.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vy.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ng.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uz.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://te.panjiajie.cn

[A17] 位运算
来源：http://qg.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ej.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pj.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zi.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tv.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dg.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kc.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yo.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kv.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://sz.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://tv.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://st.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iw.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cl.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://zz.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xz.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://jz.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://ee.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://qb.lnxyls.cn

Py:   a, b = b, a
来源：http://gc.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ji.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://fd.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://kz.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://bm.colortex.cn

Go:   a, b = b, a
来源：http://tr.huixiangedu.cn

Ruby: a, b = b, a
来源：http://iz.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://gu.shxzskj.cn

[A20] 读取标准输入
来源：http://ek.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://fm.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://au.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kl.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://rh.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://qk.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://if.shxzukj.cn

Ruby: gets.chomp
来源：http://hp.huanxung.cn

C#:   Console.ReadLine();
来源：http://xs.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://nm.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://uf.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gs.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://tc.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://ek.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://wo.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hu.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://sx.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://sg.muxihuayi.cn

[A22] 获取字符串长度
来源：http://cw.huanxung.cn

Py:   len(s)
来源：http://ps.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yz.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jd.shtwfgs.cn

TS:   s.length
来源：http://cr.hnjuh.cn

Java: s.length()
来源：http://ls.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xq.chemitech.net.cn

Ruby: s.length
来源：http://ln.shxzskj.cn

C#:   s.Length
来源：http://tv.colortex.cn

[A23] 大小写转换
来源：http://wu.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ss.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hu.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mb.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://th.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ls.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qn.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pi.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://em.wgjwhj.cn

[A24] 去除首尾空白
来源：http://zz.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xu.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cu.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tw.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mc.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xh.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://tx.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lh.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hc.jctech888.com.cn

[A25] 字符串比较
来源：http://rm.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://ob.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gp.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bi.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wy.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kn.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fe.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ob.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ub.huixiangedu.cn

[A26] 类型转换总览
来源：http://nt.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dh.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cf.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oy.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://ef.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://at.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dz.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pw.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jm.shxzukj.cn

================================================================================
来源：http://hg.colortex.cn

B. 流程控制
来源：http://ky.hnjuh.cn

================================================================================
来源：http://sa.hnjuh.cn

[B01] 条件判断 if / else
来源：http://et.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tu.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ee.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://us.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bq.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jp.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://te.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xe.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hh.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://ta.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ta.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nc.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qi.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xx.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lb.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://po.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xk.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hf.haigaiapp.cn

[B03] switch / match / case
来源：http://yc.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bn.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vy.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yl.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ak.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mh.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ab.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sy.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rl.9csxet.cn

[B04] for 计数循环
来源：http://sy.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://fn.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cj.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xc.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tm.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qe.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gx.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://yi.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yw.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://at.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://sk.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cq.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://en.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lb.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sl.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qs.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://wg.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xq.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://un.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hu.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zo.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mb.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xl.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vz.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dt.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mg.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lf.muxihuayi.cn

[B07] while 循环
来源：http://te.nicolike.cn

Py:   while i < 10: i += 1
来源：http://fb.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zn.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://vf.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://gx.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://dp.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gr.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://px.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://gm.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://in.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://vp.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jc.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://ht.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://er.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://sr.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rc.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xj.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://ae.nicolike.cn

[B09] break 与 continue
来源：http://wy.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kn.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rh.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sa.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uj.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mt.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gl.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cx.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rp.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://os.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iz.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yp.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qh.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://om.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ae.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pg.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ou.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ov.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://pn.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://rq.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://pf.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ow.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fj.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ad.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bf.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://oh.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ba.jctech888.com.cn

[B12] 跳出多层循环
来源：http://hy.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://th.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://df.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://te.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://po.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hu.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jy.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vp.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zl.shxzukj.cn

[B13] 判断是否为数字
来源：http://ph.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://ft.huanxung.cn

PHP:  is_numeric($x)
来源：http://sc.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ig.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kf.colortex.cn

Java: x instanceof Number
来源：http://tk.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sk.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://ae.lnxyls.cn

C#:   x is int or double or decimal
来源：http://pl.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://hh.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dv.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cb.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://dc.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://do.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://we.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zp.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yg.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nl.huanxung.cn

[B15] 布尔运算与取反
来源：http://nq.muxihuayi.cn

Py:   a and b or not c
来源：http://hx.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://hf.nszjky.cn

JS:   a && b || !c
来源：http://ex.asd995.cn

TS:   a && b || !c
来源：http://ir.nszjky.cn

Java: a && b || !c
来源：http://mn.hahajie.cn

Go:   a && b || !c
来源：http://gp.lnxyls.cn

Ruby: a && b || !c
来源：http://eb.9csxet.cn

C#:   a && b || !c
来源：http://kv.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ou.szsharing.cn

Py:   if not data: return
来源：http://qf.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://er.nicolike.cn

JS:   if (!data) return;
来源：http://rw.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://ia.nicolike.cn

Java: if (data == null) return;
来源：http://kt.panjiajie.cn

Go:   if data == nil { return }
来源：http://nc.shxzukj.cn

Ruby: return if data.nil?
来源：http://cu.panjiajie.cn

C#:   if (data == null) return;
来源：http://pw.shxzukj.cn

================================================================================
来源：http://xy.bjjhwx.cn

C. 函数与作用域
来源：http://si.panjiajie.cn

================================================================================
来源：http://zl.wgjwhj.cn

[C01] 定义函数
来源：http://ec.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://fs.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bw.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://bs.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xi.asd995.cn


<!-- 参考信息 -->