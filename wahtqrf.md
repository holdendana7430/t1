代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dw.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sm.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xt.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cl.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://hm.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://lr.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://vq.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://qs.yuexingan06.cn

[A06] 字符串转数字
来源：http://ub.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://fm.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jp.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sf.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nz.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uf.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tb.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fz.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://on.gzmigu.cn

[A07] 数字转字符串
来源：http://dw.nszjky.cn

Py:   str(42)
来源：http://yf.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://ck.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://uo.wgjwhj.cn

TS:   String(42)
来源：http://jy.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bs.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://yx.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://rr.jctech888.com.cn

C#:   42.ToString()
来源：http://iv.521024.cn

[A08] 取整与四舍五入
来源：http://vf.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nm.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vi.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wx.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ni.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pn.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dr.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wn.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ru.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://wi.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eo.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zn.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zk.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mh.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://va.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://do.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kn.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lf.haigaiapp.cn

[A10] 生成随机数
来源：http://gd.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://bu.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://df.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kn.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wz.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://im.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pq.jctech888.com.cn

Ruby: rand(1..100)
来源：http://jg.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://yd.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://zg.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://ov.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yq.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hc.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://og.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://sl.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zk.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zl.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eh.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://sr.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rk.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fw.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://xy.asd995.cn

TS:   `Hello, ${name}!`
来源：http://gg.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://qo.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pl.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://gw.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://nl.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ap.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://sn.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://qf.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://mx.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://ri.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://ir.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://ye.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://wt.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://lk.9csxet.cn

[A14] 注释写法
来源：http://su.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ob.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wk.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://zb.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://pz.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ne.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://jp.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gp.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://ew.shxzukj.cn

[A15] 空值判断与默认值
来源：http://dp.lnxyls.cn

Py:   value = data or "默认值"
来源：http://hf.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://nz.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://ij.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://xd.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gk.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://ez.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://al.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://id.chemitech.net.cn

[A16] 真假值判断规则
来源：http://sl.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fc.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nc.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xm.chemitech.net.cn

TS:   if (!x) {}
来源：http://df.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yi.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tr.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sr.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qf.wgjwhj.cn

[A17] 位运算
来源：http://fu.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bc.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ae.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xa.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cn.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ba.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xu.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hj.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ey.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://co.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://it.521024.cn

PHP:  ord("A"); chr(65)
来源：http://fy.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://he.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ft.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://hl.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qq.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://qz.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://lq.yuexingan06.cn

[A19] 交换两个变量
来源：http://bm.szsharing.cn

Py:   a, b = b, a
来源：http://wm.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yy.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://qf.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://np.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://mv.hahajie.cn

Go:   a, b = b, a
来源：http://py.panjiajie.cn

Ruby: a, b = b, a
来源：http://lw.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://ht.haigaiapp.cn

[A20] 读取标准输入
来源：http://fd.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://qd.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ju.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bg.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://cv.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://zs.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://og.panjiajie.cn

Ruby: gets.chomp
来源：http://ii.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://lh.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://wq.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://ls.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bo.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://cw.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://eq.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://pj.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xc.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://uf.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://lb.szxytkj.cn

[A22] 获取字符串长度
来源：http://og.jianghongdianzi.cn

Py:   len(s)
来源：http://jo.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mb.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://my.huixinmuqiang.cn

TS:   s.length
来源：http://yx.huixiangedu.cn

Java: s.length()
来源：http://il.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aq.wgjwhj.cn

Ruby: s.length
来源：http://ie.nicolike.cn

C#:   s.Length
来源：http://pn.asd995.cn

[A23] 大小写转换
来源：http://ca.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dp.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dr.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kf.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://av.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vo.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jm.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://px.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ym.wgjwhj.cn

[A24] 去除首尾空白
来源：http://oo.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yp.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sq.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sc.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ia.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vy.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://ok.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nd.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aw.chemitech.net.cn

[A25] 字符串比较
来源：http://cq.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://ew.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://to.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oy.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zs.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mx.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nf.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hc.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zi.wgjwhj.cn

[A26] 类型转换总览
来源：http://ws.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ug.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ve.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bh.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://ju.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mk.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sh.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pp.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://te.9csxet.cn

================================================================================
来源：http://hb.newstarts.cn

B. 流程控制
来源：http://xq.lnxyls.cn

================================================================================
来源：http://bd.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://ej.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bq.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ur.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fl.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pp.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://we.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rd.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nu.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cf.colortex.cn

[B02] 多分支 else if / elif
来源：http://kq.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kp.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oo.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pj.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hw.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rf.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://or.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ht.huixinmuqiang.cn

[B03] switch / match / case
来源：http://zp.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yg.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gl.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kb.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tx.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://si.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qh.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oc.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uw.chemitech.net.cn

[B04] for 计数循环
来源：http://je.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://ps.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hx.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://js.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ps.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rv.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gw.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://no.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bb.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://tr.hahajie.cn

Py:   for item in arr: print(item)
来源：http://fb.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://km.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rg.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ye.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rt.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pu.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://xm.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nj.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://tz.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wk.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vb.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://la.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kq.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ai.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://na.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://to.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mq.chemitech.net.cn

[B07] while 循环
来源：http://hg.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://xj.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rq.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://lm.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://ia.colortex.cn

Java: while (i < 10) { i++; }
来源：http://vb.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dr.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://we.521024.cn

C#:   while (i < 10) { i++; }
来源：http://qv.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://od.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://in.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ai.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://np.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://zq.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://df.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wa.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bl.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://hn.yuexingan06.cn

[B09] break 与 continue
来源：http://jc.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nt.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://io.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lc.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ep.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://um.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cf.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lc.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://vi.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ps.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://is.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xr.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qs.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rv.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ik.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ct.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://md.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://nd.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://ct.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://ev.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ll.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gj.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jx.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://na.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://et.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ur.muxihuayi.cn

[B12] 跳出多层循环
来源：http://zr.muxihuayi.cn


<!-- 参考信息 -->