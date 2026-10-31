代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ft.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qe.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qv.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://xd.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vp.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rf.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uq.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ma.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ly.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ut.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vq.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rm.wgjwhj.cn

[A10] 生成随机数
来源：http://lf.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://dx.521024.cn

PHP:  random_int(1, 100);
来源：http://pw.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ov.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aw.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://qn.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rh.newstarts.cn

Ruby: rand(1..100)
来源：http://lr.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://sy.521024.cn

[A11] 条件表达式（三元）
来源：http://gs.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://xf.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zs.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://su.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jz.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://di.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dd.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gy.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pp.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://bn.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ut.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bw.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://tf.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://av.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://zy.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ox.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://po.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://ym.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fm.521024.cn

Py:   "第一行\n第二行"
来源：http://ae.colortex.cn

PHP:  "第一行\n第二行"
来源：http://zm.nszjky.cn

JS:   "第一行\n第二行"
来源：http://ig.huanxung.cn

TS:   "第一行\n第二行"
来源：http://lj.nszjky.cn

Java: "第一行\n第二行"
来源：http://fs.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://rx.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://lp.asd995.cn

C#:   "第一行\n第二行"
来源：http://sp.9csxet.cn

[A14] 注释写法
来源：http://to.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gh.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sd.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://kw.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://cv.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vg.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://uj.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dv.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://li.szsharing.cn

[A15] 空值判断与默认值
来源：http://ov.huanxung.cn

Py:   value = data or "默认值"
来源：http://cw.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://ct.521024.cn

JS:   const value = data ?? "默认值";
来源：http://oa.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://tm.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vt.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://nx.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://lw.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://el.nszjky.cn

[A16] 真假值判断规则
来源：http://uu.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://je.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://up.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jv.newstarts.cn

TS:   if (!x) {}
来源：http://re.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xn.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ya.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dp.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fw.panjiajie.cn

[A17] 位运算
来源：http://en.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rx.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yp.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zu.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kn.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ow.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fl.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xm.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lt.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://ah.521024.cn

Py:   ord("A"); chr(65)
来源：http://kr.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://zf.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ma.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hb.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://pb.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://my.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://nh.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://or.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://mw.nicolike.cn

Py:   a, b = b, a
来源：http://fi.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qg.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://od.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://ov.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://go.bookmarksfly.cn

Go:   a, b = b, a
来源：http://nw.szsharing.cn

Ruby: a, b = b, a
来源：http://op.521024.cn

C#:   (a, b) = (b, a);
来源：http://jn.lnxyls.cn

[A20] 读取标准输入
来源：http://vn.asd995.cn

Py:   name = input("请输入：")
来源：http://ti.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rt.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eq.colortex.cn

TS:   // Node.js：readline 模块
来源：http://hs.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://js.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dz.shxzukj.cn

Ruby: gets.chomp
来源：http://mn.9csxet.cn

C#:   Console.ReadLine();
来源：http://ao.huanxung.cn

[A21] 保留指定小数位输出
来源：http://pg.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://bz.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ph.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://ei.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://oq.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://la.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://us.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://ra.521024.cn

C#:   3.14159.ToString("F2")
来源：http://gg.szxytkj.cn

[A22] 获取字符串长度
来源：http://hj.bookmarksfly.cn

Py:   len(s)
来源：http://cf.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mf.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ki.huixinmuqiang.cn

TS:   s.length
来源：http://wt.jctech888.com.cn

Java: s.length()
来源：http://cs.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://it.wgjwhj.cn

Ruby: s.length
来源：http://sd.shxzukj.cn

C#:   s.Length
来源：http://no.nicolike.cn

[A23] 大小写转换
来源：http://xp.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ik.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nb.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mb.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lx.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://np.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zo.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ty.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yu.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://jz.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nn.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wj.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dv.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mz.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cb.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://ld.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bq.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ni.jianghongdianzi.cn

[A25] 字符串比较
来源：http://bg.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://be.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fw.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://un.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://la.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ic.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gh.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xx.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://du.gzmigu.cn

[A26] 类型转换总览
来源：http://zv.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zt.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lr.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bv.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://ep.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fs.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ms.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lv.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://id.yuntaijiaju.cn

================================================================================
来源：http://zh.shxzskj.cn

B. 流程控制
来源：http://tj.nicolike.cn

================================================================================
来源：http://kg.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://er.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lx.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yr.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mt.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eu.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oc.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ls.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hm.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qu.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://kq.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gq.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wb.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yi.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zu.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vs.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ah.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iu.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pq.yuntaijiaju.cn

[B03] switch / match / case
来源：http://zi.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://df.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wc.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sq.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dt.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ul.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hb.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xl.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vd.hahajie.cn

[B04] for 计数循环
来源：http://hx.colortex.cn

Py:   for i in range(10): print(i)
来源：http://ap.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ts.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vx.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://co.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xc.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://ns.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jr.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://cp.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://ui.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wq.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cy.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gh.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wq.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sw.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://di.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://km.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://tk.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dl.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vj.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lr.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kx.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tf.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pr.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iv.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zq.jianghongdianzi.cn

[B07] while 循环
来源：http://qp.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://vo.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ev.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://if.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ce.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://cb.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dl.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://ye.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://aw.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://sb.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://vh.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qz.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://om.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://xn.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://pj.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://of.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ke.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://gl.huixinmuqiang.cn

[B09] break 与 continue
来源：http://ow.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cp.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mn.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bp.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bs.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wl.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dg.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iq.asd995.cn

[B10] 遍历同时拿索引
来源：http://io.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ns.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lj.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ty.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://at.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lx.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tj.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ac.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rf.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://od.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://ec.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://ys.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kr.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ff.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nq.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eg.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://xj.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ia.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://tu.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yc.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vi.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bl.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sd.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kc.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jq.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ln.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dg.9csxet.cn

[B13] 判断是否为数字
来源：http://tk.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://dg.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://jg.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qp.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gk.bjjhwx.cn

Java: x instanceof Number
来源：http://bd.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yw.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://iu.521024.cn

C#:   x is int or double or decimal
来源：http://ag.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://ch.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mc.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rv.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://qn.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://oz.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kq.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eu.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pe.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gf.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://fd.yuexingan06.cn

Py:   a and b or not c
来源：http://ws.nszjky.cn

PHP:  $a && $b || !$c
来源：http://gd.nszjky.cn

JS:   a && b || !c
来源：http://yk.szsharing.cn

TS:   a && b || !c
来源：http://nz.hahajie.cn

Java: a && b || !c
来源：http://sz.huixinmuqiang.cn


<!-- 参考信息 -->