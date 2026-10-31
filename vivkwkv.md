代发 wailian999

[A06] 字符串转数字
来源：http://bd.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://ay.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vu.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kx.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zy.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://do.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zh.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xn.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ao.colortex.cn

[A07] 数字转字符串
来源：http://sj.gzmigu.cn

Py:   str(42)
来源：http://mq.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://cb.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://rk.shtwfgs.cn

TS:   String(42)
来源：http://ug.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zb.colortex.cn

Go:   strconv.Itoa(42)
来源：http://kx.hnjuh.cn

Ruby: 42.to_s
来源：http://zj.yuntaijiaju.cn

C#:   42.ToString()
来源：http://rl.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://yo.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vg.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pq.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://do.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qo.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rf.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tl.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yt.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zy.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://zg.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xt.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://le.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://si.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://by.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wa.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wq.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://at.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://si.huixinmuqiang.cn

[A10] 生成随机数
来源：http://nz.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://dj.newstarts.cn

PHP:  random_int(1, 100);
来源：http://po.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hb.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://om.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://ac.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zm.shxzukj.cn

Ruby: rand(1..100)
来源：http://vu.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://ya.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://sa.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://xk.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xq.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zu.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jl.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://gt.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fh.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sh.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lg.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://ms.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dp.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ff.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://sw.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://ot.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://dq.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qs.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://ao.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://po.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jk.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://fb.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://ja.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://eb.9csxet.cn

TS:   "第一行\n第二行"
来源：http://hi.shxzskj.cn

Java: "第一行\n第二行"
来源：http://ht.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://cx.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://tz.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://rf.shxzukj.cn

[A14] 注释写法
来源：http://wy.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nw.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dr.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://gv.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://qk.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gw.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://mu.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://di.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://he.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://hl.szxytkj.cn

Py:   value = data or "默认值"
来源：http://gf.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ns.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://gv.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://nj.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yp.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://jr.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://nq.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://ka.yuexingan06.cn

[A16] 真假值判断规则
来源：http://bt.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zo.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ez.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xo.colortex.cn

TS:   if (!x) {}
来源：http://ki.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fm.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wy.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yo.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ar.bookmarksfly.cn

[A17] 位运算
来源：http://bp.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://im.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zb.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qm.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tx.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rq.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dj.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mg.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cq.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://sw.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://aw.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://uk.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ag.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gu.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://gx.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kv.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://yp.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://gi.shxzskj.cn

[A19] 交换两个变量
来源：http://ct.nszjky.cn

Py:   a, b = b, a
来源：http://ad.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ou.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://wz.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://tv.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://dx.shxzskj.cn

Go:   a, b = b, a
来源：http://wp.muxihuayi.cn

Ruby: a, b = b, a
来源：http://sv.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://ww.muxihuayi.cn

[A20] 读取标准输入
来源：http://xe.panjiajie.cn

Py:   name = input("请输入：")
来源：http://gz.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iv.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cz.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://gl.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://qk.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ga.lnxyls.cn

Ruby: gets.chomp
来源：http://ru.shxzukj.cn

C#:   Console.ReadLine();
来源：http://an.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://ke.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://em.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://we.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://jx.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://ut.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://bb.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ra.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://dd.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://ea.chemitech.net.cn

[A22] 获取字符串长度
来源：http://qu.bjjhwx.cn

Py:   len(s)
来源：http://dl.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pm.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wi.asd995.cn

TS:   s.length
来源：http://zr.bjjhwx.cn

Java: s.length()
来源：http://qb.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iw.hahajie.cn

Ruby: s.length
来源：http://vp.huanxung.cn

C#:   s.Length
来源：http://op.yuntaijiaju.cn

[A23] 大小写转换
来源：http://cb.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gv.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rh.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hy.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ul.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ib.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ag.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cu.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xp.yuexingan06.cn

[A24] 去除首尾空白
来源：http://gh.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ul.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jq.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://on.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qj.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xt.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://fp.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://et.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yq.yuntaijiaju.cn

[A25] 字符串比较
来源：http://sr.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://th.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rd.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xf.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sg.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wz.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rb.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lg.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ej.huixiangedu.cn

[A26] 类型转换总览
来源：http://kb.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://en.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ht.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qj.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://fs.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fd.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ny.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mf.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yl.szxytkj.cn

================================================================================
来源：http://ot.panjiajie.cn

B. 流程控制
来源：http://ji.yuntaijiaju.cn

================================================================================
来源：http://cy.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://sj.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ke.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rc.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mm.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yl.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ak.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ym.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oz.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hw.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://wr.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ux.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vb.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ho.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vi.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ja.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zw.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rp.newstarts.cn

[B03] switch / match / case
来源：http://se.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zl.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bn.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uq.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wi.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://we.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pu.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gn.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yn.yuexingan06.cn

[B04] for 计数循环
来源：http://jf.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://ti.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pr.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://do.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oa.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cw.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ar.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://dn.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jw.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://jw.huanxung.cn

Py:   for item in arr: print(item)
来源：http://he.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fj.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://me.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wo.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gl.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://co.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://xr.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tx.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://wd.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hx.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fp.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nf.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ck.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fq.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ae.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gd.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zy.bjjhwx.cn

[B07] while 循环
来源：http://hg.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://tt.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cj.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://je.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://mg.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://sn.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://za.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://zf.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://tm.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://my.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://er.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hk.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://wl.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://ff.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://kv.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vq.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://an.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://th.huixinmuqiang.cn

[B09] break 与 continue
来源：http://sy.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hw.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://do.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oh.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nc.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ex.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tq.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jd.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ed.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://yc.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ek.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fk.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://up.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qc.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dh.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bd.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rh.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ph.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://aj.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://sg.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://ps.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://an.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uv.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://id.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://td.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://we.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eq.huanxung.cn

[B12] 跳出多层循环
来源：http://re.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ze.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tb.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xv.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fw.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ni.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ab.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kt.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://br.wgjwhj.cn


<!-- 参考信息 -->