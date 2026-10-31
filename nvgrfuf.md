代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fi.9csxet.cn

[A07] 数字转字符串
来源：http://gf.bjjhwx.cn

Py:   str(42)
来源：http://df.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://zb.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://ym.nicolike.cn

TS:   String(42)
来源：http://fi.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vg.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://pj.nszjky.cn

Ruby: 42.to_s
来源：http://nm.huixinmuqiang.cn

C#:   42.ToString()
来源：http://zp.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://dc.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ln.hnjuh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kd.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gp.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tx.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dj.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ui.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fk.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fn.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://fz.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nk.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zt.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sh.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ae.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yl.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dk.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uw.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fb.huixinmuqiang.cn

[A10] 生成随机数
来源：http://cs.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://db.521024.cn

PHP:  random_int(1, 100);
来源：http://od.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dz.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dn.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://fn.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tg.nszjky.cn

Ruby: rand(1..100)
来源：http://rh.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://yq.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://ou.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://ol.jianghongdianzi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://iu.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vu.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://br.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://nv.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kt.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://su.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pf.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://ue.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mw.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lt.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://fp.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://lk.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://id.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lx.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://ha.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://gk.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://po.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://bq.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://ns.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://xw.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://zs.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://jh.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://lj.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://xq.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://pe.yuntaijiaju.cn

[A14] 注释写法
来源：http://rn.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xz.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kg.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://dv.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://uw.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hg.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://hg.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hj.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://xs.colortex.cn

[A15] 空值判断与默认值
来源：http://ii.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://fi.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://pp.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://an.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://mi.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://po.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://mh.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://lx.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://vd.asd995.cn

[A16] 真假值判断规则
来源：http://al.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ar.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ek.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fc.shxzukj.cn

TS:   if (!x) {}
来源：http://qp.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ir.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fi.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cv.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qo.huanxung.cn

[A17] 位运算
来源：http://go.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://py.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rz.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yi.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ok.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ls.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lu.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rp.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mp.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://oe.colortex.cn

Py:   ord("A"); chr(65)
来源：http://ts.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://mh.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ff.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ei.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://nu.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mu.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://ij.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://ks.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://uc.wgjwhj.cn

Py:   a, b = b, a
来源：http://bj.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://if.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://sn.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://kq.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://dx.521024.cn

Go:   a, b = b, a
来源：http://vm.huanxung.cn

Ruby: a, b = b, a
来源：http://qw.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://xz.nszjky.cn

[A20] 读取标准输入
来源：http://ab.szsharing.cn

Py:   name = input("请输入：")
来源：http://rx.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://th.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aw.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://fp.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://fy.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ki.wgjwhj.cn

Ruby: gets.chomp
来源：http://mg.9csxet.cn

C#:   Console.ReadLine();
来源：http://kj.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://pq.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://mj.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vg.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://ul.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://po.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://wj.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vs.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://hw.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://op.huixiangedu.cn

[A22] 获取字符串长度
来源：http://og.chemitech.net.cn

Py:   len(s)
来源：http://hm.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ts.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xo.colortex.cn

TS:   s.length
来源：http://lt.hahajie.cn

Java: s.length()
来源：http://vr.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ij.nszjky.cn

Ruby: s.length
来源：http://nf.521024.cn

C#:   s.Length
来源：http://rl.shxzukj.cn

[A23] 大小写转换
来源：http://bv.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mb.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ct.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kx.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ue.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://if.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kd.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pw.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ob.colortex.cn

[A24] 去除首尾空白
来源：http://px.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://na.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yh.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sr.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pd.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://na.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://fw.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ou.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ie.nszjky.cn

[A25] 字符串比较
来源：http://fm.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://sv.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://it.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ir.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bw.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hn.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ul.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lr.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nt.szsharing.cn

[A26] 类型转换总览
来源：http://wb.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qm.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gn.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dq.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://br.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vi.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dy.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qr.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ng.yuexingan06.cn

================================================================================
来源：http://jx.asd995.cn

B. 流程控制
来源：http://yx.bookmarksfly.cn

================================================================================
来源：http://kh.gzmigu.cn

[B01] 条件判断 if / else
来源：http://mm.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ru.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ei.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://te.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rc.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pb.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ns.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ue.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sc.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://ut.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://te.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rz.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://en.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kd.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rt.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pr.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jn.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fd.lnxyls.cn

[B03] switch / match / case
来源：http://rp.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iw.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ay.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://so.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lt.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ba.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://il.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tj.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ss.bjjhwx.cn

[B04] for 计数循环
来源：http://sj.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://uo.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jo.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fd.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vd.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ff.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jd.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://ma.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gu.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://gf.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://qi.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pu.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dt.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oz.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ul.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ka.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://lt.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://su.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://ey.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://va.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ws.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cw.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cg.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xk.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cy.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hg.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ih.panjiajie.cn

[B07] while 循环
来源：http://ps.szsharing.cn

Py:   while i < 10: i += 1
来源：http://ov.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qd.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://ou.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://tt.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://bp.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yy.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://oa.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://an.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://ig.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ij.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sx.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://wf.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://lv.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://qa.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ct.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gz.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://me.colortex.cn

[B09] break 与 continue
来源：http://yn.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tm.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qe.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jk.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ez.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ah.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dk.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bl.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mf.szsharing.cn

[B10] 遍历同时拿索引
来源：http://gk.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ep.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ze.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lx.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yl.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yc.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pj.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zv.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xg.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://xp.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://pa.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://vl.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://db.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ot.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ap.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gd.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://ua.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fv.muxihuayi.cn

[B12] 跳出多层循环
来源：http://fi.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ur.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rn.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://un.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ck.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ad.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tj.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://om.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mh.jctech888.com.cn

[B13] 判断是否为数字
来源：http://on.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://br.nicolike.cn

PHP:  is_numeric($x)
来源：http://cb.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bu.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cq.huanxung.cn

Java: x instanceof Number
来源：http://ea.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qf.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://em.nicolike.cn


<!-- 参考信息 -->