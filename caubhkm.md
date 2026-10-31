代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://rr.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://ff.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://xh.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://nv.shtwfgs.cn

[A06] 字符串转数字
来源：http://we.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://tv.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ta.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fe.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ax.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mp.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ym.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tb.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ge.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://xr.shxzskj.cn

Py:   str(42)
来源：http://bb.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://hf.hahajie.cn

JS:   String(42); (42).toString()
来源：http://wn.wgjwhj.cn

TS:   String(42)
来源：http://is.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nq.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://kw.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://bk.shtwfgs.cn

C#:   42.ToString()
来源：http://ew.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://hw.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ow.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://za.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kc.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zs.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qe.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vl.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ze.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tn.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://sg.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dy.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iy.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fy.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qf.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fz.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ug.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yt.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uo.hnjuh.cn

[A10] 生成随机数
来源：http://dj.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://ee.nicolike.cn

PHP:  random_int(1, 100);
来源：http://th.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wx.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ef.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://st.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jk.haigaiapp.cn

Ruby: rand(1..100)
来源：http://rh.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://oh.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://io.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://vn.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cv.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xu.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yi.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://on.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://af.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hl.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ah.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://ww.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jt.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yp.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://kr.asd995.cn

TS:   `Hello, ${name}!`
来源：http://el.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://rp.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lu.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://dm.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://gf.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fu.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://ta.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://jb.huanxung.cn

JS:   "第一行\n第二行"
来源：http://ha.asd995.cn

TS:   "第一行\n第二行"
来源：http://nj.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://jn.colortex.cn

Go:   "第一行\n第二行"
来源：http://uc.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://gm.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://uq.bjjhwx.cn

[A14] 注释写法
来源：http://mh.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dd.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rj.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://ap.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://vc.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://le.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://rf.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hk.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://yc.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://hd.gzmigu.cn

Py:   value = data or "默认值"
来源：http://gg.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://jc.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://jz.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://mx.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vk.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://er.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://gl.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://jk.huixiangedu.cn

[A16] 真假值判断规则
来源：http://rx.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jf.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qq.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zg.nszjky.cn

TS:   if (!x) {}
来源：http://gs.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qn.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://st.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qh.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ph.shtwfgs.cn

[A17] 位运算
来源：http://ox.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lk.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gh.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kw.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xh.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wt.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://md.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dt.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xo.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://ry.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://xe.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://ve.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fy.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uk.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://sl.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rk.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://yq.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://zy.hahajie.cn

[A19] 交换两个变量
来源：http://xh.asd995.cn

Py:   a, b = b, a
来源：http://wl.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pj.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://fs.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://mp.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://qz.jctech888.com.cn

Go:   a, b = b, a
来源：http://jd.nicolike.cn

Ruby: a, b = b, a
来源：http://wz.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://jd.shxzukj.cn

[A20] 读取标准输入
来源：http://ge.colortex.cn

Py:   name = input("请输入：")
来源：http://js.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zd.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tc.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://jl.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://om.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pb.bookmarksfly.cn

Ruby: gets.chomp
来源：http://pk.9csxet.cn

C#:   Console.ReadLine();
来源：http://fy.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://jk.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://je.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bu.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://ve.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://ha.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://hy.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ev.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://rh.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://mf.9csxet.cn

[A22] 获取字符串长度
来源：http://lm.huixinmuqiang.cn

Py:   len(s)
来源：http://bv.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ef.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ft.szsharing.cn

TS:   s.length
来源：http://ha.huixiangedu.cn

Java: s.length()
来源：http://cy.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xd.jianghongdianzi.cn

Ruby: s.length
来源：http://ap.yuexingan06.cn

C#:   s.Length
来源：http://aw.bookmarksfly.cn

[A23] 大小写转换
来源：http://yp.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://he.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ub.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nd.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fe.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uh.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pm.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ti.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://um.lnxyls.cn

[A24] 去除首尾空白
来源：http://ke.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qj.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ou.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uq.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mv.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ss.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://ft.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tn.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jy.shxzskj.cn

[A25] 字符串比较
来源：http://bo.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://hq.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ik.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ci.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kc.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tw.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ps.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wv.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nw.yuexingan06.cn

[A26] 类型转换总览
来源：http://ml.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vm.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oe.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vq.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://ad.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ej.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ra.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rn.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ad.shxzukj.cn

================================================================================
来源：http://pk.gzmigu.cn

B. 流程控制
来源：http://bb.szsharing.cn

================================================================================
来源：http://wy.nicolike.cn

[B01] 条件判断 if / else
来源：http://vt.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://go.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hg.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pd.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yx.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zx.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dy.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ba.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ca.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://nz.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mp.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dm.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nw.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nz.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ma.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pk.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qq.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.jianghongdianzi.cn

[B03] switch / match / case
来源：http://vt.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ol.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oj.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kf.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vc.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hi.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gc.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wa.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cs.shtwfgs.cn

[B04] for 计数循环
来源：http://bi.521024.cn

Py:   for i in range(10): print(i)
来源：http://nv.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tv.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qn.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pi.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://su.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lm.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://nc.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iz.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://sm.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://tl.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zq.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dj.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nv.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zs.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sc.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://hz.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ku.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://in.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://la.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hi.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nm.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uk.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sp.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ng.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ko.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aa.lnxyls.cn

[B07] while 循环
来源：http://ut.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://jr.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kz.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://xc.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://tf.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://ur.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lu.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ri.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://hk.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://er.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://he.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gf.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://lc.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://oz.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://xv.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gx.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tj.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://lz.9csxet.cn

[B09] break 与 continue
来源：http://vc.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mc.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wz.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xx.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bn.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rl.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ay.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mh.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://im.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://cl.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vu.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uy.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ze.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://st.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yn.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rn.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rt.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xk.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://ts.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://pj.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://qi.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://du.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lc.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lf.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xd.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://yu.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kv.colortex.cn

[B12] 跳出多层循环
来源：http://ug.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ms.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qf.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ob.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rb.bookmarksfly.cn


<!-- 参考信息 -->