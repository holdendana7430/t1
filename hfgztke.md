代发 wailian999

[A06] 字符串转数字
来源：http://nx.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://gs.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ir.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ue.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wu.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mq.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gn.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zs.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pu.newstarts.cn

[A07] 数字转字符串
来源：http://rc.panjiajie.cn

Py:   str(42)
来源：http://dk.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://cz.szsharing.cn

JS:   String(42); (42).toString()
来源：http://cx.shtwfgs.cn

TS:   String(42)
来源：http://de.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bk.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://kv.chemitech.net.cn

Ruby: 42.to_s
来源：http://hp.newstarts.cn

C#:   42.ToString()
来源：http://kb.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://zi.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aw.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wk.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ur.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dm.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sl.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lc.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fm.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jm.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://cy.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lt.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zi.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ua.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xh.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mk.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ae.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nu.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sp.lnxyls.cn

[A10] 生成随机数
来源：http://nt.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://vg.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://tj.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://if.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gn.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://aw.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ib.shtwfgs.cn

Ruby: rand(1..100)
来源：http://ds.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://bz.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://cy.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://dk.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pr.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nw.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lv.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://dh.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ub.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gc.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fd.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://mo.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wh.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cm.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://mv.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://sq.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://yc.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lu.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://hx.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://lh.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://aw.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://ui.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://cy.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://bg.newstarts.cn

TS:   "第一行\n第二行"
来源：http://ce.szsharing.cn

Java: "第一行\n第二行"
来源：http://sy.newstarts.cn

Go:   "第一行\n第二行"
来源：http://zt.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://fd.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://qg.bjjhwx.cn

[A14] 注释写法
来源：http://bc.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://el.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hu.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://jc.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://zn.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pr.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://vm.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tr.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://kz.gzmigu.cn

[A15] 空值判断与默认值
来源：http://lw.shxzskj.cn

Py:   value = data or "默认值"
来源：http://wg.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://fj.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://ob.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://jq.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eb.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://hr.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://hp.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://fs.haigaiapp.cn

[A16] 真假值判断规则
来源：http://pg.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ax.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vq.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ij.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://sx.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gn.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qt.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tj.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vu.huanxung.cn

[A17] 位运算
来源：http://gw.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xl.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hu.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fo.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bn.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xx.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ft.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fw.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://zg.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://ya.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://ou.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rh.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rd.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://du.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uy.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://ej.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://tt.hnjuh.cn

[A19] 交换两个变量
来源：http://hh.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://sa.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xk.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://va.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://fw.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://je.yuexingan06.cn

Go:   a, b = b, a
来源：http://ff.521024.cn

Ruby: a, b = b, a
来源：http://vf.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://xv.asd995.cn

[A20] 读取标准输入
来源：http://up.colortex.cn

Py:   name = input("请输入：")
来源：http://ak.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nl.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dc.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://yh.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://vb.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kz.muxihuayi.cn

Ruby: gets.chomp
来源：http://wq.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://ec.colortex.cn

[A21] 保留指定小数位输出
来源：http://uj.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://nd.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gw.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://hk.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://au.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://il.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ut.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://by.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://hb.gzmigu.cn

[A22] 获取字符串长度
来源：http://hj.hnjuh.cn

Py:   len(s)
来源：http://yx.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fb.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lx.haigaiapp.cn

TS:   s.length
来源：http://sr.shxzskj.cn

Java: s.length()
来源：http://yg.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cz.yuntaijiaju.cn

Ruby: s.length
来源：http://ie.lnxyls.cn

C#:   s.Length
来源：http://wh.szxytkj.cn

[A23] 大小写转换
来源：http://ji.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dx.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rq.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cp.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kt.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pv.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://px.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vu.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ex.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://aj.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://no.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lj.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hn.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sx.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nh.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://jh.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iv.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gv.huanxung.cn

[A25] 字符串比较
来源：http://dn.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://ij.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hs.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wt.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zn.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kf.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mf.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://at.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tg.newstarts.cn

[A26] 类型转换总览
来源：http://mk.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tb.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://be.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mg.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://pb.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rd.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ch.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vr.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ah.szxytkj.cn

================================================================================
来源：http://lh.wgjwhj.cn

B. 流程控制
来源：http://il.521024.cn

================================================================================
来源：http://st.nicolike.cn

[B01] 条件判断 if / else
来源：http://dc.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pr.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gv.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vh.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://co.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cs.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ou.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://od.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://uf.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ty.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lz.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mf.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ph.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ok.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lv.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ux.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ed.yuexingan06.cn

[B03] switch / match / case
来源：http://jp.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ec.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://px.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ni.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vc.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nb.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wj.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ue.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gs.hahajie.cn

[B04] for 计数循环
来源：http://av.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://ev.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pg.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ea.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cb.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vy.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ld.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://al.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hq.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://xq.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://vh.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ka.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gy.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pk.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ae.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://df.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://tq.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mm.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://bs.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tl.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xk.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tn.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ly.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vk.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gz.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ne.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tf.hahajie.cn

[B07] while 循环
来源：http://lq.nszjky.cn

Py:   while i < 10: i += 1
来源：http://at.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vb.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://aq.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://eg.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://gd.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tv.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://zh.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://ck.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://it.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://an.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hj.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://sk.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://nn.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://rx.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xa.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cl.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://ef.haigaiapp.cn

[B09] break 与 continue
来源：http://jg.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ye.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hy.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mg.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cr.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bz.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kg.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cm.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tp.colortex.cn

[B10] 遍历同时拿索引
来源：http://kb.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gc.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://am.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://my.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ll.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ms.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ki.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ul.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jw.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://is.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://df.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://vb.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gi.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xf.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eu.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vb.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://jm.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qv.szxytkj.cn

[B12] 跳出多层循环
来源：http://zl.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://to.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ek.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jo.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hd.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aw.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fp.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ew.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mj.hahajie.cn


<!-- 参考信息 -->