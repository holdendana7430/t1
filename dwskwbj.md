代发 wailian999

[A06] 字符串转数字
来源：http://ut.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://mw.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oc.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pd.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ss.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xp.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sy.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gr.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gu.wgjwhj.cn

[A07] 数字转字符串
来源：http://sl.huixinmuqiang.cn

Py:   str(42)
来源：http://wy.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://rw.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://lr.muxihuayi.cn

TS:   String(42)
来源：http://mt.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hg.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://kf.wgjwhj.cn

Ruby: 42.to_s
来源：http://xd.haigaiapp.cn

C#:   42.ToString()
来源：http://ho.szsharing.cn

[A08] 取整与四舍五入
来源：http://yu.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uz.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oa.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zy.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ep.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pl.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oe.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qu.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yh.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://ae.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dr.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://id.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nh.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tb.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yp.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://km.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pd.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dk.huanxung.cn

[A10] 生成随机数
来源：http://cu.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://vd.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://ej.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://as.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bf.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://dn.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cr.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://bd.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://oh.asd995.cn

[A11] 条件表达式（三元）
来源：http://kn.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://xt.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ko.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sm.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jk.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://ev.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://br.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pk.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yf.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://kn.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ks.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lg.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://sg.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://fy.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://cc.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://by.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://xu.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://zs.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rd.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://cy.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://rc.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://el.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://bv.nicolike.cn

Java: "第一行\n第二行"
来源：http://jj.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://vr.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://qh.hahajie.cn

C#:   "第一行\n第二行"
来源：http://ij.wgjwhj.cn

[A14] 注释写法
来源：http://gh.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bj.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://aq.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://na.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://nx.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ip.521024.cn

Go:   // 单行；/* 多行 */
来源：http://en.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ft.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://jy.shxzskj.cn

[A15] 空值判断与默认值
来源：http://xm.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://pr.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://hh.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://kv.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://jm.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ak.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://ro.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://uy.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://xf.shxzskj.cn

[A16] 真假值判断规则
来源：http://sc.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sp.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zz.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://je.gzmigu.cn

TS:   if (!x) {}
来源：http://vd.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ik.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ab.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nq.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nt.521024.cn

[A17] 位运算
来源：http://il.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ox.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lc.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aj.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cx.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ds.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bc.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://un.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hq.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://jk.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://nx.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://yh.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ud.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ml.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://pg.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://be.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://ml.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://bp.szsharing.cn

[A19] 交换两个变量
来源：http://oy.521024.cn

Py:   a, b = b, a
来源：http://on.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vf.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://ux.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://wr.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://rj.bjjhwx.cn

Go:   a, b = b, a
来源：http://he.newstarts.cn

Ruby: a, b = b, a
来源：http://cd.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://vr.bookmarksfly.cn

[A20] 读取标准输入
来源：http://qw.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://nc.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hl.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hg.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://az.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://ys.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ia.bjjhwx.cn

Ruby: gets.chomp
来源：http://aw.hnjuh.cn

C#:   Console.ReadLine();
来源：http://qw.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://dn.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://tu.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iv.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://cr.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://qe.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ht.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ld.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://hp.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://sx.nicolike.cn

[A22] 获取字符串长度
来源：http://kt.colortex.cn

Py:   len(s)
来源：http://np.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rt.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tt.colortex.cn

TS:   s.length
来源：http://iz.szxytkj.cn

Java: s.length()
来源：http://vl.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vl.wgjwhj.cn

Ruby: s.length
来源：http://hb.bookmarksfly.cn

C#:   s.Length
来源：http://ha.bjjhwx.cn

[A23] 大小写转换
来源：http://be.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uw.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gf.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pn.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ym.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fr.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pv.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ab.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://um.huixiangedu.cn

[A24] 去除首尾空白
来源：http://qb.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ix.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ej.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ag.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ot.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gl.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://bt.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mn.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://la.szxytkj.cn

[A25] 字符串比较
来源：http://hi.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://xd.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://al.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pq.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oq.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mo.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fh.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mz.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gg.asd995.cn

[A26] 类型转换总览
来源：http://ud.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wc.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dp.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fi.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://xi.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ud.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jl.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://my.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nj.shtwfgs.cn

================================================================================
来源：http://mg.lnxyls.cn

B. 流程控制
来源：http://ne.muxihuayi.cn

================================================================================
来源：http://qk.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://vq.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zi.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ui.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uq.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jk.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ch.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xs.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fe.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rv.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://zs.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zv.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ve.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qv.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ap.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xv.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cp.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pe.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xd.shxzukj.cn

[B03] switch / match / case
来源：http://py.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kf.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://km.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uf.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gq.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tw.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jc.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pa.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ts.yuexingan06.cn

[B04] for 计数循环
来源：http://ez.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://jr.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lw.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kf.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yr.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lv.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xu.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://ov.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fk.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://tt.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ao.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zk.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ie.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ql.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zt.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kg.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://fs.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qb.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://we.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oe.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wq.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iq.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://di.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ta.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vm.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://on.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tn.jctech888.com.cn

[B07] while 循环
来源：http://jx.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://he.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://se.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://ia.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://bq.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://zn.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cf.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://bw.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://lg.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://vp.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://dx.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pe.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://uh.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://iw.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://tx.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://at.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://in.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://gx.wgjwhj.cn

[B09] break 与 continue
来源：http://tj.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wp.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vr.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://di.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rr.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jr.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xd.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gl.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.521024.cn

[B10] 遍历同时拿索引
来源：http://js.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ax.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ke.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://va.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vc.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xi.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eh.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xm.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ba.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://vj.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://uy.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://hy.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zv.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://si.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uy.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dl.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://kb.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bh.haigaiapp.cn

[B12] 跳出多层循环
来源：http://pz.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ta.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tn.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wo.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vx.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qw.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hd.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://un.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qi.asd995.cn


<!-- 参考信息 -->