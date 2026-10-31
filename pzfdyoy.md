代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://sf.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://jr.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ie.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://dt.newstarts.cn

[A06] 字符串转数字
来源：http://cw.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://en.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://td.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fd.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ux.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ek.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cz.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ej.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lz.nicolike.cn

[A07] 数字转字符串
来源：http://ni.chemitech.net.cn

Py:   str(42)
来源：http://lg.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://mn.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://hj.huanxung.cn

TS:   String(42)
来源：http://ov.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://iu.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://nd.asd995.cn

Ruby: 42.to_s
来源：http://lb.yuexingan06.cn

C#:   42.ToString()
来源：http://kq.nszjky.cn

[A08] 取整与四舍五入
来源：http://xd.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yh.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qp.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wq.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tj.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jk.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zu.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kh.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vj.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://mn.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ip.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kl.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://in.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vf.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rz.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ef.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hv.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ua.jctech888.com.cn

[A10] 生成随机数
来源：http://bn.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://sh.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://fa.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gg.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ax.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://oi.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://al.lnxyls.cn

Ruby: rand(1..100)
来源：http://gy.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://rd.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://hl.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://oo.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uu.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jl.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hf.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://ez.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pk.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jz.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kf.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://xl.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nk.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ue.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://pz.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://mc.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://nm.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lc.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://wq.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://qa.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lu.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://xe.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://ts.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://ss.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://xg.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://fb.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://dw.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://sp.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://pn.9csxet.cn

[A14] 注释写法
来源：http://rk.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sg.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ts.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://eh.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://kd.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kj.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://sx.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xo.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://sm.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://dn.colortex.cn

Py:   value = data or "默认值"
来源：http://zw.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://mw.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://rd.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://lf.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xr.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://wy.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://fb.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://xt.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://qb.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rl.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gy.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wb.szxytkj.cn

TS:   if (!x) {}
来源：http://lr.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sf.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ji.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bp.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://os.jianghongdianzi.cn

[A17] 位运算
来源：http://rc.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gs.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xz.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yt.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oq.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nt.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gf.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ve.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://wo.colortex.cn

Py:   ord("A"); chr(65)
来源：http://hr.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://kq.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gw.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zi.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://tc.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yh.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://gg.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://xk.asd995.cn

[A19] 交换两个变量
来源：http://hg.muxihuayi.cn

Py:   a, b = b, a
来源：http://is.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dh.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://fx.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://vq.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://ff.521024.cn

Go:   a, b = b, a
来源：http://tx.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://pp.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://xt.newstarts.cn

[A20] 读取标准输入
来源：http://lg.shxzskj.cn

Py:   name = input("请输入：")
来源：http://hl.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fa.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yo.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://rj.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://az.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hv.hahajie.cn

Ruby: gets.chomp
来源：http://uo.nicolike.cn

C#:   Console.ReadLine();
来源：http://aw.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://hf.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://jp.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sq.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://zo.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://ej.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://or.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gm.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://lb.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://lv.newstarts.cn

[A22] 获取字符串长度
来源：http://ke.haigaiapp.cn

Py:   len(s)
来源：http://jp.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qn.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wz.huanxung.cn

TS:   s.length
来源：http://tg.panjiajie.cn

Java: s.length()
来源：http://rn.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fe.shxzukj.cn

Ruby: s.length
来源：http://bq.shtwfgs.cn

C#:   s.Length
来源：http://ey.haigaiapp.cn

[A23] 大小写转换
来源：http://yu.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ha.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gs.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ie.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fm.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gz.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zy.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ns.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sj.nicolike.cn

[A24] 去除首尾空白
来源：http://tt.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ds.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lq.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sv.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aj.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uy.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://ei.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ey.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ym.jctech888.com.cn

[A25] 字符串比较
来源：http://gd.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://xo.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rd.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vj.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tl.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fd.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tx.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tu.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mq.lnxyls.cn

[A26] 类型转换总览
来源：http://dq.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uk.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yw.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://je.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://xf.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qw.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xx.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rt.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zs.huixiangedu.cn

================================================================================
来源：http://hd.bookmarksfly.cn

B. 流程控制
来源：http://sd.gzmigu.cn

================================================================================
来源：http://xl.shxzukj.cn

[B01] 条件判断 if / else
来源：http://wg.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://of.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ki.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pn.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fm.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mk.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ak.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ky.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rp.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://qv.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jt.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gm.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xz.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wu.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yt.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fs.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wx.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vq.bookmarksfly.cn

[B03] switch / match / case
来源：http://zu.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kz.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kw.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qz.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bh.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aa.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ef.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lg.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uo.haigaiapp.cn

[B04] for 计数循环
来源：http://lb.521024.cn

Py:   for i in range(10): print(i)
来源：http://zq.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aq.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tp.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yg.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tz.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hf.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://cj.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://af.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://jo.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://ag.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oy.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dq.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://is.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ka.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ie.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://wg.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://np.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://aj.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://du.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kf.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lv.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://un.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uu.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pt.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mm.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gt.nszjky.cn

[B07] while 循环
来源：http://cf.szsharing.cn

Py:   while i < 10: i += 1
来源：http://ys.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hl.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://ze.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://lr.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://vu.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://py.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://tz.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://jj.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://wh.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://dw.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uo.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://dp.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://xb.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://pr.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://es.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cw.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://bz.bjjhwx.cn

[B09] break 与 continue
来源：http://yq.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jz.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kg.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eu.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://el.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qz.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ob.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ph.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lf.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://vf.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://em.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://my.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dm.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ky.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fq.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ui.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://he.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wl.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://fc.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://wi.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://ot.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dv.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dx.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jl.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cu.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://gq.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jc.jctech888.com.cn

[B12] 跳出多层循环
来源：http://pa.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ul.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ow.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cm.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ag.newstarts.cn


<!-- 参考信息 -->