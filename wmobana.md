代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://vs.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://if.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://av.panjiajie.cn

[A05] 整数除法与取模
来源：http://wc.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fs.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zg.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xc.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ng.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://if.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://ee.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://oz.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://ur.gzmigu.cn

[A06] 字符串转数字
来源：http://hi.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://zd.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qd.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mi.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wk.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ww.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yl.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tg.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fd.shtwfgs.cn

[A07] 数字转字符串
来源：http://nf.521024.cn

Py:   str(42)
来源：http://bd.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://ui.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://ez.hnjuh.cn

TS:   String(42)
来源：http://kj.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://va.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://vf.shxzukj.cn

Ruby: 42.to_s
来源：http://bh.asd995.cn

C#:   42.ToString()
来源：http://mx.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://ei.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://di.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ph.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sj.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ji.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pf.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oz.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ou.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dv.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://ze.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ri.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lt.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rt.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kp.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tz.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pn.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jb.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hg.jctech888.com.cn

[A10] 生成随机数
来源：http://ps.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://oj.hahajie.cn

PHP:  random_int(1, 100);
来源：http://eo.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xu.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ax.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://qd.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://up.szsharing.cn

Ruby: rand(1..100)
来源：http://or.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://dr.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://qk.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://sf.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ew.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oy.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wi.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://wu.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://on.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gc.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ec.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://ac.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yj.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ln.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://ur.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://rl.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://ga.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vh.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://hc.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://dw.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://un.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://we.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://dg.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://bq.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://jr.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://rb.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://za.521024.cn

Ruby: "第一行\n第二行"
来源：http://xu.nszjky.cn

C#:   "第一行\n第二行"
来源：http://kj.wgjwhj.cn

[A14] 注释写法
来源：http://ru.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jd.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rz.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://ii.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://ln.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kg.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://pv.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jr.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://jb.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://ky.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://qq.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://yg.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://nd.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://hp.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ks.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://cs.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://nh.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://xw.shxzskj.cn

[A16] 真假值判断规则
来源：http://ue.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pe.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nc.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kf.gzmigu.cn

TS:   if (!x) {}
来源：http://zy.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mg.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mq.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gu.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vx.lnxyls.cn

[A17] 位运算
来源：http://hv.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hl.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ml.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qe.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oz.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gw.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pz.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zy.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://mo.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://kj.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://sr.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vl.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vw.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://kb.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wz.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://ig.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://ud.nszjky.cn

[A19] 交换两个变量
来源：http://ce.lnxyls.cn

Py:   a, b = b, a
来源：http://wi.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oh.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://ht.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://go.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://zb.521024.cn

Go:   a, b = b, a
来源：http://iv.9csxet.cn

Ruby: a, b = b, a
来源：http://ye.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://cd.shtwfgs.cn

[A20] 读取标准输入
来源：http://lq.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://ej.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://us.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ar.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://wz.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://ib.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ay.bjjhwx.cn

Ruby: gets.chomp
来源：http://zz.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://et.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://gr.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://ph.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gh.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://nd.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://xu.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://vs.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ps.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://vj.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://wc.hahajie.cn

[A22] 获取字符串长度
来源：http://mk.wgjwhj.cn

Py:   len(s)
来源：http://cj.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nn.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gm.yuntaijiaju.cn

TS:   s.length
来源：http://uy.bjjhwx.cn

Java: s.length()
来源：http://ww.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mr.shxzskj.cn

Ruby: s.length
来源：http://to.shxzukj.cn

C#:   s.Length
来源：http://tk.huixinmuqiang.cn

[A23] 大小写转换
来源：http://rf.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kq.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://om.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mq.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://io.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nk.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pt.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aa.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://np.huanxung.cn

[A24] 去除首尾空白
来源：http://jm.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kz.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lv.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yc.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tb.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ls.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://wp.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ro.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bd.huanxung.cn

[A25] 字符串比较
来源：http://tw.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://iv.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://on.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ec.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nx.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zl.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yi.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ub.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bc.lnxyls.cn

[A26] 类型转换总览
来源：http://fm.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://na.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mq.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wb.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://qp.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nh.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fn.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ke.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ia.9csxet.cn

================================================================================
来源：http://gj.bookmarksfly.cn

B. 流程控制
来源：http://vp.szsharing.cn

================================================================================
来源：http://um.shxzskj.cn

[B01] 条件判断 if / else
来源：http://qk.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tw.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://od.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jx.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pf.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://up.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oo.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vi.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cr.hahajie.cn

[B02] 多分支 else if / elif
来源：http://do.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kk.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://do.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bh.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nt.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ma.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xh.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eq.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cp.521024.cn

[B03] switch / match / case
来源：http://ue.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rc.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jn.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hq.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dh.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mp.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ks.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bu.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ky.jctech888.com.cn

[B04] for 计数循环
来源：http://qe.521024.cn

Py:   for i in range(10): print(i)
来源：http://im.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iu.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kx.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vf.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gn.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kh.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://yx.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cv.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://vu.nszjky.cn

Py:   for item in arr: print(item)
来源：http://kx.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hx.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zl.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kd.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hh.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vw.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://ip.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yg.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://gc.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kp.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xv.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ix.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qk.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bc.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tp.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aq.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vv.szsharing.cn

[B07] while 循环
来源：http://ua.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://tx.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fb.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://pm.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://ow.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://up.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ky.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://lx.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://as.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://ly.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://xg.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lo.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://gc.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://og.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://bf.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ap.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wc.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://tr.huixiangedu.cn

[B09] break 与 continue
来源：http://at.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jh.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pd.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zw.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://px.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://br.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ak.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pt.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uy.nszjky.cn

[B10] 遍历同时拿索引
来源：http://pz.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sd.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qm.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eh.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cy.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fp.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ih.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ni.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tr.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://ya.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ft.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://zs.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vv.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hc.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://de.szsharing.cn


<!-- 参考信息 -->