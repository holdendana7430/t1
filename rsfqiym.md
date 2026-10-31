代发 wailian999

[A06] 字符串转数字
来源：http://gd.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://hg.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ks.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wq.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wp.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vh.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ct.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ko.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bz.huanxung.cn

[A07] 数字转字符串
来源：http://co.nszjky.cn

Py:   str(42)
来源：http://cn.521024.cn

PHP:  (string) 42; strval(42)
来源：http://su.szsharing.cn

JS:   String(42); (42).toString()
来源：http://pj.shxzskj.cn

TS:   String(42)
来源：http://rj.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ys.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://dw.nszjky.cn

Ruby: 42.to_s
来源：http://gj.9csxet.cn

C#:   42.ToString()
来源：http://uq.asd995.cn

[A08] 取整与四舍五入
来源：http://ze.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dt.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hc.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://es.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ty.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vx.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ig.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ev.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ka.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://al.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aj.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yz.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ro.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xt.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kz.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://py.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bx.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ds.yuexingan06.cn

[A10] 生成随机数
来源：http://hx.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://bm.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://px.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cm.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zj.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://pr.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tb.bjjhwx.cn

Ruby: rand(1..100)
来源：http://pp.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://jl.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://fg.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://fx.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ho.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uy.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ua.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://ve.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bp.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tn.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://md.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://gc.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://me.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tx.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://ac.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://yj.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://ek.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ht.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://po.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://fk.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wy.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://qs.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://wk.521024.cn

JS:   "第一行\n第二行"
来源：http://ad.nicolike.cn

TS:   "第一行\n第二行"
来源：http://qm.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://ta.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://yh.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://sv.huanxung.cn

C#:   "第一行\n第二行"
来源：http://lt.hnjuh.cn

[A14] 注释写法
来源：http://ok.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mv.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nr.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://oz.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://rn.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xk.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://cc.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hb.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://zg.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://pu.gzmigu.cn

Py:   value = data or "默认值"
来源：http://ep.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://ku.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://mn.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://qr.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dv.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://qh.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://qo.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://fb.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://er.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hn.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yg.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rw.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://xc.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oo.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dv.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bv.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fz.shtwfgs.cn

[A17] 位运算
来源：http://lr.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jb.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zy.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fe.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yl.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wr.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zv.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vm.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ou.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://yn.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://sl.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://zy.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dn.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nd.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://uk.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://am.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://yv.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://df.gzmigu.cn

[A19] 交换两个变量
来源：http://dv.lnxyls.cn

Py:   a, b = b, a
来源：http://tv.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ji.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://ri.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://gd.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://vq.wgjwhj.cn

Go:   a, b = b, a
来源：http://xz.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://pk.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://gv.asd995.cn

[A20] 读取标准输入
来源：http://hx.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://se.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zn.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vl.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://cz.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://lv.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jr.9csxet.cn

Ruby: gets.chomp
来源：http://fg.huanxung.cn

C#:   Console.ReadLine();
来源：http://ja.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://me.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://sp.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fh.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://tq.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://hu.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://np.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wt.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://np.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://gu.hahajie.cn

[A22] 获取字符串长度
来源：http://na.panjiajie.cn

Py:   len(s)
来源：http://yx.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ix.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tl.nicolike.cn

TS:   s.length
来源：http://lt.haigaiapp.cn

Java: s.length()
来源：http://hl.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mq.521024.cn

Ruby: s.length
来源：http://rl.jctech888.com.cn

C#:   s.Length
来源：http://ft.bookmarksfly.cn

[A23] 大小写转换
来源：http://vw.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dg.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cy.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vv.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xc.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pw.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xp.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ug.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eh.hnjuh.cn

[A24] 去除首尾空白
来源：http://ms.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wx.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qk.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qt.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dd.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mr.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://gq.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jd.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iq.hahajie.cn

[A25] 字符串比较
来源：http://dy.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://nd.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pt.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://or.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bu.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nn.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tp.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fm.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qq.wgjwhj.cn

[A26] 类型转换总览
来源：http://nx.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yq.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bz.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ry.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://nx.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hg.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nu.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mj.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://el.lnxyls.cn

================================================================================
来源：http://rt.lnxyls.cn

B. 流程控制
来源：http://xn.shtwfgs.cn

================================================================================
来源：http://vt.huanxung.cn

[B01] 条件判断 if / else
来源：http://ex.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vu.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gr.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ww.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pf.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ot.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ot.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yf.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ay.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://ee.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nc.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xb.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sd.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://py.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yi.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mg.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cv.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mc.hahajie.cn

[B03] switch / match / case
来源：http://wm.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yi.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ns.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ga.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xt.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xl.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dh.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gy.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tl.panjiajie.cn

[B04] for 计数循环
来源：http://dv.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://rz.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tm.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ql.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://be.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mb.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vg.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://ol.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://re.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://tm.colortex.cn

Py:   for item in arr: print(item)
来源：http://ix.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://am.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zt.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vq.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wr.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ki.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://wg.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ng.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://hm.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ot.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qt.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ey.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aj.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dx.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zb.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zw.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jm.jctech888.com.cn

[B07] while 循环
来源：http://jf.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://xy.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://df.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://lx.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://ny.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://hw.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hb.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://fz.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://ae.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://gv.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://ap.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://az.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://vd.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://wr.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://xf.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qn.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ty.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://wn.haigaiapp.cn

[B09] break 与 continue
来源：http://mc.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qk.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ow.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pq.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rx.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dx.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zp.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://cz.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nv.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xt.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zs.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wy.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://la.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yh.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lv.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bw.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://qr.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://va.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://kd.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://du.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://to.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://en.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fo.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://wl.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dx.shtwfgs.cn

[B12] 跳出多层循环
来源：http://tx.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ad.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ur.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ln.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jg.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vp.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ko.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dk.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://im.521024.cn


<!-- 参考信息 -->