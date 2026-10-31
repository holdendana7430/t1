代发 wailian999

[A10] 生成随机数
来源：http://be.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://wc.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://dz.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gy.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zc.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://ml.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vy.521024.cn

Ruby: rand(1..100)
来源：http://ni.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://bx.9csxet.cn

[A11] 条件表达式（三元）
来源：http://tp.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://bm.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://eq.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dw.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ji.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ty.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sb.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wi.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://za.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://fb.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xj.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xf.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://yd.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://mp.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://bs.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wo.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://di.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://xg.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ox.nszjky.cn

Py:   "第一行\n第二行"
来源：http://dj.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://cw.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://io.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://tw.hahajie.cn

Java: "第一行\n第二行"
来源：http://ae.huanxung.cn

Go:   "第一行\n第二行"
来源：http://wx.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://dp.nicolike.cn

C#:   "第一行\n第二行"
来源：http://md.shtwfgs.cn

[A14] 注释写法
来源：http://qm.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ju.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uo.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://zb.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://ch.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wd.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://sv.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hu.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://rl.nszjky.cn

[A15] 空值判断与默认值
来源：http://us.huanxung.cn

Py:   value = data or "默认值"
来源：http://jl.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://pd.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://qq.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://fp.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cx.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://vs.nicolike.cn

Ruby: value = data || "默认值"
来源：http://by.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://ex.huixiangedu.cn

[A16] 真假值判断规则
来源：http://it.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://al.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cz.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gv.newstarts.cn

TS:   if (!x) {}
来源：http://go.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zm.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ta.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mk.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ga.bjjhwx.cn

[A17] 位运算
来源：http://gm.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qu.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ym.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ax.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aq.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mg.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rk.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cd.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vi.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://xf.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://pm.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://ix.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://de.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mm.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://ip.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xx.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://bb.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://cs.muxihuayi.cn

[A19] 交换两个变量
来源：http://le.jctech888.com.cn

Py:   a, b = b, a
来源：http://rx.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mc.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://py.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://rh.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://sa.521024.cn

Go:   a, b = b, a
来源：http://yt.newstarts.cn

Ruby: a, b = b, a
来源：http://co.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://pp.wgjwhj.cn

[A20] 读取标准输入
来源：http://si.lnxyls.cn

Py:   name = input("请输入：")
来源：http://sv.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kx.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ag.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://go.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://bd.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tx.colortex.cn

Ruby: gets.chomp
来源：http://tj.lnxyls.cn

C#:   Console.ReadLine();
来源：http://ng.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://wp.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://jy.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ef.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://un.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://wh.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://mx.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fi.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ai.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://ob.9csxet.cn

[A22] 获取字符串长度
来源：http://vm.shtwfgs.cn

Py:   len(s)
来源：http://zo.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ym.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wo.hahajie.cn

TS:   s.length
来源：http://jo.yuexingan06.cn

Java: s.length()
来源：http://qe.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kn.newstarts.cn

Ruby: s.length
来源：http://tc.haigaiapp.cn

C#:   s.Length
来源：http://gl.asd995.cn

[A23] 大小写转换
来源：http://np.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gv.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kf.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lm.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vq.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ib.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cd.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://di.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dk.lnxyls.cn

[A24] 去除首尾空白
来源：http://mc.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cz.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bj.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lq.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yp.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mi.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://sk.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ii.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lr.newstarts.cn

[A25] 字符串比较
来源：http://lz.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://ee.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ca.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gb.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ut.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mv.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lz.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rw.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qk.nicolike.cn

[A26] 类型转换总览
来源：http://ul.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sj.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lt.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fc.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://vq.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lm.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ad.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mm.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cr.panjiajie.cn

================================================================================
来源：http://mu.nicolike.cn

B. 流程控制
来源：http://ws.yuexingan06.cn

================================================================================
来源：http://wm.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://cq.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fy.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ja.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nl.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lg.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sl.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aj.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kq.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xs.9csxet.cn

[B02] 多分支 else if / elif
来源：http://qg.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mj.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bu.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cz.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ji.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ks.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hu.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mg.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rl.9csxet.cn

[B03] switch / match / case
来源：http://ew.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dk.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cj.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cm.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tj.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iu.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lc.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pi.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pl.yuexingan06.cn

[B04] for 计数循环
来源：http://dj.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://cf.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://av.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yr.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dd.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nj.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cr.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://cu.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cp.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://be.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://zz.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ua.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mn.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cy.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qz.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tf.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://wk.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eg.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://lq.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bf.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jx.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ju.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jz.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cq.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ui.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uf.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://el.521024.cn

[B07] while 循环
来源：http://vu.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://ms.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xv.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://dl.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://tg.521024.cn

Java: while (i < 10) { i++; }
来源：http://jz.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yq.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://br.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://vj.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://ol.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://da.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ax.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://yh.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://uz.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://un.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yq.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gu.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://dj.shtwfgs.cn

[B09] break 与 continue
来源：http://wf.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://re.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uk.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vq.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wj.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hl.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xh.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lf.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ht.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://jb.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pn.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ne.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xp.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mi.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ph.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://am.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nx.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xw.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://bx.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://pr.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://sl.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cd.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yo.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wh.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uk.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://gz.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lu.colortex.cn

[B12] 跳出多层循环
来源：http://mb.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bc.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sl.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cs.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gs.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://or.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ww.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xq.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://db.hnjuh.cn

[B13] 判断是否为数字
来源：http://ey.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://qk.colortex.cn

PHP:  is_numeric($x)
来源：http://oc.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qz.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bq.yuexingan06.cn

Java: x instanceof Number
来源：http://lh.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://th.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://bw.shxzskj.cn

C#:   x is int or double or decimal
来源：http://ai.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://wj.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://up.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gy.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://rn.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://is.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qe.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vf.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://az.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ib.hnjuh.cn

[B15] 布尔运算与取反
来源：http://rg.yuexingan06.cn

Py:   a and b or not c
来源：http://qt.nszjky.cn

PHP:  $a && $b || !$c
来源：http://cs.szsharing.cn

JS:   a && b || !c
来源：http://al.lnxyls.cn

TS:   a && b || !c
来源：http://te.nicolike.cn

Java: a && b || !c
来源：http://ke.nszjky.cn

Go:   a && b || !c
来源：http://nu.huanxung.cn

Ruby: a && b || !c
来源：http://zp.shtwfgs.cn

C#:   a && b || !c
来源：http://oh.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vh.bjjhwx.cn

Py:   if not data: return
来源：http://sl.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://ui.yuexingan06.cn

JS:   if (!data) return;
来源：http://km.bjjhwx.cn

TS:   if (!data) return;
来源：http://ti.hnjuh.cn

Java: if (data == null) return;
来源：http://yf.shxzukj.cn

Go:   if data == nil { return }
来源：http://ca.hnjuh.cn

Ruby: return if data.nil?
来源：http://tl.bjjhwx.cn

C#:   if (data == null) return;
来源：http://ps.gzmigu.cn


<!-- 参考信息 -->