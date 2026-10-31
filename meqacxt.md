代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sj.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yy.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://on.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cw.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fd.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vx.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fx.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nk.hahajie.cn

[A10] 生成随机数
来源：http://ry.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://tl.nicolike.cn

PHP:  random_int(1, 100);
来源：http://cc.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tf.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sf.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://yr.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yr.bjjhwx.cn

Ruby: rand(1..100)
来源：http://ym.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://yr.nicolike.cn

[A11] 条件表达式（三元）
来源：http://ty.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://qq.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ki.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rg.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://is.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://uz.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ew.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://as.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zk.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://bn.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zf.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dy.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://ym.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://ho.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://qy.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nm.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://va.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://yn.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ct.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://gg.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://ks.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://we.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://tk.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://fl.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://ry.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://nn.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://xb.shxzukj.cn

[A14] 注释写法
来源：http://gs.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nn.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jr.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://wc.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://oy.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dt.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://mf.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lt.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://pd.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://om.szsharing.cn

Py:   value = data or "默认值"
来源：http://ds.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://nw.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://eh.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://lu.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wa.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://fl.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://vt.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://kv.chemitech.net.cn

[A16] 真假值判断规则
来源：http://mr.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fm.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://an.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gw.shxzskj.cn

TS:   if (!x) {}
来源：http://wf.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qh.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ax.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cf.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bz.bookmarksfly.cn

[A17] 位运算
来源：http://dt.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jc.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xl.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rz.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vf.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ba.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vt.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jq.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sg.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://tc.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://qe.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://up.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wi.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://od.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://mz.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mu.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://pi.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://xx.szsharing.cn

[A19] 交换两个变量
来源：http://tu.gzmigu.cn

Py:   a, b = b, a
来源：http://jz.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bd.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://ek.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://za.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://zw.nicolike.cn

Go:   a, b = b, a
来源：http://gf.huixiangedu.cn

Ruby: a, b = b, a
来源：http://ca.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://mc.wgjwhj.cn

[A20] 读取标准输入
来源：http://jb.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://qy.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dl.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://md.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://rr.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://vb.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mt.bookmarksfly.cn

Ruby: gets.chomp
来源：http://fw.colortex.cn

C#:   Console.ReadLine();
来源：http://rv.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://iq.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://nh.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://or.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://wg.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://dr.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://kk.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://il.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ck.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://xr.hahajie.cn

[A22] 获取字符串长度
来源：http://uy.bjjhwx.cn

Py:   len(s)
来源：http://lx.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pv.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uz.szsharing.cn

TS:   s.length
来源：http://lp.shxzukj.cn

Java: s.length()
来源：http://ha.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jy.haigaiapp.cn

Ruby: s.length
来源：http://xz.huanxung.cn

C#:   s.Length
来源：http://pr.shxzskj.cn

[A23] 大小写转换
来源：http://my.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ye.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cv.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gr.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fl.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yp.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yr.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cm.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hi.shtwfgs.cn

[A24] 去除首尾空白
来源：http://rr.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uo.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wc.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ye.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uu.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ao.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://eu.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lf.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://by.panjiajie.cn

[A25] 字符串比较
来源：http://qs.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://rt.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://io.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iy.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hm.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ha.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ky.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tk.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vj.lnxyls.cn

[A26] 类型转换总览
来源：http://lh.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ad.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lw.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ob.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://ud.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mb.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ab.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://du.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xb.521024.cn

================================================================================
来源：http://kv.lnxyls.cn

B. 流程控制
来源：http://cs.colortex.cn

================================================================================
来源：http://ba.szxytkj.cn

[B01] 条件判断 if / else
来源：http://ag.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zq.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kj.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jb.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://we.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yi.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rl.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yc.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rf.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://dm.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tj.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ru.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://me.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qj.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pc.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mu.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rr.szsharing.cn

[B03] switch / match / case
来源：http://gg.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ty.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fi.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qt.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tg.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oh.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ye.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bl.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rx.lnxyls.cn

[B04] for 计数循环
来源：http://ta.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://ar.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tw.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nl.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oj.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hb.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kb.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://za.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ct.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://ov.nicolike.cn

Py:   for item in arr: print(item)
来源：http://wp.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aa.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hj.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wz.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bl.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hd.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://hl.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://om.521024.cn

[B06] 遍历字典 / 对象
来源：http://dt.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xs.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bm.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zm.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ez.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kr.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nk.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gv.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cr.shtwfgs.cn

[B07] while 循环
来源：http://ev.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://qw.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lu.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://vy.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://lj.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://gw.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jk.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://ox.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://qj.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://xa.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://vt.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sm.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://ab.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://jh.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://jt.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bi.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mw.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://gy.shxzukj.cn

[B09] break 与 continue
来源：http://iu.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://df.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cb.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dy.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ep.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iq.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gx.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cl.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.newstarts.cn

[B10] 遍历同时拿索引
来源：http://yn.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rj.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://et.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wa.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xp.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ge.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ag.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lw.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tk.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://ra.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://zm.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://ni.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pn.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pv.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://md.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jk.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://fm.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xn.muxihuayi.cn

[B12] 跳出多层循环
来源：http://op.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sn.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wy.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tz.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vz.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://of.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dm.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mg.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pj.hahajie.cn

[B13] 判断是否为数字
来源：http://sz.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://wo.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://lr.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qd.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pz.newstarts.cn

Java: x instanceof Number
来源：http://bn.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://su.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://xv.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://xt.hahajie.cn

[B14] 判断值是否在集合内
来源：http://rr.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ml.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xs.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://ev.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://pk.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vv.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ld.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yx.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ny.asd995.cn

[B15] 布尔运算与取反
来源：http://id.bjjhwx.cn

Py:   a and b or not c
来源：http://am.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://cc.jctech888.com.cn

JS:   a && b || !c
来源：http://gx.colortex.cn

TS:   a && b || !c
来源：http://tp.asd995.cn

Java: a && b || !c
来源：http://gm.muxihuayi.cn

Go:   a && b || !c
来源：http://hn.szxytkj.cn

Ruby: a && b || !c
来源：http://he.panjiajie.cn

C#:   a && b || !c
来源：http://bv.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gg.szxytkj.cn


<!-- 参考信息 -->