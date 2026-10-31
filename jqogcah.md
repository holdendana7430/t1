代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sx.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pb.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ec.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vr.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hw.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nb.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jf.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mj.chemitech.net.cn

[A10] 生成随机数
来源：http://kr.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://oh.colortex.cn

PHP:  random_int(1, 100);
来源：http://mw.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oa.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kc.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://wz.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zl.szsharing.cn

Ruby: rand(1..100)
来源：http://xp.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://pv.newstarts.cn

[A11] 条件表达式（三元）
来源：http://mx.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://sn.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dz.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vz.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vq.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://cx.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ma.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fm.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lt.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://kn.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xe.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nv.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://xw.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://pm.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://tc.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ns.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://oo.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://ae.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ji.asd995.cn

Py:   "第一行\n第二行"
来源：http://tp.colortex.cn

PHP:  "第一行\n第二行"
来源：http://dt.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://cn.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://aj.panjiajie.cn

Java: "第一行\n第二行"
来源：http://vu.9csxet.cn

Go:   "第一行\n第二行"
来源：http://wj.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://lj.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://ax.yuexingan06.cn

[A14] 注释写法
来源：http://mv.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rq.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bk.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://qh.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://bi.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tr.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://gs.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hd.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://ie.9csxet.cn

[A15] 空值判断与默认值
来源：http://ql.nszjky.cn

Py:   value = data or "默认值"
来源：http://na.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://qv.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://ii.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://ek.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://or.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://ec.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://za.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://dy.chemitech.net.cn

[A16] 真假值判断规则
来源：http://eb.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yt.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ar.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uo.newstarts.cn

TS:   if (!x) {}
来源：http://te.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mk.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yi.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kw.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cv.yuexingan06.cn

[A17] 位运算
来源：http://yd.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hy.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wz.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ei.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://np.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yq.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oj.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yv.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vj.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://oo.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://rw.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://uc.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zl.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gi.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://fe.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sk.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://uz.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://dv.nszjky.cn

[A19] 交换两个变量
来源：http://uk.szxytkj.cn

Py:   a, b = b, a
来源：http://za.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gn.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://xs.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://nc.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://gr.nicolike.cn

Go:   a, b = b, a
来源：http://sg.hahajie.cn

Ruby: a, b = b, a
来源：http://iy.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://di.yuexingan06.cn

[A20] 读取标准输入
来源：http://bq.szxytkj.cn

Py:   name = input("请输入：")
来源：http://ox.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oy.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://du.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://oj.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://mp.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mi.colortex.cn

Ruby: gets.chomp
来源：http://bs.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://ez.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://zd.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://bw.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://go.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://mb.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://fn.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://ix.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zt.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://pg.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://ds.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://mk.jianghongdianzi.cn

Py:   len(s)
来源：http://va.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uj.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://de.muxihuayi.cn

TS:   s.length
来源：http://gu.jianghongdianzi.cn

Java: s.length()
来源：http://qu.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mn.nicolike.cn

Ruby: s.length
来源：http://ud.haigaiapp.cn

C#:   s.Length
来源：http://jj.shxzukj.cn

[A23] 大小写转换
来源：http://lc.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uc.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qq.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qh.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cb.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mb.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mj.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mj.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ho.gzmigu.cn

[A24] 去除首尾空白
来源：http://jy.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kj.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ii.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rp.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gx.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://we.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://bh.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nn.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://in.nszjky.cn

[A25] 字符串比较
来源：http://qm.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://ym.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ax.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nc.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qq.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pe.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kj.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bi.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yh.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://sb.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vq.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gn.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ut.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://zo.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eb.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gp.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nd.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ec.haigaiapp.cn

================================================================================
来源：http://qy.521024.cn

B. 流程控制
来源：http://yf.newstarts.cn

================================================================================
来源：http://aj.asd995.cn

[B01] 条件判断 if / else
来源：http://dx.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sl.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ap.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yi.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ac.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://np.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kz.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pc.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rb.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://mi.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ye.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qj.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ia.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zp.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://md.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://he.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mj.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fo.521024.cn

[B03] switch / match / case
来源：http://em.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fz.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hs.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mn.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gu.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xc.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eb.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sc.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kv.yuexingan06.cn

[B04] for 计数循环
来源：http://nh.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://au.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xa.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rt.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xq.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gq.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ca.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://vz.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lr.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://ap.nicolike.cn

Py:   for item in arr: print(item)
来源：http://un.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mt.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vs.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ko.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://td.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qq.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://pc.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nu.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://uc.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dx.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ss.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lc.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nh.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://km.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ai.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ud.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ku.asd995.cn

[B07] while 循环
来源：http://uu.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://ir.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qi.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://bi.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://se.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://vw.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fm.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://zg.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://rt.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://nl.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ar.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ev.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://yp.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://hp.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://bw.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wh.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xv.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://hl.colortex.cn

[B09] break 与 continue
来源：http://nz.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kb.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mk.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ug.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fe.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ga.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sh.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yc.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://bg.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cx.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cq.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zi.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lq.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aw.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vi.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lv.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lw.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://bz.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://pr.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://qk.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://on.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lh.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://as.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zu.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://sb.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://no.muxihuayi.cn

[B12] 跳出多层循环
来源：http://bf.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ef.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ii.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xu.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://io.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nz.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hy.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ak.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://re.hnjuh.cn

[B13] 判断是否为数字
来源：http://mj.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://sn.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://uq.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fg.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://db.hnjuh.cn

Java: x instanceof Number
来源：http://of.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ul.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://se.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://gd.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://ni.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fp.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zk.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://cs.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://vy.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pu.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rs.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://st.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pq.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://ta.lnxyls.cn

Py:   a and b or not c
来源：http://vq.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://im.szxytkj.cn

JS:   a && b || !c
来源：http://ex.szxytkj.cn

TS:   a && b || !c
来源：http://dq.bookmarksfly.cn

Java: a && b || !c
来源：http://ny.huixinmuqiang.cn

Go:   a && b || !c
来源：http://el.lnxyls.cn

Ruby: a && b || !c
来源：http://rr.bookmarksfly.cn

C#:   a && b || !c
来源：http://ep.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ke.bjjhwx.cn


<!-- 参考信息 -->