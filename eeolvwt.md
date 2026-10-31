代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gk.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qh.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ar.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zs.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://cj.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://dn.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://zv.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://zf.chemitech.net.cn

[A06] 字符串转数字
来源：http://br.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://wp.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hw.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ru.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oz.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zt.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kc.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jt.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tg.huanxung.cn

[A07] 数字转字符串
来源：http://nl.asd995.cn

Py:   str(42)
来源：http://wx.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://vl.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://xa.bjjhwx.cn

TS:   String(42)
来源：http://nh.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qb.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://qs.shxzukj.cn

Ruby: 42.to_s
来源：http://ho.hahajie.cn

C#:   42.ToString()
来源：http://ip.nszjky.cn

[A08] 取整与四舍五入
来源：http://ku.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nw.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mc.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ty.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qx.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cl.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vb.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uo.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kg.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://vw.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cp.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vv.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yy.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eq.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vg.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eu.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kv.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gb.szxytkj.cn

[A10] 生成随机数
来源：http://pz.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://vi.nszjky.cn

PHP:  random_int(1, 100);
来源：http://vz.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vs.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zt.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://ov.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eo.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://sa.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://ih.521024.cn

[A11] 条件表达式（三元）
来源：http://gs.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://lt.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cs.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rj.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bh.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://tn.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zo.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://we.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jz.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://jh.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rz.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lr.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://nu.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://ma.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://gf.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zb.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://jm.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://ef.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mh.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://uv.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://ro.newstarts.cn

JS:   "第一行\n第二行"
来源：http://xm.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://ny.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://uh.szsharing.cn

Go:   "第一行\n第二行"
来源：http://vu.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://uv.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://qr.521024.cn

[A14] 注释写法
来源：http://du.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sw.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://os.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://ro.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://pe.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://al.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://vp.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://me.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://lw.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://mp.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://jg.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://hq.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://fn.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://en.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ck.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://bk.nicolike.cn

Ruby: value = data || "默认值"
来源：http://jm.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://bv.szsharing.cn

[A16] 真假值判断规则
来源：http://bo.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qg.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xx.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://au.newstarts.cn

TS:   if (!x) {}
来源：http://mi.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xa.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tl.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gp.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://um.huixinmuqiang.cn

[A17] 位运算
来源：http://vz.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tw.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xw.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ku.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ah.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fl.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iv.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hm.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://do.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://gq.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://sg.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://bz.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://io.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ts.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://mx.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fm.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://jc.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://li.gzmigu.cn

[A19] 交换两个变量
来源：http://gq.muxihuayi.cn

Py:   a, b = b, a
来源：http://vi.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vl.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://lv.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://jl.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://ga.jctech888.com.cn

Go:   a, b = b, a
来源：http://jn.huanxung.cn

Ruby: a, b = b, a
来源：http://he.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://ki.bookmarksfly.cn

[A20] 读取标准输入
来源：http://hm.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://gm.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://st.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ar.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://in.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://gf.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zl.huanxung.cn

Ruby: gets.chomp
来源：http://ne.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://ls.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://vp.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://no.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cw.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://jq.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://uq.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://ln.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://va.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://cp.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://no.521024.cn

[A22] 获取字符串长度
来源：http://es.521024.cn

Py:   len(s)
来源：http://ny.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ic.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ls.yuexingan06.cn

TS:   s.length
来源：http://sy.shxzskj.cn

Java: s.length()
来源：http://bt.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kz.gzmigu.cn

Ruby: s.length
来源：http://bi.asd995.cn

C#:   s.Length
来源：http://uq.bookmarksfly.cn

[A23] 大小写转换
来源：http://zq.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mk.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://je.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jh.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lx.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hr.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://an.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wd.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ky.wgjwhj.cn

[A24] 去除首尾空白
来源：http://fd.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zy.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oy.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fh.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://se.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ge.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://bg.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ll.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fx.9csxet.cn

[A25] 字符串比较
来源：http://fx.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://se.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lg.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://se.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yt.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kw.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rg.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cu.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://es.yuexingan06.cn

[A26] 类型转换总览
来源：http://vw.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ss.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nd.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zn.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://vs.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pj.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ln.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ea.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mm.jctech888.com.cn

================================================================================
来源：http://mk.jianghongdianzi.cn

B. 流程控制
来源：http://qt.gzmigu.cn

================================================================================
来源：http://dt.nszjky.cn

[B01] 条件判断 if / else
来源：http://qw.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://df.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://si.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rv.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dg.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eu.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fa.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xg.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zi.szsharing.cn

[B02] 多分支 else if / elif
来源：http://wb.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ye.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ou.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oo.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yd.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tt.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bk.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cy.hahajie.cn

[B03] switch / match / case
来源：http://cq.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pe.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wb.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zt.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ji.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://av.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vo.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gn.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lk.hahajie.cn

[B04] for 计数循环
来源：http://np.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://xf.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dt.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xr.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lq.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://et.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fx.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://jd.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gy.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://ab.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://rx.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ih.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mg.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://we.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pr.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mw.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://ec.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jj.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://hr.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vx.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mu.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ir.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wq.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tp.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zl.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cv.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://db.nszjky.cn

[B07] while 循环
来源：http://qa.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://zh.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ix.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://gl.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://gx.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://xb.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wu.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://hq.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://vy.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://pw.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://tq.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hr.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://gk.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://te.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://eb.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yp.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vq.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://hj.haigaiapp.cn

[B09] break 与 continue
来源：http://qy.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ea.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eu.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://il.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ee.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iw.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hw.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ig.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://km.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://ug.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lv.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xt.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://et.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tx.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ia.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xb.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ms.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cu.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://tk.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://hn.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://ws.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gi.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rk.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zc.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ln.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://xa.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pe.szxytkj.cn

[B12] 跳出多层循环
来源：http://pa.asd995.cn


<!-- 参考信息 -->