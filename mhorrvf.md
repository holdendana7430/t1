代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pz.bjjhwx.cn

[A07] 数字转字符串
来源：http://mt.colortex.cn

Py:   str(42)
来源：http://hi.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://my.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://og.yuexingan06.cn

TS:   String(42)
来源：http://xq.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://an.colortex.cn

Go:   strconv.Itoa(42)
来源：http://bw.bookmarksfly.cn

Ruby: 42.to_s
来源：http://gs.yuexingan06.cn

C#:   42.ToString()
来源：http://tv.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://xr.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fw.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ao.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://od.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wy.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ie.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eh.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rd.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hb.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://uj.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://av.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hk.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bx.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oq.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://at.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ck.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zb.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://io.huixiangedu.cn

[A10] 生成随机数
来源：http://rp.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://jl.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://cp.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gx.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zr.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://yb.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://on.szxytkj.cn

Ruby: rand(1..100)
来源：http://be.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://cf.9csxet.cn

[A11] 条件表达式（三元）
来源：http://iz.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://qc.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ay.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fr.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ds.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://li.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gv.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ji.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qc.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://ju.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yc.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nm.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://ob.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://ke.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://qs.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ab.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://ke.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://vd.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wv.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://fh.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://hd.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://oi.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://jm.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://gc.szsharing.cn

Go:   "第一行\n第二行"
来源：http://pf.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://se.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://mo.szsharing.cn

[A14] 注释写法
来源：http://fh.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kl.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lx.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://em.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://ur.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kb.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://ku.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bn.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://ne.lnxyls.cn

[A15] 空值判断与默认值
来源：http://po.hnjuh.cn

Py:   value = data or "默认值"
来源：http://tv.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://lt.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://vt.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://st.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kf.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://bj.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://vp.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://em.jctech888.com.cn

[A16] 真假值判断规则
来源：http://cy.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://op.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rf.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://do.nszjky.cn

TS:   if (!x) {}
来源：http://bc.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vl.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ry.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cf.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nk.hnjuh.cn

[A17] 位运算
来源：http://tx.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lq.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gy.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ky.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://br.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sq.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eb.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fj.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qe.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://tw.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://ka.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://no.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fp.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vk.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://ki.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oo.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://kd.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://dj.shxzskj.cn

[A19] 交换两个变量
来源：http://nt.newstarts.cn

Py:   a, b = b, a
来源：http://yk.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ko.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://na.asd995.cn

TS:   [a, b] = [b, a];
来源：http://zq.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://hd.nicolike.cn

Go:   a, b = b, a
来源：http://sp.jctech888.com.cn

Ruby: a, b = b, a
来源：http://jp.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://qm.colortex.cn

[A20] 读取标准输入
来源：http://sd.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://xr.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lz.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dq.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://is.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://br.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pw.hnjuh.cn

Ruby: gets.chomp
来源：http://zt.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://jx.newstarts.cn

[A21] 保留指定小数位输出
来源：http://fz.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://zw.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://or.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://du.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://qi.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://hh.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ia.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://rh.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://vz.shxzukj.cn

[A22] 获取字符串长度
来源：http://oj.huixiangedu.cn

Py:   len(s)
来源：http://jl.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ww.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mm.huixinmuqiang.cn

TS:   s.length
来源：http://qk.huixiangedu.cn

Java: s.length()
来源：http://qc.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qt.521024.cn

Ruby: s.length
来源：http://mf.chemitech.net.cn

C#:   s.Length
来源：http://bh.hahajie.cn

[A23] 大小写转换
来源：http://lq.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fi.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kv.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pl.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vi.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kg.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://no.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pf.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gg.muxihuayi.cn

[A24] 去除首尾空白
来源：http://tc.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kh.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vr.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gm.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iz.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ur.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://zh.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gx.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ch.jctech888.com.cn

[A25] 字符串比较
来源：http://ir.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://fa.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tw.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bm.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pp.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ay.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uq.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wz.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lh.nszjky.cn

[A26] 类型转换总览
来源：http://nj.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sw.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yr.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jo.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://yh.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ye.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://il.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://te.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nc.nszjky.cn

================================================================================
来源：http://ic.szxytkj.cn

B. 流程控制
来源：http://zo.lnxyls.cn

================================================================================
来源：http://va.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://wd.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xe.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nq.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tf.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pp.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fe.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://be.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rm.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mx.hahajie.cn

[B02] 多分支 else if / elif
来源：http://tn.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gm.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sk.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lj.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yg.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://es.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kn.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kq.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jf.szsharing.cn

[B03] switch / match / case
来源：http://kr.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bm.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hl.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cl.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qb.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sk.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cm.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dl.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mq.nszjky.cn

[B04] for 计数循环
来源：http://rr.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://ql.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xd.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vq.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lz.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ll.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hd.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://dj.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vg.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://nq.szsharing.cn

Py:   for item in arr: print(item)
来源：http://da.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wv.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yq.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yl.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lv.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ax.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://dx.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ww.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://qu.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ed.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://az.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ek.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ij.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ij.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iv.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pr.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://np.panjiajie.cn

[B07] while 循环
来源：http://fs.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://bt.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fj.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://zs.521024.cn

TS:   while (i < 10) { i++; }
来源：http://eo.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://vr.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gz.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://zm.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://lw.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://wi.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://ln.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wk.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://vl.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://xp.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://qq.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fi.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fh.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://nd.colortex.cn

[B09] break 与 continue
来源：http://bh.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ns.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rw.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oo.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yl.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fb.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fs.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dp.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://if.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://sq.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xz.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vq.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ld.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yv.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jb.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lw.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bm.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zb.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://xp.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://ge.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://av.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ri.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sz.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ws.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bn.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://xr.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mr.shxzukj.cn

[B12] 跳出多层循环
来源：http://mq.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gp.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://im.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bp.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ia.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fp.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lr.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ka.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vj.chemitech.net.cn

[B13] 判断是否为数字
来源：http://xp.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://pj.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://wl.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ee.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://re.nszjky.cn

Java: x instanceof Number
来源：http://pq.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dn.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://ct.521024.cn


<!-- 参考信息 -->