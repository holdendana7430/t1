代发 wailian999

[A10] 生成随机数
来源：http://og.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://jr.huanxung.cn

PHP:  random_int(1, 100);
来源：http://uf.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zw.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eq.chemitech.net.cn

Java: new Random().nextInt(100) + 1
来源：http://wv.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bg.nicolike.cn

Ruby: rand(1..100)
来源：http://pz.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://id.szsharing.cn

[A11] 条件表达式（三元）
来源：http://kp.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://xp.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rw.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qd.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uq.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://fb.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ih.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://th.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lt.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://bb.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ko.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rw.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://gz.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://iw.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://gd.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dj.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://ju.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://ly.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://od.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://kz.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://mt.newstarts.cn

JS:   "第一行\n第二行"
来源：http://zc.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://tp.panjiajie.cn

Java: "第一行\n第二行"
来源：http://xs.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://kx.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://ez.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://vy.panjiajie.cn

[A14] 注释写法
来源：http://dl.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hb.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nh.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://ag.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://lg.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yg.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://zq.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ec.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://vq.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://nr.521024.cn

Py:   value = data or "默认值"
来源：http://ke.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ob.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://ij.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://ff.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fz.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://er.newstarts.cn

Ruby: value = data || "默认值"
来源：http://lo.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://qg.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://rv.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hl.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ah.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mn.bookmarksfly.cn

TS:   if (!x) {}
来源：http://ub.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rw.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fu.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dk.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dj.newstarts.cn

[A17] 位运算
来源：http://zd.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lh.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://do.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://og.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fa.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ja.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ke.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bt.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dr.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://ve.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://ib.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://ax.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dd.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dg.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://xk.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pg.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://ij.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://ip.huanxung.cn

[A19] 交换两个变量
来源：http://cc.gzmigu.cn

Py:   a, b = b, a
来源：http://fv.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jd.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://zd.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://it.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://iq.colortex.cn

Go:   a, b = b, a
来源：http://gj.nicolike.cn

Ruby: a, b = b, a
来源：http://ii.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://zp.colortex.cn

[A20] 读取标准输入
来源：http://nv.shxzskj.cn

Py:   name = input("请输入：")
来源：http://fd.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lj.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wv.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://iy.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://qo.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mw.hnjuh.cn

Ruby: gets.chomp
来源：http://he.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://rm.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://rr.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://jt.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ce.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://zp.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://ha.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://yg.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bt.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ck.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://hm.hahajie.cn

[A22] 获取字符串长度
来源：http://zg.bjjhwx.cn

Py:   len(s)
来源：http://ew.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gl.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yk.muxihuayi.cn

TS:   s.length
来源：http://pb.panjiajie.cn

Java: s.length()
来源：http://ks.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ou.jctech888.com.cn

Ruby: s.length
来源：http://zm.huixiangedu.cn

C#:   s.Length
来源：http://nm.panjiajie.cn

[A23] 大小写转换
来源：http://cm.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mv.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oq.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ft.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hw.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ws.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://th.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xv.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gz.panjiajie.cn

[A24] 去除首尾空白
来源：http://oe.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ku.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lm.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lh.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pl.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://io.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://xg.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bz.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sb.jianghongdianzi.cn

[A25] 字符串比较
来源：http://qp.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://ag.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wa.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zc.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ge.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dx.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sw.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vp.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nk.haigaiapp.cn

[A26] 类型转换总览
来源：http://co.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fg.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vq.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fg.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://fr.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ki.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dg.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mo.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ni.nszjky.cn

================================================================================
来源：http://oh.hnjuh.cn

B. 流程控制
来源：http://cc.jianghongdianzi.cn

================================================================================
来源：http://im.hahajie.cn

[B01] 条件判断 if / else
来源：http://xa.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rz.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ic.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bs.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wj.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qp.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ud.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lf.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bd.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://ls.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://od.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ja.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qh.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wl.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ve.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hd.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dk.nszjky.cn

[B03] switch / match / case
来源：http://md.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ku.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bp.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wo.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xq.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mb.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://np.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rv.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ci.hnjuh.cn

[B04] for 计数循环
来源：http://sy.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://bj.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wn.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ld.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ca.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pi.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ez.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://ny.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hg.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://sl.521024.cn

Py:   for item in arr: print(item)
来源：http://ff.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kq.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://df.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ek.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yf.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kj.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://us.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uz.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://wa.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eg.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vi.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zo.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vf.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ow.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fv.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fv.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xc.szsharing.cn

[B07] while 循环
来源：http://uu.colortex.cn

Py:   while i < 10: i += 1
来源：http://le.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ov.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://jf.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://hm.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://sm.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gq.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://ne.521024.cn

C#:   while (i < 10) { i++; }
来源：http://if.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://iq.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://ym.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nw.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://jz.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://hx.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://yd.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wi.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://aq.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://lh.newstarts.cn

[B09] break 与 continue
来源：http://id.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mj.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ns.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ox.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aw.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dp.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ot.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gx.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fd.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://yw.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gb.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vf.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sv.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tn.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nh.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zp.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rh.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dk.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://xn.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://li.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://aj.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kw.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hy.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wf.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rk.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://wh.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yc.asd995.cn

[B12] 跳出多层循环
来源：http://iy.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nh.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cc.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ez.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://um.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://am.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ea.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cv.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dk.bjjhwx.cn

[B13] 判断是否为数字
来源：http://py.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://df.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://zb.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ig.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xz.521024.cn

Java: x instanceof Number
来源：http://uo.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tv.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://pb.asd995.cn

C#:   x is int or double or decimal
来源：http://gg.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://ci.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wt.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://no.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://nd.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://av.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ez.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wz.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mn.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zh.hahajie.cn

[B15] 布尔运算与取反
来源：http://al.nszjky.cn

Py:   a and b or not c
来源：http://rq.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://dx.muxihuayi.cn

JS:   a && b || !c
来源：http://ea.chemitech.net.cn

TS:   a && b || !c
来源：http://ki.newstarts.cn

Java: a && b || !c
来源：http://jw.panjiajie.cn

Go:   a && b || !c
来源：http://rp.521024.cn

Ruby: a && b || !c
来源：http://sk.hahajie.cn

C#:   a && b || !c
来源：http://za.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ku.hnjuh.cn

Py:   if not data: return
来源：http://wa.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://uh.bookmarksfly.cn

JS:   if (!data) return;
来源：http://nd.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://rf.nszjky.cn

Java: if (data == null) return;
来源：http://ko.nszjky.cn

Go:   if data == nil { return }
来源：http://uc.nicolike.cn

Ruby: return if data.nil?
来源：http://cb.nicolike.cn

C#:   if (data == null) return;
来源：http://jq.bjjhwx.cn


<!-- 参考信息 -->