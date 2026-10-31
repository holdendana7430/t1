代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://cy.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://mv.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://vx.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://kg.asd995.cn

[A06] 字符串转数字
来源：http://nt.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://jh.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yp.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vk.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cq.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pc.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fv.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wc.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://an.lnxyls.cn

[A07] 数字转字符串
来源：http://zm.9csxet.cn

Py:   str(42)
来源：http://ub.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://um.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://pw.yuntaijiaju.cn

TS:   String(42)
来源：http://pm.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://no.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://nv.nszjky.cn

Ruby: 42.to_s
来源：http://vt.bjjhwx.cn

C#:   42.ToString()
来源：http://pv.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://zy.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fc.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zn.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://au.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nz.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gj.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vk.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://co.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dw.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://yt.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kt.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://li.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ib.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://os.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://di.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gq.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hm.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cn.asd995.cn

[A10] 生成随机数
来源：http://nn.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://vv.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://nw.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nm.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ne.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://bk.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ol.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://hj.521024.cn

C#:   new Random().Next(1, 101)
来源：http://my.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://eq.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://rp.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yf.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qx.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lr.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://ni.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dx.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uk.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://la.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://cw.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lf.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yx.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://nm.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://yr.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://rj.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ab.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://om.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://rm.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ie.nicolike.cn

Py:   "第一行\n第二行"
来源：http://vm.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://fr.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://rd.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://vy.colortex.cn

Java: "第一行\n第二行"
来源：http://da.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://el.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://ci.521024.cn

C#:   "第一行\n第二行"
来源：http://te.wgjwhj.cn

[A14] 注释写法
来源：http://xg.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pg.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fb.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://hz.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://lr.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wk.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://yc.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lt.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://co.szxytkj.cn

[A15] 空值判断与默认值
来源：http://dn.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://eb.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://ad.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://rr.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://ud.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oa.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://zt.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://ca.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://wx.521024.cn

[A16] 真假值判断规则
来源：http://ks.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ya.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fp.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wz.521024.cn

TS:   if (!x) {}
来源：http://hh.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nf.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vl.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hs.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hc.haigaiapp.cn

[A17] 位运算
来源：http://er.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eh.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ar.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gy.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pn.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jl.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jm.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yl.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kl.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://kh.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://sc.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://zt.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tm.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vd.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://fd.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gx.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://zx.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://rm.colortex.cn

[A19] 交换两个变量
来源：http://sz.9csxet.cn

Py:   a, b = b, a
来源：http://ux.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ci.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://xy.521024.cn

TS:   [a, b] = [b, a];
来源：http://bh.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://sc.521024.cn

Go:   a, b = b, a
来源：http://ad.szxytkj.cn

Ruby: a, b = b, a
来源：http://ob.colortex.cn

C#:   (a, b) = (b, a);
来源：http://uf.jctech888.com.cn

[A20] 读取标准输入
来源：http://ol.newstarts.cn

Py:   name = input("请输入：")
来源：http://ly.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xc.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kv.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://we.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://hc.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uh.huanxung.cn

Ruby: gets.chomp
来源：http://yy.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://ic.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://du.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://tv.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://of.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://oq.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://cv.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://dw.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lq.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://pd.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://sm.panjiajie.cn

[A22] 获取字符串长度
来源：http://jk.colortex.cn

Py:   len(s)
来源：http://ou.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hx.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cs.newstarts.cn

TS:   s.length
来源：http://hf.jctech888.com.cn

Java: s.length()
来源：http://nq.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uz.yuntaijiaju.cn

Ruby: s.length
来源：http://jv.bjjhwx.cn

C#:   s.Length
来源：http://wk.haigaiapp.cn

[A23] 大小写转换
来源：http://qe.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zh.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qe.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ef.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pa.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hr.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://li.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lu.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bp.haigaiapp.cn

[A24] 去除首尾空白
来源：http://ef.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ou.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://no.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oy.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ye.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mg.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://mn.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ww.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wm.521024.cn

[A25] 字符串比较
来源：http://ge.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://nf.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mc.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://du.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qu.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ng.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kk.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://io.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ot.shxzukj.cn

[A26] 类型转换总览
来源：http://cb.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://md.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://st.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pw.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://co.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ny.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zu.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mk.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sz.9csxet.cn

================================================================================
来源：http://mi.shxzskj.cn

B. 流程控制
来源：http://qm.hahajie.cn

================================================================================
来源：http://ww.9csxet.cn

[B01] 条件判断 if / else
来源：http://xq.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xf.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://if.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wx.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mt.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lc.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jd.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pj.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iu.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://kq.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xh.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ms.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jh.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ja.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wr.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qc.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.shxzukj.cn

[B03] switch / match / case
来源：http://vn.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wf.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://st.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rb.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wy.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://me.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vu.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vj.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zp.shxzukj.cn

[B04] for 计数循环
来源：http://ba.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://hh.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hi.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nc.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bi.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tm.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ke.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://uc.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sv.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://xp.521024.cn

Py:   for item in arr: print(item)
来源：http://ql.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cy.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fe.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ht.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ra.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yu.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://qg.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xm.asd995.cn

[B06] 遍历字典 / 对象
来源：http://yq.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qg.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aq.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://in.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ux.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jg.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uv.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ka.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hr.haigaiapp.cn

[B07] while 循环
来源：http://ph.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://qr.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mi.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://xr.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://oe.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://mn.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gf.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://vd.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://ke.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://aw.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://pz.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cs.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://sw.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://sq.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://la.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qi.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cf.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://on.panjiajie.cn

[B09] break 与 continue
来源：http://lg.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ok.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ua.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ns.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iu.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ng.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hr.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sk.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://fk.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zx.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hk.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qd.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oa.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sf.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sl.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ib.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bg.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://of.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://za.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://kl.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ga.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ag.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://le.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wq.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://jc.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sf.huixiangedu.cn

[B12] 跳出多层循环
来源：http://ci.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ux.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wc.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ii.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bx.newstarts.cn


<!-- 参考信息 -->