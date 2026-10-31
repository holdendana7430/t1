代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ro.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cc.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vh.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ev.nszjky.cn

[A10] 生成随机数
来源：http://kk.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://ga.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://ja.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pt.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://na.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://im.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://na.hahajie.cn

Ruby: rand(1..100)
来源：http://ze.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://gt.asd995.cn

[A11] 条件表达式（三元）
来源：http://xw.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://bg.shxzskj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://il.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gz.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ef.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://eu.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bu.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vw.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qq.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://lk.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iu.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xd.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://el.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://mk.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://nm.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fx.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://ze.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://ki.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://we.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://ep.colortex.cn

PHP:  "第一行\n第二行"
来源：http://ys.521024.cn

JS:   "第一行\n第二行"
来源：http://vl.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://fs.gzmigu.cn

Java: "第一行\n第二行"
来源：http://ch.huanxung.cn

Go:   "第一行\n第二行"
来源：http://cb.colortex.cn

Ruby: "第一行\n第二行"
来源：http://ji.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://da.muxihuayi.cn

[A14] 注释写法
来源：http://ro.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://od.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kk.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://ut.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://ne.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uq.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://jk.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sg.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://ha.lnxyls.cn

[A15] 空值判断与默认值
来源：http://sw.shxzukj.cn

Py:   value = data or "默认值"
来源：http://oy.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://qd.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://cn.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://ga.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gs.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://zx.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://ec.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://ld.huixiangedu.cn

[A16] 真假值判断规则
来源：http://qs.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qv.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uz.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aj.muxihuayi.cn

TS:   if (!x) {}
来源：http://tc.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qp.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zi.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cm.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wn.huixiangedu.cn

[A17] 位运算
来源：http://hq.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pi.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mr.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ht.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iu.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nq.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hr.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://me.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vf.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://lb.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://up.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://so.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dh.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yb.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://xc.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dx.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://bi.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://ld.chemitech.net.cn

[A19] 交换两个变量
来源：http://wx.colortex.cn

Py:   a, b = b, a
来源：http://iq.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sl.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://so.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://ce.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://qf.panjiajie.cn

Go:   a, b = b, a
来源：http://ey.nszjky.cn

Ruby: a, b = b, a
来源：http://wp.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://ly.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://uq.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://mw.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hp.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oy.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://mf.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://mq.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ry.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://fp.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://rz.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://yn.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://dk.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ga.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://zv.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://dr.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://tc.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rw.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://ng.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://yt.lnxyls.cn

[A22] 获取字符串长度
来源：http://wb.bookmarksfly.cn

Py:   len(s)
来源：http://lj.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ha.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ui.szsharing.cn

TS:   s.length
来源：http://zq.bookmarksfly.cn

Java: s.length()
来源：http://ur.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cw.huixinmuqiang.cn

Ruby: s.length
来源：http://pp.nszjky.cn

C#:   s.Length
来源：http://fd.bjjhwx.cn

[A23] 大小写转换
来源：http://kj.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wc.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dq.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qo.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sz.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yq.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ib.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bd.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bx.muxihuayi.cn

[A24] 去除首尾空白
来源：http://ob.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jz.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://by.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://np.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wy.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oa.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://dv.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://um.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vj.gzmigu.cn

[A25] 字符串比较
来源：http://xt.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://ck.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ti.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zf.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qz.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yg.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eu.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xr.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xk.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://zt.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nv.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cy.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oj.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://oo.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yw.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://al.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lo.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yt.shxzskj.cn

================================================================================
来源：http://qo.shtwfgs.cn

B. 流程控制
来源：http://oj.shxzskj.cn

================================================================================
来源：http://kn.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://jm.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lw.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rq.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mi.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yj.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eu.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://my.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nw.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yc.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://hj.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rj.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cv.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wp.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qz.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vz.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sd.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bn.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ae.huanxung.cn

[B03] switch / match / case
来源：http://cf.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ok.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cm.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://er.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rt.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pk.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pe.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ya.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tt.shxzukj.cn

[B04] for 计数循环
来源：http://qp.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://kc.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gp.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zd.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mz.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kx.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gq.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://ng.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wp.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://sg.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://in.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dx.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ki.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ml.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jn.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ov.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://hw.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jx.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://zq.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://er.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sb.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nx.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://km.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xn.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zf.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://po.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://py.521024.cn

[B07] while 循环
来源：http://om.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://eq.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ax.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://jr.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://xo.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://cs.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ss.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ad.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://sy.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://ih.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://sk.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dg.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://cq.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://tn.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://jl.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ig.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mm.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://hv.huanxung.cn

[B09] break 与 continue
来源：http://hv.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lg.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mt.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tz.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zw.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ss.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lz.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ue.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://ed.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tr.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fg.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vu.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sc.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pz.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qn.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jz.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dc.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://aw.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://pm.521024.cn

PHP:  range(0, 10, 2);
来源：http://gb.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xo.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aq.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vw.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bc.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://cz.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jt.huanxung.cn

[B12] 跳出多层循环
来源：http://jo.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xh.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xi.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hk.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ii.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gh.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lo.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mz.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sy.wgjwhj.cn

[B13] 判断是否为数字
来源：http://vv.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://to.colortex.cn

PHP:  is_numeric($x)
来源：http://hb.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ug.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sp.hahajie.cn

Java: x instanceof Number
来源：http://rl.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vk.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://wn.lnxyls.cn

C#:   x is int or double or decimal
来源：http://iq.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://zc.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cg.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qw.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://lz.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://jp.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yj.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ol.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ec.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vm.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://vj.nszjky.cn

Py:   a and b or not c
来源：http://vc.nicolike.cn

PHP:  $a && $b || !$c
来源：http://zy.wgjwhj.cn

JS:   a && b || !c
来源：http://cd.wgjwhj.cn

TS:   a && b || !c
来源：http://gm.shtwfgs.cn

Java: a && b || !c
来源：http://je.lnxyls.cn

Go:   a && b || !c
来源：http://ul.newstarts.cn

Ruby: a && b || !c
来源：http://mw.newstarts.cn

C#:   a && b || !c
来源：http://lh.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uc.hahajie.cn

Py:   if not data: return
来源：http://gp.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://av.shxzukj.cn

JS:   if (!data) return;
来源：http://an.521024.cn

TS:   if (!data) return;
来源：http://ab.bookmarksfly.cn


<!-- 参考信息 -->