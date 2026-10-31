代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xi.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://iz.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lx.shtwfgs.cn

Ruby: rand(1..100)
来源：http://qn.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://tj.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://zi.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://qp.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vr.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rd.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nl.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://mr.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gb.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tq.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bm.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://db.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kk.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ek.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://hq.colortex.cn

TS:   `Hello, ${name}!`
来源：http://lq.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://ae.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qk.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://ta.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://iz.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vf.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://ba.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://lz.nszjky.cn

JS:   "第一行\n第二行"
来源：http://yb.nszjky.cn

TS:   "第一行\n第二行"
来源：http://kz.521024.cn

Java: "第一行\n第二行"
来源：http://my.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://nk.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://kz.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://eu.9csxet.cn

[A14] 注释写法
来源：http://pv.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kf.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ur.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://ck.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://yu.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aa.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://xf.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oi.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://cs.colortex.cn

[A15] 空值判断与默认值
来源：http://dg.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://mw.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://tk.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://nl.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://iv.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mc.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://pp.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://tn.521024.cn

C#:   var value = data ?? "默认值";
来源：http://to.521024.cn

[A16] 真假值判断规则
来源：http://ha.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ca.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wt.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kk.gzmigu.cn

TS:   if (!x) {}
来源：http://pq.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rx.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qr.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wq.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ce.hnjuh.cn

[A17] 位运算
来源：http://vb.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gv.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fe.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ji.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xz.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tz.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gd.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jk.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://as.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://mg.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://yy.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://pp.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ai.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zw.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://kh.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pg.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://zw.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://qj.asd995.cn

[A19] 交换两个变量
来源：http://im.521024.cn

Py:   a, b = b, a
来源：http://jr.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qv.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://pf.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://hj.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://oh.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://sp.muxihuayi.cn

Ruby: a, b = b, a
来源：http://gc.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://kn.521024.cn

[A20] 读取标准输入
来源：http://gv.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://pd.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aj.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://gj.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://wx.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ek.huanxung.cn

Ruby: gets.chomp
来源：http://ui.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://ki.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://hg.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://mv.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mi.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://bw.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://lx.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://ub.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oh.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://vj.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://wj.huixiangedu.cn

[A22] 获取字符串长度
来源：http://ra.newstarts.cn

Py:   len(s)
来源：http://nb.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xo.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ng.hnjuh.cn

TS:   s.length
来源：http://xz.shxzskj.cn

Java: s.length()
来源：http://lf.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ly.gzmigu.cn

Ruby: s.length
来源：http://wa.panjiajie.cn

C#:   s.Length
来源：http://bi.haigaiapp.cn

[A23] 大小写转换
来源：http://jf.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cy.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://re.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fl.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iu.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ok.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ie.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bd.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qq.wgjwhj.cn

[A24] 去除首尾空白
来源：http://fn.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ab.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ph.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yr.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gy.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sh.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://uk.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mq.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sf.asd995.cn

[A25] 字符串比较
来源：http://jd.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://dx.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rb.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ia.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sk.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qr.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://py.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ex.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oy.wgjwhj.cn

[A26] 类型转换总览
来源：http://of.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://by.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ia.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ex.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://wv.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wz.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://km.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rv.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ek.521024.cn

================================================================================
来源：http://ru.yuntaijiaju.cn

B. 流程控制
来源：http://nx.521024.cn

================================================================================
来源：http://cv.hnjuh.cn

[B01] 条件判断 if / else
来源：http://vb.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nr.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ak.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bj.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ig.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tj.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xy.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hm.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mg.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://ry.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ef.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://va.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hy.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wu.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ep.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uh.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ps.nicolike.cn

[B03] switch / match / case
来源：http://in.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nl.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://us.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://as.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jd.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nj.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fu.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lx.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xl.yuntaijiaju.cn

[B04] for 计数循环
来源：http://rl.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://pi.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rq.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fm.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rf.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dh.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kp.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://lf.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lf.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://up.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://rk.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cb.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ui.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bw.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vw.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uq.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://nj.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cg.asd995.cn

[B06] 遍历字典 / 对象
来源：http://tp.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ow.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ik.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xo.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://os.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rs.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://li.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tj.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wu.muxihuayi.cn

[B07] while 循环
来源：http://nf.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://qu.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ui.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://hj.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://xk.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://gf.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sd.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://ob.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://ig.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://oq.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://od.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jw.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://gx.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://wh.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://ji.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ua.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xt.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://sz.lnxyls.cn

[B09] break 与 continue
来源：http://bf.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mh.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ik.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vr.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ma.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fi.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gc.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lp.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zj.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://tt.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sx.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xi.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sk.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vb.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sw.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tt.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ga.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://os.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://aj.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://xd.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://uf.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hb.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gm.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xy.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bb.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://jn.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dm.huixiangedu.cn

[B12] 跳出多层循环
来源：http://ma.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yt.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jo.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pw.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yy.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ql.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dv.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kg.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gf.shxzukj.cn

[B13] 判断是否为数字
来源：http://ga.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://rp.shxzukj.cn

PHP:  is_numeric($x)
来源：http://ng.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lv.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aj.hnjuh.cn

Java: x instanceof Number
来源：http://oe.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kl.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://tv.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://wx.hahajie.cn

[B14] 判断值是否在集合内
来源：http://vn.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ii.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ij.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://kx.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://lj.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://to.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fd.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://au.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ek.panjiajie.cn

[B15] 布尔运算与取反
来源：http://iw.yuntaijiaju.cn

Py:   a and b or not c
来源：http://fs.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://ym.szsharing.cn

JS:   a && b || !c
来源：http://rn.colortex.cn

TS:   a && b || !c
来源：http://xi.asd995.cn

Java: a && b || !c
来源：http://xk.hahajie.cn

Go:   a && b || !c
来源：http://ho.bookmarksfly.cn

Ruby: a && b || !c
来源：http://tw.szsharing.cn

C#:   a && b || !c
来源：http://oi.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ux.bjjhwx.cn

Py:   if not data: return
来源：http://ex.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://jv.nicolike.cn

JS:   if (!data) return;
来源：http://mz.nicolike.cn

TS:   if (!data) return;
来源：http://iv.9csxet.cn

Java: if (data == null) return;
来源：http://xp.shxzukj.cn

Go:   if data == nil { return }
来源：http://rc.lnxyls.cn

Ruby: return if data.nil?
来源：http://sy.shxzukj.cn

C#:   if (data == null) return;
来源：http://cs.huanxung.cn

================================================================================
来源：http://cp.haigaiapp.cn

C. 函数与作用域
来源：http://bx.asd995.cn

================================================================================
来源：http://lm.haigaiapp.cn

[C01] 定义函数
来源：http://vr.yuntaijiaju.cn


<!-- 参考信息 -->