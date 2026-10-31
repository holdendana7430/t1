代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ih.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cs.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nk.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cp.huanxung.cn

[A10] 生成随机数
来源：http://rk.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://gb.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://il.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://le.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vc.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://wa.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xd.nszjky.cn

Ruby: rand(1..100)
来源：http://xh.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://fy.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://ex.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ye.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://da.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qy.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yk.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://lf.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ka.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ri.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qt.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://ai.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zi.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qb.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://rc.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://qf.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://lu.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nu.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://ur.asd995.cn

C#:   $"Hello, {name}!"
来源：http://uo.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pg.9csxet.cn

Py:   "第一行\n第二行"
来源：http://sd.521024.cn

PHP:  "第一行\n第二行"
来源：http://fo.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://kk.nszjky.cn

TS:   "第一行\n第二行"
来源：http://zy.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://iq.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ck.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://un.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://af.hnjuh.cn

[A14] 注释写法
来源：http://la.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bn.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://do.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://eh.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://aw.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mt.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://nv.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yz.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://ez.nicolike.cn

[A15] 空值判断与默认值
来源：http://ji.521024.cn

Py:   value = data or "默认值"
来源：http://pv.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://qe.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://pi.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://gi.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yc.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://ko.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://tq.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://qq.nicolike.cn

[A16] 真假值判断规则
来源：http://ff.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wp.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ho.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xd.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://kv.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ku.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gg.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bd.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cp.bookmarksfly.cn

[A17] 位运算
来源：http://ah.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bv.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cu.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zt.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xu.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lu.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fl.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ns.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fg.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://at.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://kb.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://jq.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fe.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yr.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://up.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lv.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://al.asd995.cn

C#:   (int)'A'; (char)65
来源：http://ay.haigaiapp.cn

[A19] 交换两个变量
来源：http://yi.nszjky.cn

Py:   a, b = b, a
来源：http://mp.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sy.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://bp.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://ij.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://mi.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://lh.haigaiapp.cn

Ruby: a, b = b, a
来源：http://wp.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://pg.muxihuayi.cn

[A20] 读取标准输入
来源：http://rr.huanxung.cn

Py:   name = input("请输入：")
来源：http://az.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ae.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bb.colortex.cn

TS:   // Node.js：readline 模块
来源：http://om.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://io.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ce.jctech888.com.cn

Ruby: gets.chomp
来源：http://in.nicolike.cn

C#:   Console.ReadLine();
来源：http://so.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://wk.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://ni.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vv.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ny.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://ay.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://bj.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kt.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://zt.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://hs.huixiangedu.cn

[A22] 获取字符串长度
来源：http://eh.gzmigu.cn

Py:   len(s)
来源：http://ax.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zs.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ja.nicolike.cn

TS:   s.length
来源：http://ir.nicolike.cn

Java: s.length()
来源：http://kx.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ki.huixiangedu.cn

Ruby: s.length
来源：http://ix.jctech888.com.cn

C#:   s.Length
来源：http://gk.newstarts.cn

[A23] 大小写转换
来源：http://ji.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gw.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gf.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://og.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wl.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lg.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://po.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ou.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yz.jctech888.com.cn

[A24] 去除首尾空白
来源：http://fg.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lg.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yd.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ve.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ym.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xc.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://ap.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qj.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nt.lnxyls.cn

[A25] 字符串比较
来源：http://fa.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://ir.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wm.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sm.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uq.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kn.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ee.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rm.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mk.muxihuayi.cn

[A26] 类型转换总览
来源：http://ea.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wf.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xr.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bj.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://gh.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iq.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gw.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kn.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://it.shxzskj.cn

================================================================================
来源：http://ug.hahajie.cn

B. 流程控制
来源：http://td.haigaiapp.cn

================================================================================
来源：http://fp.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://ga.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://at.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jl.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ny.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bj.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vi.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tf.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ic.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sl.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://kq.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ot.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wp.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hd.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yq.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hk.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://br.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://le.huanxung.cn

[B03] switch / match / case
来源：http://yz.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bf.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kf.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dk.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://de.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://am.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nj.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pl.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jw.huanxung.cn

[B04] for 计数循环
来源：http://mv.521024.cn

Py:   for i in range(10): print(i)
来源：http://jn.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zp.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://md.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ck.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wc.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ma.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://kc.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qz.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://hl.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://ma.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dm.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://js.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pv.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fn.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://md.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://lb.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xq.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://iv.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://az.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gh.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qx.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uz.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uj.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lc.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bw.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://se.haigaiapp.cn

[B07] while 循环
来源：http://gx.nicolike.cn

Py:   while i < 10: i += 1
来源：http://vg.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bl.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://dd.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://hi.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://cf.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dy.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://aq.521024.cn

C#:   while (i < 10) { i++; }
来源：http://ku.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://gz.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://xs.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pr.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://np.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://vs.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://ad.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uj.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sh.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://ld.hnjuh.cn

[B09] break 与 continue
来源：http://ue.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bg.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dh.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://db.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xm.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://za.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nr.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mg.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://ow.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://va.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qc.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xt.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nr.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dw.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://en.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rs.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ro.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://dt.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://dv.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://oj.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bw.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://be.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://be.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fj.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://sx.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xn.yuexingan06.cn

[B12] 跳出多层循环
来源：http://pl.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ku.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qv.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://go.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lm.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nr.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://du.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vr.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fq.nszjky.cn

[B13] 判断是否为数字
来源：http://ph.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://gj.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://rs.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yr.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wz.colortex.cn

Java: x instanceof Number
来源：http://jj.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xv.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://tz.nicolike.cn

C#:   x is int or double or decimal
来源：http://cg.hahajie.cn

[B14] 判断值是否在集合内
来源：http://xh.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ns.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ir.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://bq.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://dg.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gn.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ng.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qb.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zo.nszjky.cn

[B15] 布尔运算与取反
来源：http://gu.huixiangedu.cn

Py:   a and b or not c
来源：http://xc.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://vv.nszjky.cn

JS:   a && b || !c
来源：http://pf.haigaiapp.cn

TS:   a && b || !c
来源：http://ko.huixiangedu.cn

Java: a && b || !c
来源：http://ll.nicolike.cn

Go:   a && b || !c
来源：http://ga.newstarts.cn

Ruby: a && b || !c
来源：http://qw.szsharing.cn

C#:   a && b || !c
来源：http://ga.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wv.lnxyls.cn

Py:   if not data: return
来源：http://vl.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://pz.shxzskj.cn

JS:   if (!data) return;
来源：http://bu.wgjwhj.cn

TS:   if (!data) return;
来源：http://xs.haigaiapp.cn


<!-- 参考信息 -->