代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://nb.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wp.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gw.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xk.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dw.bjjhwx.cn

[A07] 数字转字符串
来源：http://ce.szxytkj.cn

Py:   str(42)
来源：http://cu.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://zq.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://lk.yuntaijiaju.cn

TS:   String(42)
来源：http://ky.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wd.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://pv.chemitech.net.cn

Ruby: 42.to_s
来源：http://sq.huixiangedu.cn

C#:   42.ToString()
来源：http://ou.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://ow.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cn.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hc.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ow.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kc.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xc.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://im.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ja.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jh.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://fc.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://me.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://id.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://un.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ks.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://we.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yp.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rr.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ka.huixinmuqiang.cn

[A10] 生成随机数
来源：http://lg.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://jl.colortex.cn

PHP:  random_int(1, 100);
来源：http://eu.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kh.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fd.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://iz.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jj.hahajie.cn

Ruby: rand(1..100)
来源：http://yc.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://lr.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://sw.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://fz.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pe.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qo.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qb.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://pt.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wd.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ig.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mj.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://nu.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pk.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fh.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://we.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://un.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://rw.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ry.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://ny.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://ex.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oc.9csxet.cn

Py:   "第一行\n第二行"
来源：http://sr.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://by.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://yv.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://yc.521024.cn

Java: "第一行\n第二行"
来源：http://uc.newstarts.cn

Go:   "第一行\n第二行"
来源：http://yr.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://gq.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://ed.9csxet.cn

[A14] 注释写法
来源：http://wp.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hk.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nv.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://kx.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://my.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sd.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://iv.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://al.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://xe.newstarts.cn

[A15] 空值判断与默认值
来源：http://lw.panjiajie.cn

Py:   value = data or "默认值"
来源：http://vc.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://zy.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://lj.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://vc.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wk.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://ap.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://re.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://ic.gzmigu.cn

[A16] 真假值判断规则
来源：http://vp.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mu.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zt.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uc.newstarts.cn

TS:   if (!x) {}
来源：http://xg.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pd.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://si.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qy.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://re.shxzskj.cn

[A17] 位运算
来源：http://px.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bg.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tp.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jm.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ah.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mx.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jo.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mf.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://pp.asd995.cn

Py:   ord("A"); chr(65)
来源：http://fd.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://rd.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oo.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bs.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://km.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yn.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://hz.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://jg.nszjky.cn

[A19] 交换两个变量
来源：http://cf.521024.cn

Py:   a, b = b, a
来源：http://cl.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qi.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://ex.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://ky.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://fz.gzmigu.cn

Go:   a, b = b, a
来源：http://on.nicolike.cn

Ruby: a, b = b, a
来源：http://sp.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://cz.panjiajie.cn

[A20] 读取标准输入
来源：http://zu.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://nr.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://va.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gw.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://vk.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://zf.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mj.hnjuh.cn

Ruby: gets.chomp
来源：http://gw.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://fa.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://bl.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://gr.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jv.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://lr.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://np.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://kz.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dj.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://bo.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://qg.lnxyls.cn

[A22] 获取字符串长度
来源：http://bz.haigaiapp.cn

Py:   len(s)
来源：http://dg.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aw.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mu.hahajie.cn

TS:   s.length
来源：http://vu.jianghongdianzi.cn

Java: s.length()
来源：http://ir.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pc.huixinmuqiang.cn

Ruby: s.length
来源：http://ak.huixiangedu.cn

C#:   s.Length
来源：http://ah.yuntaijiaju.cn

[A23] 大小写转换
来源：http://hv.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uq.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cx.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://to.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ja.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qc.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tj.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://np.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zy.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://et.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ij.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gh.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rv.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zv.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jm.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://xm.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ca.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nd.nicolike.cn

[A25] 字符串比较
来源：http://ic.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://mi.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zo.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ok.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zq.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xi.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wl.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ej.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jt.panjiajie.cn

[A26] 类型转换总览
来源：http://ag.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ac.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xy.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jb.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://ma.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://li.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yc.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uv.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mw.bookmarksfly.cn

================================================================================
来源：http://rq.huixiangedu.cn

B. 流程控制
来源：http://er.szxytkj.cn

================================================================================
来源：http://jv.szxytkj.cn

[B01] 条件判断 if / else
来源：http://dr.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sw.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cc.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pa.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://of.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gg.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zc.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://em.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wu.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://sk.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pc.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fu.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rj.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rd.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cq.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://er.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nt.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xz.hahajie.cn

[B03] switch / match / case
来源：http://wb.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gf.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bv.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ni.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nf.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lx.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zk.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ob.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bi.bjjhwx.cn

[B04] for 计数循环
来源：http://rf.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://yb.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ic.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uq.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ba.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aj.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ec.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://jq.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nn.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://hp.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://ni.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://za.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kd.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qf.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dm.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vo.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://by.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qn.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://kv.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ai.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sn.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jg.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://to.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vp.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ps.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mg.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pd.szxytkj.cn

[B07] while 循环
来源：http://sz.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://rd.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kp.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://nb.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://aj.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://vn.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jq.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://vl.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://eg.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://vc.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://qi.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tv.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://nt.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://rq.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://fo.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ie.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yn.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://vi.lnxyls.cn

[B09] break 与 continue
来源：http://ma.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dy.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xf.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wb.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fw.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://la.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kk.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wx.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://su.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://ye.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eg.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yp.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tm.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kd.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fx.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://us.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ms.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gy.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://jl.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://uk.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://nb.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hu.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ej.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jr.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yn.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://vv.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ky.szxytkj.cn

[B12] 跳出多层循环
来源：http://eb.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pg.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xs.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://if.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kd.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://co.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zd.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zs.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lz.szxytkj.cn

[B13] 判断是否为数字
来源：http://kp.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://jn.panjiajie.cn

PHP:  is_numeric($x)
来源：http://rd.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ph.shtwfgs.cn


<!-- 参考信息 -->