代发 wailian999

Ruby: 42.to_s
来源：http://db.9csxet.cn

C#:   42.ToString()
来源：http://zq.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://vz.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dw.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cc.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sk.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xg.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yx.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qs.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://in.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nj.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://pb.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://br.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fz.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://td.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aj.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oz.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://md.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sn.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kt.huixiangedu.cn

[A10] 生成随机数
来源：http://xt.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://qv.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://zs.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bo.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ex.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://vf.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sc.hahajie.cn

Ruby: rand(1..100)
来源：http://xc.521024.cn

C#:   new Random().Next(1, 101)
来源：http://fk.521024.cn

[A11] 条件表达式（三元）
来源：http://hz.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://uh.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://my.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sq.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://av.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://zx.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ze.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bx.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qr.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://pc.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lq.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oc.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://wu.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://qa.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://ai.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mz.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://ih.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://qu.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fb.asd995.cn

Py:   "第一行\n第二行"
来源：http://ju.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://uz.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://sn.szsharing.cn

TS:   "第一行\n第二行"
来源：http://md.newstarts.cn

Java: "第一行\n第二行"
来源：http://mu.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://wl.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://ab.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://mj.colortex.cn

[A14] 注释写法
来源：http://xv.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dn.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ia.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://as.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://gb.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ch.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://lg.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://is.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://wd.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://ot.shxzskj.cn

Py:   value = data or "默认值"
来源：http://sm.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ru.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://yn.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://op.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pz.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://yv.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://ij.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://vl.muxihuayi.cn

[A16] 真假值判断规则
来源：http://eo.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ys.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sa.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ub.bookmarksfly.cn

TS:   if (!x) {}
来源：http://ts.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://re.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jp.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://we.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bm.asd995.cn

[A17] 位运算
来源：http://gu.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jj.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ns.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ji.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aj.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oc.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mv.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ok.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aj.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://zl.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://eq.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://el.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nw.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ot.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://ol.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pi.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://bt.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://be.hnjuh.cn

[A19] 交换两个变量
来源：http://xp.bjjhwx.cn

Py:   a, b = b, a
来源：http://wi.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zr.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://ej.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://sv.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://oi.huixiangedu.cn

Go:   a, b = b, a
来源：http://hu.nicolike.cn

Ruby: a, b = b, a
来源：http://bu.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://xf.gzmigu.cn

[A20] 读取标准输入
来源：http://zc.9csxet.cn

Py:   name = input("请输入：")
来源：http://cx.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wn.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cv.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://ep.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://ig.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://np.shtwfgs.cn

Ruby: gets.chomp
来源：http://uj.gzmigu.cn

C#:   Console.ReadLine();
来源：http://jf.szsharing.cn

[A21] 保留指定小数位输出
来源：http://bi.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://pg.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gy.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://ik.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://fk.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://af.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://js.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://if.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://xe.gzmigu.cn

[A22] 获取字符串长度
来源：http://ek.521024.cn

Py:   len(s)
来源：http://xe.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xm.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ih.shxzskj.cn

TS:   s.length
来源：http://ak.shxzskj.cn

Java: s.length()
来源：http://cb.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nf.nszjky.cn

Ruby: s.length
来源：http://eu.lnxyls.cn

C#:   s.Length
来源：http://sa.muxihuayi.cn

[A23] 大小写转换
来源：http://ln.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yw.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ta.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jv.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fd.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://to.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xt.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ly.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ib.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://bc.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://du.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hn.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://si.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hr.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lr.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://ph.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zz.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nv.lnxyls.cn

[A25] 字符串比较
来源：http://bm.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://sk.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ny.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jn.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cb.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dw.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zx.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lc.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hi.hahajie.cn

[A26] 类型转换总览
来源：http://om.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vp.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mi.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zh.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://iv.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yk.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fc.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qh.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ho.shxzukj.cn

================================================================================
来源：http://pd.hahajie.cn

B. 流程控制
来源：http://ts.shtwfgs.cn

================================================================================
来源：http://pd.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://ku.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ee.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vv.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hy.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ni.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://au.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rs.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bu.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://go.hahajie.cn

[B02] 多分支 else if / elif
来源：http://do.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mh.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oa.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bu.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tp.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jg.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tm.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oa.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.szxytkj.cn

[B03] switch / match / case
来源：http://aq.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rt.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yv.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jj.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bv.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vw.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ov.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pl.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://om.szxytkj.cn

[B04] for 计数循环
来源：http://ux.colortex.cn

Py:   for i in range(10): print(i)
来源：http://bc.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ok.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ob.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bf.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xo.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bt.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://wq.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zi.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://ut.521024.cn

Py:   for item in arr: print(item)
来源：http://hn.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eb.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ex.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ue.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qi.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hp.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://wj.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ix.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://ja.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oa.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://su.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lx.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ao.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://du.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vz.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eo.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tu.asd995.cn

[B07] while 循环
来源：http://az.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://mx.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xj.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://fh.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://yv.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://yb.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mq.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://mn.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://cj.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://xx.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://nb.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nk.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://dr.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://iu.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://bv.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bi.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ow.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://yc.shxzskj.cn

[B09] break 与 continue
来源：http://oh.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oa.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mm.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qp.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sb.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vw.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jx.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ne.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.nicolike.cn

[B10] 遍历同时拿索引
来源：http://dj.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ft.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ce.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://np.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rj.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qa.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lo.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://me.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://te.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://wq.521024.cn

Py:   list(range(0, 10, 2))
来源：http://iq.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://hw.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kp.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ow.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sx.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ma.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://rj.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://si.panjiajie.cn

[B12] 跳出多层循环
来源：http://fw.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xb.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qa.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://am.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uq.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uj.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cj.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bl.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lh.wgjwhj.cn

[B13] 判断是否为数字
来源：http://og.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://xf.szsharing.cn

PHP:  is_numeric($x)
来源：http://yp.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://np.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://my.hahajie.cn

Java: x instanceof Number
来源：http://mq.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ft.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://br.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://fp.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://sk.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sz.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yt.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ij.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://mz.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ol.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://du.huanxung.cn


<!-- 参考信息 -->