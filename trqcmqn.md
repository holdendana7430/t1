代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://hr.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://om.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://vw.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://fs.nicolike.cn

[A06] 字符串转数字
来源：http://hh.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://vi.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ir.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fq.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oh.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lx.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xb.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vd.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ef.jctech888.com.cn

[A07] 数字转字符串
来源：http://mp.hnjuh.cn

Py:   str(42)
来源：http://qm.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://yk.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://gz.colortex.cn

TS:   String(42)
来源：http://nw.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ks.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://ex.colortex.cn

Ruby: 42.to_s
来源：http://we.asd995.cn

C#:   42.ToString()
来源：http://zw.panjiajie.cn

[A08] 取整与四舍五入
来源：http://zy.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vi.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pw.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hk.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kc.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://px.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rq.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xo.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zn.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://ml.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jc.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pa.hahajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lk.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zu.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dn.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bl.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uw.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zi.jianghongdianzi.cn

[A10] 生成随机数
来源：http://ts.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://jl.nszjky.cn

PHP:  random_int(1, 100);
来源：http://so.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ii.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pv.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://pv.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kg.colortex.cn

Ruby: rand(1..100)
来源：http://ci.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://de.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://dg.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://dx.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fb.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://aw.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wa.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://hz.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xu.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qw.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rh.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://tv.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xq.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://df.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://hi.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://tq.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://dd.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kd.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://pd.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://gi.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vf.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://uq.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://kr.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://mg.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://vl.lnxyls.cn

Java: "第一行\n第二行"
来源：http://pa.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://uo.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://oh.asd995.cn

C#:   "第一行\n第二行"
来源：http://ue.jctech888.com.cn

[A14] 注释写法
来源：http://zb.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zl.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tf.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://wl.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://oq.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://us.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://cy.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zp.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://lh.shxzskj.cn

[A15] 空值判断与默认值
来源：http://ln.szsharing.cn

Py:   value = data or "默认值"
来源：http://jn.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://tg.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://bf.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://hx.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ha.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://cp.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://hv.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://md.szxytkj.cn

[A16] 真假值判断规则
来源：http://nq.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ph.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wc.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nx.shtwfgs.cn

TS:   if (!x) {}
来源：http://gu.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zh.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ls.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cs.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hq.9csxet.cn

[A17] 位运算
来源：http://gi.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sa.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yy.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cr.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hf.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hy.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oy.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nb.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qh.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://pn.asd995.cn

Py:   ord("A"); chr(65)
来源：http://ey.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://pd.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bm.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hp.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://qq.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kj.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://pm.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://le.wgjwhj.cn

[A19] 交换两个变量
来源：http://nd.wgjwhj.cn

Py:   a, b = b, a
来源：http://jw.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cx.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://ip.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://su.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://qo.panjiajie.cn

Go:   a, b = b, a
来源：http://xm.colortex.cn

Ruby: a, b = b, a
来源：http://zo.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://ls.chemitech.net.cn

[A20] 读取标准输入
来源：http://oi.szsharing.cn

Py:   name = input("请输入：")
来源：http://st.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://th.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jy.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://sm.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://bu.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://by.panjiajie.cn

Ruby: gets.chomp
来源：http://da.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://qg.szsharing.cn

[A21] 保留指定小数位输出
来源：http://bp.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://ji.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yj.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://ua.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://xt.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://uf.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kl.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://tz.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://vs.jctech888.com.cn

[A22] 获取字符串长度
来源：http://rx.nszjky.cn

Py:   len(s)
来源：http://tz.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kt.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nl.yuexingan06.cn

TS:   s.length
来源：http://sf.newstarts.cn

Java: s.length()
来源：http://lw.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bq.nszjky.cn

Ruby: s.length
来源：http://dt.hnjuh.cn

C#:   s.Length
来源：http://xg.asd995.cn

[A23] 大小写转换
来源：http://rq.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ns.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kr.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cf.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jr.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pm.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lr.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qm.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qi.lnxyls.cn

[A24] 去除首尾空白
来源：http://ow.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dn.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bd.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ra.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oy.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ba.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://xg.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oe.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://al.wgjwhj.cn

[A25] 字符串比较
来源：http://bk.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://pe.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://db.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mh.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bl.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rl.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rx.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jv.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ex.jctech888.com.cn

[A26] 类型转换总览
来源：http://dx.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ax.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rh.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://md.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://cf.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pj.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sn.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ic.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rb.521024.cn

================================================================================
来源：http://tc.szsharing.cn

B. 流程控制
来源：http://hw.hahajie.cn

================================================================================
来源：http://nh.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://fs.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oj.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rf.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mv.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ro.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xi.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://au.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wi.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qi.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://pc.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lx.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sn.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cf.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bv.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dw.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pr.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://we.shxzskj.cn

[B03] switch / match / case
来源：http://vi.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xg.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nn.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hu.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fa.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wf.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mu.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lm.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ew.lnxyls.cn

[B04] for 计数循环
来源：http://jj.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://en.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vd.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fq.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://az.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cy.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hw.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://nv.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rm.colortex.cn

[B05] 遍历数组 / 列表
来源：http://ul.newstarts.cn

Py:   for item in arr: print(item)
来源：http://fh.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yw.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nw.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gq.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tj.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yl.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://aa.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bp.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://af.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jh.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dj.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fr.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yn.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mj.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vf.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jn.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fr.shtwfgs.cn

[B07] while 循环
来源：http://zk.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://gm.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bj.521024.cn

JS:   while (i < 10) { i++; }
来源：http://vi.521024.cn

TS:   while (i < 10) { i++; }
来源：http://gg.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://sy.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://on.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://ic.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://ja.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://yb.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://wn.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pz.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://we.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://tu.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://qr.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://di.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://og.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://lr.colortex.cn

[B09] break 与 continue
来源：http://ky.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ek.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oj.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wk.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xf.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oc.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xz.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xb.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sl.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://ze.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vt.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ii.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fx.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vp.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ot.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ih.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bb.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jv.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://rz.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://ae.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://wh.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zq.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qk.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oy.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yk.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://og.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gx.asd995.cn

[B12] 跳出多层循环
来源：http://yq.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fk.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mh.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fc.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xu.shxzskj.cn


<!-- 参考信息 -->