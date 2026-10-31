代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yx.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ag.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wj.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://cq.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ov.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pq.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kf.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xp.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rz.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lo.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://um.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zr.bjjhwx.cn

[A10] 生成随机数
来源：http://dx.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://te.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://im.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rt.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oy.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://dw.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ot.huixiangedu.cn

Ruby: rand(1..100)
来源：http://si.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://gi.521024.cn

[A11] 条件表达式（三元）
来源：http://ha.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://wv.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xf.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gx.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ep.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://tv.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oo.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://te.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nn.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://fn.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oo.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yw.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://pj.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://fh.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://le.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mn.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://jy.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://wp.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ma.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://zj.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://bm.szsharing.cn

JS:   "第一行\n第二行"
来源：http://cc.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://kn.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://it.asd995.cn

Go:   "第一行\n第二行"
来源：http://lg.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://ii.colortex.cn

C#:   "第一行\n第二行"
来源：http://gk.nszjky.cn

[A14] 注释写法
来源：http://dr.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pt.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rn.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://jb.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://yn.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sx.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://rh.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://or.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://xg.newstarts.cn

[A15] 空值判断与默认值
来源：http://ap.shxzukj.cn

Py:   value = data or "默认值"
来源：http://lz.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://nh.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://si.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://yd.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xq.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://ma.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://dj.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://ei.muxihuayi.cn

[A16] 真假值判断规则
来源：http://zh.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://at.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sf.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lf.szxytkj.cn

TS:   if (!x) {}
来源：http://zx.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hb.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gx.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://on.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jc.huanxung.cn

[A17] 位运算
来源：http://lr.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ht.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sy.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ra.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ki.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gv.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jn.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bh.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mg.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://xv.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://jw.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://ze.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pf.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rw.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://lq.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pk.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://tv.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://xl.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://xw.shxzukj.cn

Py:   a, b = b, a
来源：http://uu.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bu.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://dr.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://lm.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://bo.hnjuh.cn

Go:   a, b = b, a
来源：http://qc.huixiangedu.cn

Ruby: a, b = b, a
来源：http://ag.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://ep.wgjwhj.cn

[A20] 读取标准输入
来源：http://at.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://qa.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rz.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vb.colortex.cn

TS:   // Node.js：readline 模块
来源：http://kf.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://fw.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ra.yuexingan06.cn

Ruby: gets.chomp
来源：http://sf.9csxet.cn

C#:   Console.ReadLine();
来源：http://jb.huanxung.cn

[A21] 保留指定小数位输出
来源：http://dp.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://rn.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dr.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://ub.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://dr.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ju.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wb.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://ur.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://ch.szxytkj.cn

[A22] 获取字符串长度
来源：http://fy.wgjwhj.cn

Py:   len(s)
来源：http://vv.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nv.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vt.chemitech.net.cn

TS:   s.length
来源：http://xl.newstarts.cn

Java: s.length()
来源：http://gm.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://je.colortex.cn

Ruby: s.length
来源：http://yu.huixinmuqiang.cn

C#:   s.Length
来源：http://em.shxzukj.cn

[A23] 大小写转换
来源：http://bu.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tz.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ms.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ym.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yo.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hr.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iq.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://go.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kr.hahajie.cn

[A24] 去除首尾空白
来源：http://tk.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hu.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ig.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ae.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ix.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yo.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://yg.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wr.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lq.muxihuayi.cn

[A25] 字符串比较
来源：http://vv.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://vr.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pn.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ak.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wb.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://de.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ws.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ym.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ic.asd995.cn

[A26] 类型转换总览
来源：http://ww.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aq.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tn.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rt.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://bh.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://it.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ky.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ft.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oe.bjjhwx.cn

================================================================================
来源：http://ji.521024.cn

B. 流程控制
来源：http://lx.huanxung.cn

================================================================================
来源：http://dx.nicolike.cn

[B01] 条件判断 if / else
来源：http://id.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uq.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ev.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pe.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tw.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ne.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://el.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uw.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qo.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://go.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xu.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tt.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://id.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wu.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yw.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ze.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bu.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fy.szxytkj.cn

[B03] switch / match / case
来源：http://pk.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ow.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gu.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yu.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sl.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rl.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ld.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ph.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vh.newstarts.cn

[B04] for 计数循环
来源：http://wx.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://hy.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aa.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dp.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tk.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sy.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fn.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://bt.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ux.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://br.nszjky.cn

Py:   for item in arr: print(item)
来源：http://pe.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fu.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bt.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qx.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wv.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wr.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://tv.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tm.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://lp.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dw.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bc.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ao.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pq.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://un.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://no.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fu.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gl.gzmigu.cn

[B07] while 循环
来源：http://zm.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://sn.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lc.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://yy.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://pu.colortex.cn

Java: while (i < 10) { i++; }
来源：http://do.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kb.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://gq.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://ey.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://su.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://wu.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tm.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://ax.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://ll.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://ay.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xe.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ew.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://kj.shxzukj.cn

[B09] break 与 continue
来源：http://ey.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jq.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sv.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sq.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bf.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ha.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://un.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kx.szsharing.cn

[B10] 遍历同时拿索引
来源：http://sm.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lu.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yb.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qi.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ug.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ov.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://el.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://on.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://um.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://wq.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://pd.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://ia.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ku.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cr.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ti.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ts.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://oh.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ox.nicolike.cn

[B12] 跳出多层循环
来源：http://xn.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pr.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mz.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ok.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dg.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ux.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nn.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gg.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yc.huanxung.cn

[B13] 判断是否为数字
来源：http://ys.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://wk.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://ow.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dq.huanxung.cn

Java: x instanceof Number
来源：http://aq.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rr.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://kz.panjiajie.cn

C#:   x is int or double or decimal
来源：http://ac.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://pi.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wk.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fr.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://nm.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://lx.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dl.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ni.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sm.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://la.shxzskj.cn

[B15] 布尔运算与取反
来源：http://ma.nszjky.cn

Py:   a and b or not c
来源：http://ww.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://hr.colortex.cn

JS:   a && b || !c
来源：http://vc.asd995.cn

TS:   a && b || !c
来源：http://wn.szxytkj.cn

Java: a && b || !c
来源：http://lx.chemitech.net.cn


<!-- 参考信息 -->