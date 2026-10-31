代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://hd.521024.cn

Go:   7 / 2; 7 % 2
来源：http://tr.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://fi.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://hh.yuexingan06.cn

[A06] 字符串转数字
来源：http://ah.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://yh.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rk.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dv.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yn.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://au.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wy.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fs.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uh.shtwfgs.cn

[A07] 数字转字符串
来源：http://rt.colortex.cn

Py:   str(42)
来源：http://fs.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://rv.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://bo.hnjuh.cn

TS:   String(42)
来源：http://yf.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://br.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://mi.hahajie.cn

Ruby: 42.to_s
来源：http://vq.nicolike.cn

C#:   42.ToString()
来源：http://px.lnxyls.cn

[A08] 取整与四舍五入
来源：http://dp.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fo.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zy.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ef.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pz.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://du.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zx.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lj.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gy.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://ca.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ij.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gu.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gl.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fb.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ic.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ed.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nn.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vt.panjiajie.cn

[A10] 生成随机数
来源：http://qd.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://tq.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://ae.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://er.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wv.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://wy.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://st.colortex.cn

Ruby: rand(1..100)
来源：http://ux.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://sj.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://ky.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://hm.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gg.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uf.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vs.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://ki.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wk.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mw.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://py.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://wv.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sm.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ev.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://su.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://xq.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://ku.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rs.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://fq.asd995.cn

C#:   $"Hello, {name}!"
来源：http://wb.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zt.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://eh.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://qa.colortex.cn

JS:   "第一行\n第二行"
来源：http://tl.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://dt.hnjuh.cn

Java: "第一行\n第二行"
来源：http://dh.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://af.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://gh.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://lc.jianghongdianzi.cn

[A14] 注释写法
来源：http://be.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cm.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fc.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://vj.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://jl.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sk.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://jg.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wm.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://yq.nicolike.cn

[A15] 空值判断与默认值
来源：http://vr.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://fk.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ct.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://vj.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://je.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ws.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://mp.nszjky.cn

Ruby: value = data || "默认值"
来源：http://gw.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://nd.panjiajie.cn

[A16] 真假值判断规则
来源：http://bw.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kj.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cx.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qf.muxihuayi.cn

TS:   if (!x) {}
来源：http://zx.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vd.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yu.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rs.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ml.bookmarksfly.cn

[A17] 位运算
来源：http://fr.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qf.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://am.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://me.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://so.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ii.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ym.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ml.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xo.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://yh.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://fh.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://eb.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ac.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bh.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://cb.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ih.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://cb.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://xh.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://zg.panjiajie.cn

Py:   a, b = b, a
来源：http://ix.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ui.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://ty.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://er.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://rk.szsharing.cn

Go:   a, b = b, a
来源：http://rq.nszjky.cn

Ruby: a, b = b, a
来源：http://rs.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://yt.shxzukj.cn

[A20] 读取标准输入
来源：http://ye.newstarts.cn

Py:   name = input("请输入：")
来源：http://bh.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mq.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dw.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://rq.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://ji.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://by.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://lb.szxytkj.cn

C#:   Console.ReadLine();
来源：http://tv.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://ob.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://di.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rk.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://er.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://xc.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://jd.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zh.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://ie.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://hf.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://oa.szxytkj.cn

Py:   len(s)
来源：http://uq.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yy.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fe.szxytkj.cn

TS:   s.length
来源：http://jj.shxzukj.cn

Java: s.length()
来源：http://jn.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zw.hahajie.cn

Ruby: s.length
来源：http://mz.bjjhwx.cn

C#:   s.Length
来源：http://yr.muxihuayi.cn

[A23] 大小写转换
来源：http://le.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bf.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pp.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pi.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://op.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://un.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qp.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xh.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hi.huixiangedu.cn

[A24] 去除首尾空白
来源：http://zc.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yo.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://po.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mt.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://td.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qg.521024.cn

Go:   strings.TrimSpace(s)
来源：http://vd.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xo.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qo.muxihuayi.cn

[A25] 字符串比较
来源：http://ip.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://pr.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bi.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lt.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ec.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ax.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pf.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ed.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://js.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://lh.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hc.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zd.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aa.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://my.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vr.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ko.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mx.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zq.newstarts.cn

================================================================================
来源：http://ny.nszjky.cn

B. 流程控制
来源：http://cv.nszjky.cn

================================================================================
来源：http://qe.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://ja.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://we.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tw.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ik.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rn.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oh.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cp.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ln.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://as.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://fi.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ac.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hx.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ga.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qf.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vj.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ax.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ib.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hu.huanxung.cn

[B03] switch / match / case
来源：http://fg.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://if.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oo.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rb.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mz.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qc.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kj.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cb.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tr.bookmarksfly.cn

[B04] for 计数循环
来源：http://dv.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://oe.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gi.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://np.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ak.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ka.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ny.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://ri.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tg.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://mm.colortex.cn

Py:   for item in arr: print(item)
来源：http://tk.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ek.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ux.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ks.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pj.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xq.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://wh.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yf.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://zf.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xv.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ol.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yc.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sb.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yb.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pp.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zn.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wj.lnxyls.cn

[B07] while 循环
来源：http://nj.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://fb.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vs.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://su.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://pq.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://ej.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wj.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://ek.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://ec.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://gs.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://oc.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pr.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://tb.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://ny.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://wb.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://la.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pu.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://ny.huixinmuqiang.cn

[B09] break 与 continue
来源：http://yx.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aa.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cs.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dl.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://al.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eo.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dh.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bf.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qa.szsharing.cn

[B10] 遍历同时拿索引
来源：http://xc.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ui.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ng.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qo.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ku.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zd.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ww.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yy.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://to.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://ue.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://xs.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://jd.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://br.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://is.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sx.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jq.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://nd.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ic.panjiajie.cn

[B12] 跳出多层循环
来源：http://wu.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ii.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vo.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fy.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bh.jianghongdianzi.cn


<!-- 参考信息 -->