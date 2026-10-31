代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://al.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://la.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://op.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dq.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wy.shtwfgs.cn

[A07] 数字转字符串
来源：http://ke.newstarts.cn

Py:   str(42)
来源：http://vv.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://zz.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://fe.colortex.cn

TS:   String(42)
来源：http://kd.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nu.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://ay.shxzukj.cn

Ruby: 42.to_s
来源：http://kq.gzmigu.cn

C#:   42.ToString()
来源：http://tm.shxzskj.cn

[A08] 取整与四舍五入
来源：http://my.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://on.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xv.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vh.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://li.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fr.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fs.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zl.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ag.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://ou.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cd.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dh.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dx.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lz.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zi.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jg.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://io.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tw.hahajie.cn

[A10] 生成随机数
来源：http://zr.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://og.asd995.cn

PHP:  random_int(1, 100);
来源：http://zo.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dw.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://va.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://hd.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dj.nszjky.cn

Ruby: rand(1..100)
来源：http://ky.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://fd.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://sw.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://yl.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://px.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gs.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xu.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://wr.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xu.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iw.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://js.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://rz.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jc.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://np.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://kb.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://zv.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://ig.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zx.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://ft.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://ai.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tk.colortex.cn

Py:   "第一行\n第二行"
来源：http://tn.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://vf.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://vd.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://xf.nszjky.cn

Java: "第一行\n第二行"
来源：http://go.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://vl.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://iv.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://dn.huixinmuqiang.cn

[A14] 注释写法
来源：http://mt.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ks.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vq.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://mo.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://ya.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zj.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://oj.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uh.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://hf.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://ko.newstarts.cn

Py:   value = data or "默认值"
来源：http://pt.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://he.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://oo.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://xq.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eg.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://mw.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://pm.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://wh.asd995.cn

[A16] 真假值判断规则
来源：http://cz.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wq.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hc.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jo.huixiangedu.cn

TS:   if (!x) {}
来源：http://il.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://in.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bu.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ar.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ht.haigaiapp.cn

[A17] 位运算
来源：http://zx.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yi.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ub.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://os.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sc.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mz.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vk.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uz.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://oo.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://mw.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://gq.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xs.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ox.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://sj.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ro.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://oy.colortex.cn

C#:   (int)'A'; (char)65
来源：http://ev.shxzukj.cn

[A19] 交换两个变量
来源：http://ph.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://yk.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vm.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://an.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://ms.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://rg.wgjwhj.cn

Go:   a, b = b, a
来源：http://ga.chemitech.net.cn

Ruby: a, b = b, a
来源：http://ec.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://sm.hahajie.cn

[A20] 读取标准输入
来源：http://sw.nszjky.cn

Py:   name = input("请输入：")
来源：http://be.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hj.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pa.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://xq.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://aj.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qp.szxytkj.cn

Ruby: gets.chomp
来源：http://ec.9csxet.cn

C#:   Console.ReadLine();
来源：http://hv.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://fk.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://oo.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yg.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://cr.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://zh.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://zp.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pi.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://zo.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://rp.haigaiapp.cn

[A22] 获取字符串长度
来源：http://ks.nszjky.cn

Py:   len(s)
来源：http://ns.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://re.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zs.szsharing.cn

TS:   s.length
来源：http://ui.asd995.cn

Java: s.length()
来源：http://no.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fj.bjjhwx.cn

Ruby: s.length
来源：http://ut.nicolike.cn

C#:   s.Length
来源：http://bi.newstarts.cn

[A23] 大小写转换
来源：http://jj.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tb.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ft.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sw.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xd.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zc.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nr.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://un.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ul.haigaiapp.cn

[A24] 去除首尾空白
来源：http://ly.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cy.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ix.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ak.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nl.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fo.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://qk.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xx.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ep.nszjky.cn

[A25] 字符串比较
来源：http://sz.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://yb.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xb.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wc.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bt.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bd.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jq.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bf.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yf.shxzskj.cn

[A26] 类型转换总览
来源：http://uy.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hm.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ol.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ly.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://hq.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zr.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vv.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vp.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fu.shtwfgs.cn

================================================================================
来源：http://af.szsharing.cn

B. 流程控制
来源：http://az.huixiangedu.cn

================================================================================
来源：http://sg.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://vq.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nw.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vd.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lg.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ua.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rf.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ub.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ql.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ts.nszjky.cn

[B02] 多分支 else if / elif
来源：http://sr.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pk.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gv.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sw.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gc.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qe.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ow.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yf.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gq.gzmigu.cn

[B03] switch / match / case
来源：http://wo.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://od.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jd.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jn.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gp.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wi.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vv.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kh.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pd.colortex.cn

[B04] for 计数循环
来源：http://bf.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://ri.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ah.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cs.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nr.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yh.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gu.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://gn.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://um.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://un.nicolike.cn

Py:   for item in arr: print(item)
来源：http://lj.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ii.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bs.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ex.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wf.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uo.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://vk.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rw.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://zw.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qj.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ie.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://is.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qh.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ny.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aa.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mj.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xf.colortex.cn

[B07] while 循环
来源：http://qs.9csxet.cn

Py:   while i < 10: i += 1
来源：http://uq.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xb.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://ni.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://hq.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://ks.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jv.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://lv.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://zx.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://np.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://jz.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zl.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://mf.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://mz.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://dr.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zx.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://du.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://rr.asd995.cn

[B09] break 与 continue
来源：http://hw.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rn.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://md.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pv.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ji.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zg.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rt.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vm.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vj.colortex.cn

[B10] 遍历同时拿索引
来源：http://hu.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fk.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ps.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://of.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ng.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nc.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wg.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ze.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ae.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://xh.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://pq.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://yf.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://as.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ux.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nc.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tx.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://ky.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pd.szxytkj.cn

[B12] 跳出多层循环
来源：http://tw.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bj.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pb.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rn.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qc.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qj.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qr.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ef.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xi.wgjwhj.cn

[B13] 判断是否为数字
来源：http://uc.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://pl.hnjuh.cn

PHP:  is_numeric($x)
来源：http://ua.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cu.shxzukj.cn


<!-- 参考信息 -->