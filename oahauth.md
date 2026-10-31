代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://dw.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://qz.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://ot.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://km.521024.cn

[A06] 字符串转数字
来源：http://wx.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://cn.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rk.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://up.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ek.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mm.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mh.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lx.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fc.huixiangedu.cn

[A07] 数字转字符串
来源：http://bc.jctech888.com.cn

Py:   str(42)
来源：http://ol.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://qi.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://ff.chemitech.net.cn

TS:   String(42)
来源：http://cv.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sf.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://qq.szsharing.cn

Ruby: 42.to_s
来源：http://ib.nszjky.cn

C#:   42.ToString()
来源：http://ru.nicolike.cn

[A08] 取整与四舍五入
来源：http://gn.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bc.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hp.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hs.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jd.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tu.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nh.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ka.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qx.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://fc.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ag.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://to.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vx.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bb.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xv.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dd.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qq.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://um.szsharing.cn

[A10] 生成随机数
来源：http://xy.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://cn.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://pa.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dl.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pz.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://uw.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nx.shxzskj.cn

Ruby: rand(1..100)
来源：http://po.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://uh.huanxung.cn

[A11] 条件表达式（三元）
来源：http://xz.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://nk.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ci.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://np.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://th.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://pr.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qq.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vz.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ug.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://dx.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cy.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ak.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://mw.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://dw.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://ed.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xf.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://df.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://bu.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://js.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://nz.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://pl.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://hz.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://bi.huanxung.cn

Java: "第一行\n第二行"
来源：http://mw.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://yn.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://gf.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://wh.nicolike.cn

[A14] 注释写法
来源：http://es.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ls.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dj.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://in.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://nr.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vr.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://qu.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hl.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://bj.nicolike.cn

[A15] 空值判断与默认值
来源：http://sb.szxytkj.cn

Py:   value = data or "默认值"
来源：http://rp.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://dd.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://ar.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://vc.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bz.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://at.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://mb.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://cq.haigaiapp.cn

[A16] 真假值判断规则
来源：http://mv.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gl.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gy.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yi.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://oa.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ou.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dm.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pa.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nj.nszjky.cn

[A17] 位运算
来源：http://pu.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ol.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ox.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pv.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hg.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://je.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ex.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ur.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bf.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://ab.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://cu.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://ck.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ql.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ax.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://rm.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ql.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://vn.colortex.cn

C#:   (int)'A'; (char)65
来源：http://bp.nicolike.cn

[A19] 交换两个变量
来源：http://cf.szxytkj.cn

Py:   a, b = b, a
来源：http://lw.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ng.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://xr.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://fu.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://gm.panjiajie.cn

Go:   a, b = b, a
来源：http://cx.szxytkj.cn

Ruby: a, b = b, a
来源：http://sg.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://bj.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://yg.newstarts.cn

Py:   name = input("请输入：")
来源：http://aa.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gk.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kj.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://dw.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://xw.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ks.szsharing.cn

Ruby: gets.chomp
来源：http://ai.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://qt.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://xd.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://rh.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ux.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://ca.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://jv.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://gr.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gg.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://he.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://tt.lnxyls.cn

[A22] 获取字符串长度
来源：http://wy.wgjwhj.cn

Py:   len(s)
来源：http://my.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zu.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dt.huanxung.cn

TS:   s.length
来源：http://ql.hnjuh.cn

Java: s.length()
来源：http://vt.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gi.szsharing.cn

Ruby: s.length
来源：http://vl.hahajie.cn

C#:   s.Length
来源：http://sk.szsharing.cn

[A23] 大小写转换
来源：http://ys.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zz.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tu.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lz.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://au.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hh.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sz.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vz.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mi.yuexingan06.cn

[A24] 去除首尾空白
来源：http://tu.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zv.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://re.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://no.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jk.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lq.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://sx.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gl.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://li.hahajie.cn

[A25] 字符串比较
来源：http://iw.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://bc.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ru.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ah.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fi.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://si.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pm.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dx.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://os.colortex.cn

[A26] 类型转换总览
来源：http://yp.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bu.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://es.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ab.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://vp.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ch.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ub.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kd.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wl.newstarts.cn

================================================================================
来源：http://xw.hnjuh.cn

B. 流程控制
来源：http://zx.bookmarksfly.cn

================================================================================
来源：http://zd.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://wp.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://av.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sf.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yv.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aw.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://av.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kw.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dy.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://um.9csxet.cn

[B02] 多分支 else if / elif
来源：http://ze.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pj.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rg.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oc.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bz.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jw.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aa.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sn.gzmigu.cn

[B03] switch / match / case
来源：http://qi.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yi.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ku.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qq.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zr.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ch.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ve.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rb.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qi.nszjky.cn

[B04] for 计数循环
来源：http://kf.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://ug.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kk.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ca.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ka.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zn.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://go.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://cq.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kj.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://ni.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://hz.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://of.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hr.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ym.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cp.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://st.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://eb.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xc.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://bb.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ft.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yf.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hk.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wc.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sm.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kl.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rk.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mc.szsharing.cn

[B07] while 循环
来源：http://ph.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://kf.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yc.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://yo.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://hh.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://oc.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lu.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://xi.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://xf.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://pq.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://ah.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eq.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://zg.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://ln.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://bu.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://se.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zd.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://gq.shxzskj.cn

[B09] break 与 continue
来源：http://xb.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pu.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://it.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zx.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gj.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vc.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dw.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cx.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lv.newstarts.cn

[B10] 遍历同时拿索引
来源：http://vl.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ft.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hr.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ze.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oh.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cm.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nt.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qt.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qe.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://rj.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://oy.asd995.cn

PHP:  range(0, 10, 2);
来源：http://bl.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cr.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mh.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ev.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fh.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://qb.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://as.szsharing.cn

[B12] 跳出多层循环
来源：http://ni.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pp.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jm.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ij.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qy.szxytkj.cn


<!-- 参考信息 -->