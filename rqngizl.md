代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sk.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iu.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://gw.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iv.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ty.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vz.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://hs.panjiajie.cn

[A05] 整数除法与取模
来源：http://bb.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ef.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ew.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nv.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wc.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://yr.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://bc.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://dy.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://mx.yuexingan06.cn

[A06] 字符串转数字
来源：http://mf.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://wf.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ka.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://np.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kx.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://me.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://se.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fz.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lx.wgjwhj.cn

[A07] 数字转字符串
来源：http://li.muxihuayi.cn

Py:   str(42)
来源：http://fp.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://bi.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://fr.chemitech.net.cn

TS:   String(42)
来源：http://xo.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pj.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://jz.newstarts.cn

Ruby: 42.to_s
来源：http://ar.muxihuayi.cn

C#:   42.ToString()
来源：http://nx.szxytkj.cn

[A08] 取整与四舍五入
来源：http://sq.jianghongdianzi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pq.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mt.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dt.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vc.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://go.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oc.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jh.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fe.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://ab.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uh.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iy.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eh.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://er.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://je.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eq.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ez.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jr.chemitech.net.cn

[A10] 生成随机数
来源：http://mv.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://yr.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://ir.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gx.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yr.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://mj.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wi.9csxet.cn

Ruby: rand(1..100)
来源：http://lv.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://ss.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://tv.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://th.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xq.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oa.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zm.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://vs.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ph.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pi.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ct.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://xe.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hf.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gx.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://fs.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://vm.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://sm.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tc.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://ga.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://qa.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bj.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://jn.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://ob.colortex.cn

JS:   "第一行\n第二行"
来源：http://ee.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://ne.szsharing.cn

Java: "第一行\n第二行"
来源：http://ym.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://gq.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://mt.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://nb.hnjuh.cn

[A14] 注释写法
来源：http://cb.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ew.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vm.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://aj.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://ux.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ij.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://jl.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jh.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://wo.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://tu.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://wu.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://kc.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://wy.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://sy.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dv.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://rt.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://uv.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://dl.hahajie.cn

[A16] 真假值判断规则
来源：http://ey.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zs.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aq.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ca.newstarts.cn

TS:   if (!x) {}
来源：http://gv.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kd.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lt.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wq.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lw.yuntaijiaju.cn

[A17] 位运算
来源：http://lo.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qt.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uo.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eb.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cc.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://is.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ds.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hm.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://iu.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://np.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://fd.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kj.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oh.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://sj.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ho.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://nr.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://pu.lnxyls.cn

[A19] 交换两个变量
来源：http://uo.szxytkj.cn

Py:   a, b = b, a
来源：http://vl.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yn.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://qf.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://ew.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://an.lnxyls.cn

Go:   a, b = b, a
来源：http://rd.521024.cn

Ruby: a, b = b, a
来源：http://bf.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://dp.panjiajie.cn

[A20] 读取标准输入
来源：http://ix.521024.cn

Py:   name = input("请输入：")
来源：http://ve.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pb.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://le.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://zl.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://qu.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lv.yuexingan06.cn

Ruby: gets.chomp
来源：http://it.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://or.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://uy.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://ga.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://up.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://bq.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://oj.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://vw.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cg.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://mm.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://qe.colortex.cn

[A22] 获取字符串长度
来源：http://pj.yuntaijiaju.cn

Py:   len(s)
来源：http://ld.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fv.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zg.haigaiapp.cn

TS:   s.length
来源：http://th.chemitech.net.cn

Java: s.length()
来源：http://lh.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ua.colortex.cn

Ruby: s.length
来源：http://vy.nszjky.cn

C#:   s.Length
来源：http://wk.szxytkj.cn

[A23] 大小写转换
来源：http://iw.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gv.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hq.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uk.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tj.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pk.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ca.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nu.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sc.shtwfgs.cn

[A24] 去除首尾空白
来源：http://lm.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nl.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mu.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ro.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ge.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xo.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://eh.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ng.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lo.bjjhwx.cn

[A25] 字符串比较
来源：http://jo.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://bq.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oq.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://se.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rc.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fb.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nf.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qu.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xi.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://yo.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ez.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lc.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hq.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://pk.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dr.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gf.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://si.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://of.asd995.cn

================================================================================
来源：http://il.wgjwhj.cn

B. 流程控制
来源：http://ew.hnjuh.cn

================================================================================
来源：http://qh.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://el.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nq.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dn.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vs.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ff.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ed.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zz.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pr.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tw.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://ud.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vk.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uv.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sk.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rh.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mx.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qn.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://en.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://il.shxzskj.cn

[B03] switch / match / case
来源：http://dw.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ws.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://he.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dl.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bo.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nx.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zq.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yq.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ca.muxihuayi.cn

[B04] for 计数循环
来源：http://hg.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://et.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ow.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lk.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ne.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cx.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://js.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://vy.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dr.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://yy.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://bc.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fo.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dr.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vw.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tf.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fi.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://el.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wt.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://rl.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ml.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jg.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yh.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aq.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ba.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sr.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ed.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xy.huixinmuqiang.cn

[B07] while 循环
来源：http://pp.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://oi.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nt.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://ay.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://dc.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://xh.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eu.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://vw.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://yi.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://bu.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://em.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jr.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://hn.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://og.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://jq.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://et.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fh.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://kr.521024.cn

[B09] break 与 continue
来源：http://tg.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://to.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://md.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cv.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yt.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zk.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fo.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gy.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://yx.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xb.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jw.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ws.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ee.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://og.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ok.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aq.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ej.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://tg.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://uq.yuntaijiaju.cn


<!-- 参考信息 -->