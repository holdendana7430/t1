代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://jf.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rv.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://qk.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gw.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sg.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://lt.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://vz.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://lf.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://og.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://si.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://hj.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cb.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://he.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://fc.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://qf.hahajie.cn

TS:   "第一行\n第二行"
来源：http://gd.521024.cn

Java: "第一行\n第二行"
来源：http://go.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://pt.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://zl.521024.cn

C#:   "第一行\n第二行"
来源：http://fq.huanxung.cn

[A14] 注释写法
来源：http://qw.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://at.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://su.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://gl.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://np.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ro.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://vw.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://af.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://sk.asd995.cn

[A15] 空值判断与默认值
来源：http://gl.9csxet.cn

Py:   value = data or "默认值"
来源：http://sa.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://wm.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://nq.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://du.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cb.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://wn.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://yf.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://xf.shxzukj.cn

[A16] 真假值判断规则
来源：http://rv.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ef.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nt.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://an.huixiangedu.cn

TS:   if (!x) {}
来源：http://pl.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://li.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bj.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mp.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rn.hahajie.cn

[A17] 位运算
来源：http://fc.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ti.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wl.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rm.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nz.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hv.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fi.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ps.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qr.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://ia.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://qz.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://yt.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://go.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ln.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://kx.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sb.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://pe.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://ca.jctech888.com.cn

[A19] 交换两个变量
来源：http://zi.wgjwhj.cn

Py:   a, b = b, a
来源：http://as.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cg.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://se.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://um.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://zg.shxzskj.cn

Go:   a, b = b, a
来源：http://ms.muxihuayi.cn

Ruby: a, b = b, a
来源：http://jk.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://cm.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://xk.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://rl.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ah.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ge.521024.cn

TS:   // Node.js：readline 模块
来源：http://fg.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://mo.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ry.muxihuayi.cn

Ruby: gets.chomp
来源：http://jn.newstarts.cn

C#:   Console.ReadLine();
来源：http://qr.szsharing.cn

[A21] 保留指定小数位输出
来源：http://ib.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://ca.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vs.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://tn.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://tg.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://qq.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mw.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://tg.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://pp.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://gh.nicolike.cn

Py:   len(s)
来源：http://iq.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kj.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ms.szxytkj.cn

TS:   s.length
来源：http://ip.panjiajie.cn

Java: s.length()
来源：http://iv.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yn.newstarts.cn

Ruby: s.length
来源：http://jh.bjjhwx.cn

C#:   s.Length
来源：http://he.nszjky.cn

[A23] 大小写转换
来源：http://gl.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ne.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ww.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fh.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vf.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ki.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yi.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jq.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wd.yuexingan06.cn

[A24] 去除首尾空白
来源：http://md.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ag.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ph.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rs.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rq.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bt.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://eq.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mx.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mg.szsharing.cn

[A25] 字符串比较
来源：http://eg.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://hc.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ju.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cr.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gw.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wz.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xk.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yx.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ip.yuexingan06.cn

[A26] 类型转换总览
来源：http://tt.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zl.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ed.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://me.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://oo.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oo.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://er.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://up.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iw.shxzskj.cn

================================================================================
来源：http://vc.nszjky.cn

B. 流程控制
来源：http://pq.newstarts.cn

================================================================================
来源：http://gw.newstarts.cn

[B01] 条件判断 if / else
来源：http://rd.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://no.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://en.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zi.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xw.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ox.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lg.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ns.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yo.nicolike.cn

[B02] 多分支 else if / elif
来源：http://bx.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nc.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ub.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ka.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qv.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ud.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vz.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ze.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ia.yuexingan06.cn

[B03] switch / match / case
来源：http://su.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pa.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ta.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pb.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pn.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vu.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yg.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fg.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xg.wgjwhj.cn

[B04] for 计数循环
来源：http://dn.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://lk.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ez.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kb.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oz.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ac.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bs.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://jv.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qc.521024.cn

[B05] 遍历数组 / 列表
来源：http://zl.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://ch.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zr.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hv.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sx.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xh.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://no.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://uv.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ly.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://jm.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cm.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sl.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ig.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mn.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oh.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jo.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://be.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://md.hnjuh.cn

[B07] while 循环
来源：http://qj.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://zy.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jb.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://sq.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://rp.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://jn.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dk.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://wp.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://yf.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://pv.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://yu.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tj.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://zm.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://ff.521024.cn

Java: do { i++; } while (i < 10);
来源：http://my.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yk.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nw.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://vn.nszjky.cn

[B09] break 与 continue
来源：http://vx.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zt.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fv.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vx.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kc.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pj.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jo.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tu.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lj.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://gv.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jn.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jf.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://on.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qe.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oz.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wy.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hq.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hq.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://gb.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://ft.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://mg.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://if.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xz.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ig.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ii.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://ib.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yp.nicolike.cn

[B12] 跳出多层循环
来源：http://xe.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xo.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zn.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ll.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://im.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cg.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ta.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pg.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gv.yuexingan06.cn

[B13] 判断是否为数字
来源：http://ev.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://tv.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://mm.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kk.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ri.nicolike.cn

Java: x instanceof Number
来源：http://mm.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oy.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://xs.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://yg.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://we.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tf.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gt.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://fa.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://rh.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ux.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nm.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xu.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://do.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://dj.haigaiapp.cn

Py:   a and b or not c
来源：http://ro.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://kj.nszjky.cn

JS:   a && b || !c
来源：http://hk.huanxung.cn

TS:   a && b || !c
来源：http://xk.panjiajie.cn

Java: a && b || !c
来源：http://gu.bjjhwx.cn

Go:   a && b || !c
来源：http://if.jctech888.com.cn

Ruby: a && b || !c
来源：http://dp.yuexingan06.cn

C#:   a && b || !c
来源：http://tn.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lw.chemitech.net.cn

Py:   if not data: return
来源：http://mp.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://wg.yuexingan06.cn

JS:   if (!data) return;
来源：http://vq.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://jv.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://qy.shtwfgs.cn

Go:   if data == nil { return }
来源：http://jt.shtwfgs.cn

Ruby: return if data.nil?
来源：http://rw.yuexingan06.cn

C#:   if (data == null) return;
来源：http://dw.chemitech.net.cn

================================================================================
来源：http://pc.huixiangedu.cn

C. 函数与作用域
来源：http://fh.yuntaijiaju.cn

================================================================================
来源：http://ro.yuntaijiaju.cn

[C01] 定义函数
来源：http://ki.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://ri.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://py.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://xv.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mm.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lm.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ma.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://sq.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hm.wgjwhj.cn

[C02] 默认参数
来源：http://br.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://zz.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yc.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qc.jctech888.com.cn


<!-- 参考信息 -->