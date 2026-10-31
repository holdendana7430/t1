代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ez.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wu.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fr.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://kz.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vh.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mj.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sj.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://on.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rx.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tr.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ot.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xx.colortex.cn

[A10] 生成随机数
来源：http://no.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://cv.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://sf.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mv.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yx.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://wo.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://te.hnjuh.cn

Ruby: rand(1..100)
来源：http://vw.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://wy.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://kc.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://er.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wt.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jj.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ux.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://er.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hx.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rc.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cv.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://ma.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cz.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jh.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://qy.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://lj.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://sn.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kb.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://hs.colortex.cn

C#:   $"Hello, {name}!"
来源：http://em.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sh.huanxung.cn

Py:   "第一行\n第二行"
来源：http://bj.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://on.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://dz.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://qp.szsharing.cn

Java: "第一行\n第二行"
来源：http://lj.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://iz.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://gb.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://sj.colortex.cn

[A14] 注释写法
来源：http://dt.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pc.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ld.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://jk.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://uc.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hu.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://li.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sa.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://iz.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://vv.hahajie.cn

Py:   value = data or "默认值"
来源：http://fz.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://cq.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://qc.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://bx.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ll.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://kl.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://yg.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://pc.nszjky.cn

[A16] 真假值判断规则
来源：http://ef.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ai.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sl.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kx.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://qg.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ar.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vd.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vp.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sh.nszjky.cn

[A17] 位运算
来源：http://ms.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eb.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zh.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hs.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://au.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yo.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rm.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ow.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://px.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://iq.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://aj.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rr.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xs.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://ro.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mn.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://bm.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://bw.muxihuayi.cn

[A19] 交换两个变量
来源：http://fb.colortex.cn

Py:   a, b = b, a
来源：http://bg.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://we.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://pc.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://op.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://nt.newstarts.cn

Go:   a, b = b, a
来源：http://bl.szxytkj.cn

Ruby: a, b = b, a
来源：http://bu.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://je.lnxyls.cn

[A20] 读取标准输入
来源：http://oz.shxzukj.cn

Py:   name = input("请输入：")
来源：http://ld.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xf.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lj.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://qq.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://qm.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fz.szsharing.cn

Ruby: gets.chomp
来源：http://an.nicolike.cn

C#:   Console.ReadLine();
来源：http://dg.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://id.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://vd.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jr.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://gg.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://vp.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://vj.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jf.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://rk.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://bs.shxzukj.cn

[A22] 获取字符串长度
来源：http://yq.yuntaijiaju.cn

Py:   len(s)
来源：http://mq.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yj.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ss.bookmarksfly.cn

TS:   s.length
来源：http://jx.gzmigu.cn

Java: s.length()
来源：http://hf.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lj.nszjky.cn

Ruby: s.length
来源：http://or.huanxung.cn

C#:   s.Length
来源：http://cr.chemitech.net.cn

[A23] 大小写转换
来源：http://ev.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uy.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kr.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ra.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://no.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ro.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hy.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ei.yuexingan06.cn

[A24] 去除首尾空白
来源：http://rd.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ym.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gn.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rb.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qj.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qr.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://lx.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mo.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yn.haigaiapp.cn

[A25] 字符串比较
来源：http://es.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://zj.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xw.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://am.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xu.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qp.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xz.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tu.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ce.muxihuayi.cn

[A26] 类型转换总览
来源：http://tk.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fh.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pv.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hk.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://dt.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hi.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zu.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sw.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jv.jctech888.com.cn

================================================================================
来源：http://md.huixiangedu.cn

B. 流程控制
来源：http://wg.newstarts.cn

================================================================================
来源：http://xz.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://pa.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vn.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sf.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tc.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fp.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ye.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cv.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cs.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dy.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://zo.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pg.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wg.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mo.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dl.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xu.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ic.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zo.gzmigu.cn

[B03] switch / match / case
来源：http://vr.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://po.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fw.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oy.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yk.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sr.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uw.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zw.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vr.jianghongdianzi.cn

[B04] for 计数循环
来源：http://ae.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://po.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yb.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ky.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cb.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jv.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ym.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://rt.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://px.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://hl.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://mf.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ru.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oa.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qj.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aj.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jb.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://wi.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://db.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://uy.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://id.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mh.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yq.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ip.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nc.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wa.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yl.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fz.shxzukj.cn

[B07] while 循环
来源：http://fn.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://uq.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fo.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://ho.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://za.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://br.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dc.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://yc.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://hd.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://hp.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://fm.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wg.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://nx.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://je.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://xe.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zb.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qq.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://gb.hahajie.cn

[B09] break 与 continue
来源：http://ya.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qk.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vb.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vv.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yy.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jc.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rr.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xi.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://al.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://hv.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xd.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pz.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hq.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zf.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mw.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gm.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ba.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fo.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://ez.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://wq.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://kn.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pd.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hp.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zt.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ko.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://iw.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ay.shtwfgs.cn

[B12] 跳出多层循环
来源：http://rk.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zb.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://js.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ps.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kq.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bu.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://td.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zg.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fw.shtwfgs.cn

[B13] 判断是否为数字
来源：http://zi.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://cm.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://lv.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://am.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yb.9csxet.cn

Java: x instanceof Number
来源：http://in.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xp.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://yw.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://mu.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://vk.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sl.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fd.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://uf.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://hk.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ye.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ke.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tx.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ws.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://gb.hnjuh.cn

Py:   a and b or not c
来源：http://bc.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://tq.szsharing.cn

JS:   a && b || !c
来源：http://gd.colortex.cn

TS:   a && b || !c
来源：http://bi.panjiajie.cn

Java: a && b || !c
来源：http://fs.shtwfgs.cn


<!-- 参考信息 -->