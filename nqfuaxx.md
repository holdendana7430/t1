代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ct.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://iy.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cf.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://qr.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ws.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vv.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tt.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jw.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://md.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oa.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fz.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fv.9csxet.cn

[A10] 生成随机数
来源：http://gy.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://jw.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://wl.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nf.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rf.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ci.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sp.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://bc.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://ka.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://dw.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://co.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vc.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hv.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qf.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ui.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zf.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rj.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iw.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://gx.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://go.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vy.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://gr.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://ij.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://df.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rv.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://wr.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://ci.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ji.9csxet.cn

Py:   "第一行\n第二行"
来源：http://eg.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://xh.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://qb.newstarts.cn

TS:   "第一行\n第二行"
来源：http://uj.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://cv.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://sa.colortex.cn

Ruby: "第一行\n第二行"
来源：http://ag.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://jn.newstarts.cn

[A14] 注释写法
来源：http://rx.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hc.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zt.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://il.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://ra.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yr.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://rt.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wu.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://jv.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://qn.shxzukj.cn

Py:   value = data or "默认值"
来源：http://ia.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://dn.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://is.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://il.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cd.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://lf.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://fw.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://uv.9csxet.cn

[A16] 真假值判断规则
来源：http://rn.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://de.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zu.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://je.bookmarksfly.cn

TS:   if (!x) {}
来源：http://zm.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dp.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://up.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ev.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gb.hahajie.cn

[A17] 位运算
来源：http://rp.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uv.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uv.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vo.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vm.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ta.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://re.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rh.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sv.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://sh.asd995.cn

Py:   ord("A"); chr(65)
来源：http://yy.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://wq.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sk.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ig.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://jn.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fg.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://ht.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://na.wgjwhj.cn

[A19] 交换两个变量
来源：http://tx.bjjhwx.cn

Py:   a, b = b, a
来源：http://uh.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tt.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://vm.asd995.cn

TS:   [a, b] = [b, a];
来源：http://sl.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://tm.newstarts.cn

Go:   a, b = b, a
来源：http://yv.newstarts.cn

Ruby: a, b = b, a
来源：http://nv.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://cs.wgjwhj.cn

[A20] 读取标准输入
来源：http://na.shxzskj.cn

Py:   name = input("请输入：")
来源：http://ly.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://du.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zj.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://db.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://it.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kx.lnxyls.cn

Ruby: gets.chomp
来源：http://ot.newstarts.cn

C#:   Console.ReadLine();
来源：http://ic.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://li.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://mh.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dd.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://ya.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://xs.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://tc.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jx.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://uk.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://tt.nszjky.cn

[A22] 获取字符串长度
来源：http://ni.nszjky.cn

Py:   len(s)
来源：http://rc.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ig.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sr.szxytkj.cn

TS:   s.length
来源：http://ob.bookmarksfly.cn

Java: s.length()
来源：http://xe.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sz.yuntaijiaju.cn

Ruby: s.length
来源：http://ot.colortex.cn

C#:   s.Length
来源：http://mr.jianghongdianzi.cn

[A23] 大小写转换
来源：http://ze.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mt.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://on.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ag.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gf.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rw.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ki.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nk.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zu.haigaiapp.cn

[A24] 去除首尾空白
来源：http://ha.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cv.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ph.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cd.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jd.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://az.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://bs.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://au.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mg.muxihuayi.cn

[A25] 字符串比较
来源：http://pp.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://mq.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ez.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aj.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fv.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oa.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kn.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://le.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tv.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://qx.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fi.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wk.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jg.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://xm.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jz.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ku.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fh.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gd.bjjhwx.cn

================================================================================
来源：http://yt.jianghongdianzi.cn

B. 流程控制
来源：http://ve.huanxung.cn

================================================================================
来源：http://dz.gzmigu.cn

[B01] 条件判断 if / else
来源：http://tj.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pn.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fl.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ny.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tj.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xu.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wg.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ap.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xs.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://bk.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://os.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fv.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cj.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tz.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gc.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mp.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://do.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.asd995.cn

[B03] switch / match / case
来源：http://wt.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://al.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vg.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vb.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sy.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pl.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://be.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jh.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wj.shxzskj.cn

[B04] for 计数循环
来源：http://su.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://sq.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tr.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nk.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fe.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://io.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ua.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://lp.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ys.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://sv.9csxet.cn

Py:   for item in arr: print(item)
来源：http://ha.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oa.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ve.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ub.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hc.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wt.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://ry.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ok.colortex.cn

[B06] 遍历字典 / 对象
来源：http://mi.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oy.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zy.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ls.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oi.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gk.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fj.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://du.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://th.hnjuh.cn

[B07] while 循环
来源：http://iw.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://td.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bg.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://ix.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://zd.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://ox.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rq.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://bl.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://yc.asd995.cn

[B08] do-while（至少执行一次）
来源：http://rb.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ge.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ix.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://go.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://xy.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://vn.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uc.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://or.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://hc.yuexingan06.cn

[B09] break 与 continue
来源：http://rq.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vl.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sg.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ob.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zu.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uk.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gj.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fr.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ew.521024.cn

[B10] 遍历同时拿索引
来源：http://te.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rn.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uq.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uq.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kg.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aw.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sy.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ap.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zj.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://dz.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://py.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://de.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gx.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nk.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cl.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wp.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://vd.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nx.colortex.cn

[B12] 跳出多层循环
来源：http://nk.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nr.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bc.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zr.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zv.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ro.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sm.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jx.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mt.colortex.cn

[B13] 判断是否为数字
来源：http://vy.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://on.gzmigu.cn

PHP:  is_numeric($x)
来源：http://ab.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ms.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wv.gzmigu.cn

Java: x instanceof Number
来源：http://wn.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vx.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://fs.9csxet.cn

C#:   x is int or double or decimal
来源：http://pi.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://ot.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gv.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sd.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ad.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://vi.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kz.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ha.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nz.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rx.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://rc.yuntaijiaju.cn

Py:   a and b or not c
来源：http://ls.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://oz.huanxung.cn

JS:   a && b || !c
来源：http://ye.bookmarksfly.cn

TS:   a && b || !c
来源：http://zx.yuexingan06.cn

Java: a && b || !c
来源：http://qk.lnxyls.cn


<!-- 参考信息 -->