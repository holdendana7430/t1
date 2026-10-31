代发 wailian999

[A10] 生成随机数
来源：http://vy.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://ic.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://sf.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hx.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bx.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://yw.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uk.hahajie.cn

Ruby: rand(1..100)
来源：http://wt.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://zt.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://jx.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://hm.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tu.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vx.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dr.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://fm.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lt.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vx.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://td.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://iq.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://og.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xv.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://rp.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://ae.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://dk.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nw.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://qr.asd995.cn

C#:   $"Hello, {name}!"
来源：http://th.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://td.nicolike.cn

Py:   "第一行\n第二行"
来源：http://ik.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://ii.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://oy.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://cg.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://rw.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://ab.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://ss.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://lk.yuexingan06.cn

[A14] 注释写法
来源：http://oy.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ja.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pi.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://vm.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://wu.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ys.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://xe.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bf.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://xm.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://qf.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://lj.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://af.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://ki.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://wy.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zm.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://lj.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://sv.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://zc.nszjky.cn

[A16] 真假值判断规则
来源：http://nt.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rt.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://od.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qx.muxihuayi.cn

TS:   if (!x) {}
来源：http://eb.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fi.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oj.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jf.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jx.colortex.cn

[A17] 位运算
来源：http://gd.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fh.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tw.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fu.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nq.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ml.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://do.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zx.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lc.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://ua.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://ob.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://me.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ie.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dd.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://ns.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ja.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://rv.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://zu.9csxet.cn

[A19] 交换两个变量
来源：http://sf.hnjuh.cn

Py:   a, b = b, a
来源：http://vr.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ez.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://ww.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://ob.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://xl.9csxet.cn

Go:   a, b = b, a
来源：http://tu.szxytkj.cn

Ruby: a, b = b, a
来源：http://zx.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://ws.521024.cn

[A20] 读取标准输入
来源：http://tb.shxzskj.cn

Py:   name = input("请输入：")
来源：http://pb.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nb.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gb.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://ej.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://ce.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gf.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://eu.szsharing.cn

C#:   Console.ReadLine();
来源：http://ry.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://jo.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://ox.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vq.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://bz.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://jd.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://wm.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uf.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://pj.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://xe.hnjuh.cn

[A22] 获取字符串长度
来源：http://gu.gzmigu.cn

Py:   len(s)
来源：http://ic.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bv.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fj.huixiangedu.cn

TS:   s.length
来源：http://if.huixinmuqiang.cn

Java: s.length()
来源：http://qx.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wg.jianghongdianzi.cn

Ruby: s.length
来源：http://sz.jctech888.com.cn

C#:   s.Length
来源：http://ac.gzmigu.cn

[A23] 大小写转换
来源：http://le.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ek.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vl.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rd.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zn.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fx.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ky.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bl.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qt.newstarts.cn

[A24] 去除首尾空白
来源：http://ec.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lk.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xf.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fk.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lz.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eb.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://ck.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rk.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kq.hahajie.cn

[A25] 字符串比较
来源：http://rd.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://ni.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ks.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ez.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://im.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://li.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zu.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yh.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qk.chemitech.net.cn

[A26] 类型转换总览
来源：http://xn.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vi.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oi.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iq.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://zy.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oe.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rl.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hk.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vh.shxzukj.cn

================================================================================
来源：http://iq.shtwfgs.cn

B. 流程控制
来源：http://qm.wgjwhj.cn

================================================================================
来源：http://tx.521024.cn

[B01] 条件判断 if / else
来源：http://mw.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vx.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://np.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pr.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bo.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fp.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nz.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zf.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ez.huanxung.cn

[B02] 多分支 else if / elif
来源：http://gm.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mo.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pz.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://za.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pz.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cf.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fh.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://on.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ll.shxzukj.cn

[B03] switch / match / case
来源：http://px.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gz.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ow.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wi.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jm.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dc.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gx.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vw.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xl.521024.cn

[B04] for 计数循环
来源：http://ku.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://qf.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yd.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cy.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vz.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://in.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dm.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://sc.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ea.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://pk.newstarts.cn

Py:   for item in arr: print(item)
来源：http://tj.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ep.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bg.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ye.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xq.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ai.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://hl.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yd.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://by.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ao.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dq.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mx.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oo.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gk.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pd.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fj.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hi.bjjhwx.cn

[B07] while 循环
来源：http://mj.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://zj.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mf.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://jx.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://fb.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://uo.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mu.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://dd.521024.cn

C#:   while (i < 10) { i++; }
来源：http://yz.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://kw.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://vm.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ph.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://zc.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://rs.521024.cn

Java: do { i++; } while (i < 10);
来源：http://je.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sj.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qj.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://hp.gzmigu.cn

[B09] break 与 continue
来源：http://yn.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hq.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gt.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vy.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dk.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ft.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ie.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yy.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.hahajie.cn

[B10] 遍历同时拿索引
来源：http://uy.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ce.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://us.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vy.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ue.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hr.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kt.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iy.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oi.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://cm.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://xh.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://yg.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ub.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zv.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uh.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://af.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://qq.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wc.panjiajie.cn

[B12] 跳出多层循环
来源：http://aw.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lo.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hb.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mb.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mx.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mt.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uj.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://df.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ux.colortex.cn

[B13] 判断是否为数字
来源：http://lu.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://pw.shxzukj.cn

PHP:  is_numeric($x)
来源：http://sg.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ow.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qw.yuexingan06.cn

Java: x instanceof Number
来源：http://bi.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cx.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://eu.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://vf.hahajie.cn

[B14] 判断值是否在集合内
来源：http://lc.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lq.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ag.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://xl.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://sg.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://su.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://og.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sn.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://em.newstarts.cn

[B15] 布尔运算与取反
来源：http://hs.yuexingan06.cn

Py:   a and b or not c
来源：http://to.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://hq.jctech888.com.cn

JS:   a && b || !c
来源：http://gx.wgjwhj.cn

TS:   a && b || !c
来源：http://qj.panjiajie.cn

Java: a && b || !c
来源：http://on.huanxung.cn

Go:   a && b || !c
来源：http://pc.hahajie.cn

Ruby: a && b || !c
来源：http://ku.bookmarksfly.cn

C#:   a && b || !c
来源：http://oy.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://at.bjjhwx.cn

Py:   if not data: return
来源：http://of.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://nk.huanxung.cn

JS:   if (!data) return;
来源：http://ge.wgjwhj.cn

TS:   if (!data) return;
来源：http://fm.hahajie.cn

Java: if (data == null) return;
来源：http://xn.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://gt.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://gv.asd995.cn

C#:   if (data == null) return;
来源：http://ty.asd995.cn


<!-- 参考信息 -->