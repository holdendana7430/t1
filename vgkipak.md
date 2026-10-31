代发 wailian999

[A10] 生成随机数
来源：http://gz.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://js.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://yq.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qd.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gc.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ie.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jz.nicolike.cn

Ruby: rand(1..100)
来源：http://lo.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://si.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://ew.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://nc.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xg.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kp.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hk.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://kl.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lj.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ct.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ry.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://do.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ai.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sw.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://zj.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://au.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://bw.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pi.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://hd.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://zt.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pc.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://xy.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://mb.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://sr.huanxung.cn

TS:   "第一行\n第二行"
来源：http://el.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://em.9csxet.cn

Go:   "第一行\n第二行"
来源：http://zl.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://vm.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://qa.yuexingan06.cn

[A14] 注释写法
来源：http://bu.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qy.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ea.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://ez.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://zi.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zq.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://pe.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pl.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://sm.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://xd.9csxet.cn

Py:   value = data or "默认值"
来源：http://ho.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://ho.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://xo.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://hk.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cx.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://it.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://kl.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://gg.jctech888.com.cn

[A16] 真假值判断规则
来源：http://ak.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tv.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mm.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vl.haigaiapp.cn

TS:   if (!x) {}
来源：http://rh.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bb.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sr.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ch.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bu.colortex.cn

[A17] 位运算
来源：http://jl.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ms.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ea.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zw.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zs.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://af.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fo.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://do.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zc.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://uq.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://uz.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://id.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mb.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://se.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://zo.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qt.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://hr.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://wc.hnjuh.cn

[A19] 交换两个变量
来源：http://mq.huixiangedu.cn

Py:   a, b = b, a
来源：http://iy.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ok.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://qh.521024.cn

TS:   [a, b] = [b, a];
来源：http://hz.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://xy.szsharing.cn

Go:   a, b = b, a
来源：http://hb.huixiangedu.cn

Ruby: a, b = b, a
来源：http://gz.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://ph.panjiajie.cn

[A20] 读取标准输入
来源：http://cg.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://mr.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tf.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cj.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://ji.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://jf.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ge.chemitech.net.cn

Ruby: gets.chomp
来源：http://to.huanxung.cn

C#:   Console.ReadLine();
来源：http://ai.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://md.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://ak.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ob.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://pt.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://ir.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://jj.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bl.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ei.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://ov.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://re.shxzukj.cn

Py:   len(s)
来源：http://zb.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hr.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vp.szxytkj.cn

TS:   s.length
来源：http://bl.huixinmuqiang.cn

Java: s.length()
来源：http://ij.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ze.nszjky.cn

Ruby: s.length
来源：http://qn.shxzskj.cn

C#:   s.Length
来源：http://bd.szxytkj.cn

[A23] 大小写转换
来源：http://ep.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ni.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ul.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vz.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lj.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ff.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kk.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gi.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pg.yuexingan06.cn

[A24] 去除首尾空白
来源：http://xr.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bn.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sm.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wq.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zu.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://li.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://xg.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://up.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://su.bookmarksfly.cn

[A25] 字符串比较
来源：http://hs.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://ap.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yq.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qu.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vf.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://za.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yb.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zj.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jg.panjiajie.cn

[A26] 类型转换总览
来源：http://sg.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hn.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ry.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pj.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://ze.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wk.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zl.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zg.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cp.huixiangedu.cn

================================================================================
来源：http://io.shxzukj.cn

B. 流程控制
来源：http://nk.huixiangedu.cn

================================================================================
来源：http://sv.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://wa.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jp.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://od.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://je.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hv.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cd.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vy.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://de.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://th.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://qw.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sx.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ym.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://de.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hn.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://so.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qx.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gs.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bb.yuexingan06.cn

[B03] switch / match / case
来源：http://mn.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qd.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cl.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zq.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jb.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jp.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://it.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ey.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rg.chemitech.net.cn

[B04] for 计数循环
来源：http://rg.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://ym.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uf.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nk.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wy.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fe.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dn.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://wm.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ex.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://hb.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://dv.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://od.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wh.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qj.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tm.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wr.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://eo.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xp.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://pb.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qs.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mo.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://va.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sm.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ih.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xy.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://op.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uk.gzmigu.cn

[B07] while 循环
来源：http://mm.hahajie.cn

Py:   while i < 10: i += 1
来源：http://jh.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ip.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://no.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://jj.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://kl.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mg.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://vy.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://ah.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ww.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://fv.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ew.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://cg.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://bp.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://zg.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rm.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dn.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://fs.haigaiapp.cn

[B09] break 与 continue
来源：http://xu.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qb.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cd.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zy.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sz.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://np.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ga.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://lh.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vg.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://je.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xg.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rt.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gf.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rt.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mr.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ct.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://dq.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://qh.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://el.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ip.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xh.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yg.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ik.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://vm.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zn.shxzskj.cn

[B12] 跳出多层循环
来源：http://xd.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ze.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ua.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jx.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xo.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qs.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xz.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://np.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tf.newstarts.cn

[B13] 判断是否为数字
来源：http://wz.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://pc.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://vd.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bn.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fx.gzmigu.cn

Java: x instanceof Number
来源：http://xl.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://du.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://gr.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://qt.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://jt.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yl.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mo.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://xs.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://fh.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ud.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dw.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vi.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ov.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://yv.hahajie.cn

Py:   a and b or not c
来源：http://xy.nicolike.cn

PHP:  $a && $b || !$c
来源：http://xm.bookmarksfly.cn

JS:   a && b || !c
来源：http://ct.wgjwhj.cn

TS:   a && b || !c
来源：http://xa.9csxet.cn

Java: a && b || !c
来源：http://sm.lnxyls.cn

Go:   a && b || !c
来源：http://rs.nszjky.cn

Ruby: a && b || !c
来源：http://nl.nicolike.cn

C#:   a && b || !c
来源：http://do.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lc.haigaiapp.cn

Py:   if not data: return
来源：http://mn.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://vi.haigaiapp.cn

JS:   if (!data) return;
来源：http://gh.newstarts.cn

TS:   if (!data) return;
来源：http://ev.haigaiapp.cn

Java: if (data == null) return;
来源：http://is.szsharing.cn

Go:   if data == nil { return }
来源：http://ka.nicolike.cn

Ruby: return if data.nil?
来源：http://bs.chemitech.net.cn

C#:   if (data == null) return;
来源：http://xp.panjiajie.cn


<!-- 参考信息 -->