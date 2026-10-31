代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ql.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qs.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://wr.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jj.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://od.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oq.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://lv.huixiangedu.cn

[A05] 整数除法与取模
来源：http://xf.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eh.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xx.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rf.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jf.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://pq.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://ep.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://aq.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://cq.haigaiapp.cn

[A06] 字符串转数字
来源：http://jt.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://hv.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uy.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kg.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ab.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://im.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fo.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zb.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wi.wgjwhj.cn

[A07] 数字转字符串
来源：http://np.shxzukj.cn

Py:   str(42)
来源：http://ti.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://up.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://fo.yuntaijiaju.cn

TS:   String(42)
来源：http://wn.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://te.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://jy.lnxyls.cn

Ruby: 42.to_s
来源：http://um.nicolike.cn

C#:   42.ToString()
来源：http://pr.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://vp.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tv.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ua.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vy.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pu.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qk.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ce.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ym.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xx.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://lx.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bs.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vp.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ow.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bl.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yz.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uo.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zr.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lk.shtwfgs.cn

[A10] 生成随机数
来源：http://dp.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://ut.szsharing.cn

PHP:  random_int(1, 100);
来源：http://zj.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qd.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vy.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://rh.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tw.huixiangedu.cn

Ruby: rand(1..100)
来源：http://hw.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://xj.huanxung.cn

[A11] 条件表达式（三元）
来源：http://di.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://xq.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fs.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xl.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tm.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://yt.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xj.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ub.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rt.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://hl.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gu.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bp.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://cr.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://ev.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://zx.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xw.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://ob.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://kc.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gf.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://ks.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://px.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://rr.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://ms.szsharing.cn

Java: "第一行\n第二行"
来源：http://lp.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://ql.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://aa.hahajie.cn

C#:   "第一行\n第二行"
来源：http://ot.haigaiapp.cn

[A14] 注释写法
来源：http://qt.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://es.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xa.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://ff.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://fx.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vm.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://hm.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tt.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://rg.nszjky.cn

[A15] 空值判断与默认值
来源：http://xt.szsharing.cn

Py:   value = data or "默认值"
来源：http://qr.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://og.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://rx.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://qv.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ma.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://tq.hahajie.cn

Ruby: value = data || "默认值"
来源：http://gl.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://mg.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://wm.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ji.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://by.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zh.9csxet.cn

TS:   if (!x) {}
来源：http://df.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dq.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zx.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pw.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gs.szsharing.cn

[A17] 位运算
来源：http://tf.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sc.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ac.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vp.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hg.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qo.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ix.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xc.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ob.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://yy.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://hk.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://tk.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://we.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rr.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://ii.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yf.521024.cn

Ruby: "A".ord; 65.chr
来源：http://xv.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://wg.huixiangedu.cn

[A19] 交换两个变量
来源：http://im.nszjky.cn

Py:   a, b = b, a
来源：http://tg.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ig.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://gn.colortex.cn

TS:   [a, b] = [b, a];
来源：http://cx.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://hx.521024.cn

Go:   a, b = b, a
来源：http://ch.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://ge.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://ca.nszjky.cn

[A20] 读取标准输入
来源：http://oh.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://vo.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dz.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bc.colortex.cn

TS:   // Node.js：readline 模块
来源：http://ve.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://kf.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ig.bjjhwx.cn

Ruby: gets.chomp
来源：http://hp.shxzukj.cn

C#:   Console.ReadLine();
来源：http://ul.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://ue.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://fi.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oo.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://ov.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://fo.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://fm.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://th.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://zf.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://vj.jctech888.com.cn

[A22] 获取字符串长度
来源：http://qn.nicolike.cn

Py:   len(s)
来源：http://ob.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rl.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oa.nicolike.cn

TS:   s.length
来源：http://vy.shtwfgs.cn

Java: s.length()
来源：http://dq.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fh.chemitech.net.cn

Ruby: s.length
来源：http://fb.muxihuayi.cn

C#:   s.Length
来源：http://rr.hnjuh.cn

[A23] 大小写转换
来源：http://ut.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://af.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fp.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://na.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hb.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fo.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rq.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://am.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ni.hahajie.cn

[A24] 去除首尾空白
来源：http://bu.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bd.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hs.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wk.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zo.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wn.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://hd.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dk.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mi.asd995.cn

[A25] 字符串比较
来源：http://vo.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://du.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dj.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eo.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rh.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dk.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ha.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zi.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xb.szsharing.cn

[A26] 类型转换总览
来源：http://co.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wz.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://an.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rs.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://mc.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fy.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tv.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zt.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ju.9csxet.cn

================================================================================
来源：http://ca.bjjhwx.cn

B. 流程控制
来源：http://vk.shxzskj.cn

================================================================================
来源：http://uu.nszjky.cn

[B01] 条件判断 if / else
来源：http://di.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ys.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ih.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://up.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ex.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xv.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://np.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uj.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sv.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://vm.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://id.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wq.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fe.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gt.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xp.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vx.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jl.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bu.szxytkj.cn

[B03] switch / match / case
来源：http://kz.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cy.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dl.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://np.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qy.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wz.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://th.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ef.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://of.nszjky.cn

[B04] for 计数循环
来源：http://cr.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://xy.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ef.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zw.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rm.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://es.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kj.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://ya.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rt.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://wy.huanxung.cn

Py:   for item in arr: print(item)
来源：http://ix.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ie.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lv.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zj.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://za.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lq.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://pc.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jn.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://qk.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kd.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rc.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nq.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kk.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qw.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://re.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ri.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wj.yuntaijiaju.cn

[B07] while 循环
来源：http://fk.9csxet.cn

Py:   while i < 10: i += 1
来源：http://hq.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hx.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://la.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://ui.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://ka.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lj.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://ra.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://jg.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://ym.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://nw.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ei.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://kg.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://gm.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://xo.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xb.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yt.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://qf.asd995.cn

[B09] break 与 continue
来源：http://mw.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fs.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cj.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pg.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oi.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tb.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://le.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gd.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oo.asd995.cn

[B10] 遍历同时拿索引
来源：http://ae.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qm.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mj.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cb.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zd.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ew.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iw.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mr.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hb.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://oc.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://uf.chemitech.net.cn


<!-- 参考信息 -->