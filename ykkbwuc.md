代发 wailian999

JS:   String(42); (42).toString()
来源：http://hl.hahajie.cn

TS:   String(42)
来源：http://xh.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sn.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://ih.hnjuh.cn

Ruby: 42.to_s
来源：http://gk.muxihuayi.cn

C#:   42.ToString()
来源：http://so.shxzukj.cn

[A08] 取整与四舍五入
来源：http://nf.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xn.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hd.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vs.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zv.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ad.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jp.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bd.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xw.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://ii.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://or.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pe.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yt.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xl.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zv.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vd.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jt.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fz.szxytkj.cn

[A10] 生成随机数
来源：http://hf.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://gu.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://lm.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tf.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ca.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://sr.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oo.jctech888.com.cn

Ruby: rand(1..100)
来源：http://bu.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://mu.521024.cn

[A11] 条件表达式（三元）
来源：http://un.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ym.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hl.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dh.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://th.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://ur.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fs.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jn.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bt.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://xf.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qy.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qp.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://dk.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://sx.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://va.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://jo.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://hl.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ot.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://fs.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://qh.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://bt.szsharing.cn

TS:   "第一行\n第二行"
来源：http://vi.shxzukj.cn

Java: "第一行\n第二行"
来源：http://sz.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://cd.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://se.szsharing.cn

C#:   "第一行\n第二行"
来源：http://lg.nicolike.cn

[A14] 注释写法
来源：http://yd.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vm.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mj.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://rx.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://zw.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://du.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://iw.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lv.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://cx.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://hl.shxzukj.cn

Py:   value = data or "默认值"
来源：http://de.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://tj.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://vl.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://br.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://le.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://wy.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://ih.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://pc.521024.cn

[A16] 真假值判断规则
来源：http://mk.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ql.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oq.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qm.newstarts.cn

TS:   if (!x) {}
来源：http://gc.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aw.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sq.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zo.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ls.jctech888.com.cn

[A17] 位运算
来源：http://rw.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wx.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cu.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uy.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cq.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://im.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qx.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kg.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ed.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://mc.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://id.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://ak.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kr.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jh.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://do.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://au.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://mh.colortex.cn

C#:   (int)'A'; (char)65
来源：http://se.bjjhwx.cn

[A19] 交换两个变量
来源：http://pr.9csxet.cn

Py:   a, b = b, a
来源：http://ct.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ha.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://xm.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://nr.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://eb.wgjwhj.cn

Go:   a, b = b, a
来源：http://hd.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://ef.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://sl.shxzskj.cn

[A20] 读取标准输入
来源：http://ca.9csxet.cn

Py:   name = input("请输入：")
来源：http://aj.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://om.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fv.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://ry.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://yw.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vw.huanxung.cn

Ruby: gets.chomp
来源：http://vq.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://ns.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://me.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://bl.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lj.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://ip.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://yy.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://vy.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://at.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://od.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://yz.asd995.cn

[A22] 获取字符串长度
来源：http://yq.yuntaijiaju.cn

Py:   len(s)
来源：http://yw.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qn.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://re.hahajie.cn

TS:   s.length
来源：http://qx.yuntaijiaju.cn

Java: s.length()
来源：http://xp.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://md.lnxyls.cn

Ruby: s.length
来源：http://fg.muxihuayi.cn

C#:   s.Length
来源：http://mt.gzmigu.cn

[A23] 大小写转换
来源：http://so.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ma.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hn.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lu.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://km.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ei.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fh.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wi.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://by.panjiajie.cn

[A24] 去除首尾空白
来源：http://ee.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cs.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vb.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gb.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xi.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fk.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://gb.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ck.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gf.hahajie.cn

[A25] 字符串比较
来源：http://cv.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://tf.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jl.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vb.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://te.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yh.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hb.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nl.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ku.shxzukj.cn

[A26] 类型转换总览
来源：http://ut.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lu.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mz.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nb.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://fl.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ns.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iw.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://og.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bb.huixiangedu.cn

================================================================================
来源：http://jq.newstarts.cn

B. 流程控制
来源：http://mc.lnxyls.cn

================================================================================
来源：http://jc.newstarts.cn

[B01] 条件判断 if / else
来源：http://ah.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lq.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ah.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cx.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yn.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lc.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wr.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sq.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lh.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://yt.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rq.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wt.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fo.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hr.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qr.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ig.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pu.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hg.gzmigu.cn

[B03] switch / match / case
来源：http://uv.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gv.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ia.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tr.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ol.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ji.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yt.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vh.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ju.huanxung.cn

[B04] for 计数循环
来源：http://mi.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://tq.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iy.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ap.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mb.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kv.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sc.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://uq.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xc.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://bq.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://ts.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uw.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rf.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ea.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vc.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://es.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://as.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jd.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://zo.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lj.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lc.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rz.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rh.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://md.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lp.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ww.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://go.521024.cn

[B07] while 循环
来源：http://jr.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://ps.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kk.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://er.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://vz.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://vo.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cj.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://we.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://zx.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://bf.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://fu.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vr.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://hk.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://mw.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://fp.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zj.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gp.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://zn.hahajie.cn

[B09] break 与 continue
来源：http://dk.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lb.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://px.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ne.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ot.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jo.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eo.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hp.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lv.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://hi.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fb.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kp.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xt.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://my.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kq.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wr.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lf.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rl.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://kw.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://im.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://hg.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rp.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vv.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bi.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vw.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://ug.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mf.yuexingan06.cn

[B12] 跳出多层循环
来源：http://oe.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zd.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gg.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uu.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bv.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jc.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://py.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://he.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://at.9csxet.cn

[B13] 判断是否为数字
来源：http://vl.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://hl.nszjky.cn

PHP:  is_numeric($x)
来源：http://ui.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cs.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xh.haigaiapp.cn

Java: x instanceof Number
来源：http://nd.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pr.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://ce.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://pr.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://ip.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://me.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://no.panjiajie.cn


<!-- 参考信息 -->