代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rn.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gu.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yj.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://zq.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yt.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tk.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pn.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rb.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xn.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vf.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sk.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ql.lnxyls.cn

[A10] 生成随机数
来源：http://pm.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://sb.szsharing.cn

PHP:  random_int(1, 100);
来源：http://iv.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mw.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cr.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://vm.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vy.hahajie.cn

Ruby: rand(1..100)
来源：http://er.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://ce.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://mb.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://us.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://te.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://iv.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ir.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://yk.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oy.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nx.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ls.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://xa.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zc.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ej.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://yd.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://ga.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://ju.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pd.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://qv.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://yl.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hj.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://jd.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://uv.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://xm.newstarts.cn

TS:   "第一行\n第二行"
来源：http://xq.nszjky.cn

Java: "第一行\n第二行"
来源：http://op.9csxet.cn

Go:   "第一行\n第二行"
来源：http://ki.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://gb.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://fl.huixiangedu.cn

[A14] 注释写法
来源：http://gp.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pg.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fv.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://kn.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://me.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oq.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://aj.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uo.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://gr.gzmigu.cn

[A15] 空值判断与默认值
来源：http://kf.lnxyls.cn

Py:   value = data or "默认值"
来源：http://xv.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://fo.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://sp.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://np.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wp.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://gu.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://te.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://wz.shxzukj.cn

[A16] 真假值判断规则
来源：http://pb.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://aq.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ss.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ll.shtwfgs.cn

TS:   if (!x) {}
来源：http://dh.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gd.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bp.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yz.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fg.nicolike.cn

[A17] 位运算
来源：http://xp.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xl.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fv.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kp.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://as.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eg.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://si.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ew.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jb.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://ff.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://ft.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://rd.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gn.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ck.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://wp.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vw.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://jz.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://gj.hnjuh.cn

[A19] 交换两个变量
来源：http://fr.shxzukj.cn

Py:   a, b = b, a
来源：http://wv.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cf.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://dw.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://mp.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://oi.szsharing.cn

Go:   a, b = b, a
来源：http://cr.huanxung.cn

Ruby: a, b = b, a
来源：http://hm.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://ou.huixiangedu.cn

[A20] 读取标准输入
来源：http://qu.lnxyls.cn

Py:   name = input("请输入：")
来源：http://ou.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xo.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yx.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://fx.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://zn.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sx.muxihuayi.cn

Ruby: gets.chomp
来源：http://bk.9csxet.cn

C#:   Console.ReadLine();
来源：http://ub.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://ya.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://oa.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tc.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://rz.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://em.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://kc.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fl.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://xe.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://fy.shtwfgs.cn

[A22] 获取字符串长度
来源：http://lp.gzmigu.cn

Py:   len(s)
来源：http://eq.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tj.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dh.hahajie.cn

TS:   s.length
来源：http://tk.hahajie.cn

Java: s.length()
来源：http://ou.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://js.hahajie.cn

Ruby: s.length
来源：http://ys.muxihuayi.cn

C#:   s.Length
来源：http://gj.shxzukj.cn

[A23] 大小写转换
来源：http://ui.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jy.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sk.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dp.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yv.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eo.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jb.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zu.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sf.huanxung.cn

[A24] 去除首尾空白
来源：http://xe.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ud.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ew.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ji.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iz.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://un.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://em.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aq.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tk.szsharing.cn

[A25] 字符串比较
来源：http://vm.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://bo.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kc.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lp.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yt.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yt.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cj.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gz.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://px.muxihuayi.cn

[A26] 类型转换总览
来源：http://ri.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uq.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xt.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vb.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://hf.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nd.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ud.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lp.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qa.shxzukj.cn

================================================================================
来源：http://nr.huanxung.cn

B. 流程控制
来源：http://tm.bjjhwx.cn

================================================================================
来源：http://hc.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://ix.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hm.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gq.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rq.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pu.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jy.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uj.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tv.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tx.9csxet.cn

[B02] 多分支 else if / elif
来源：http://mb.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sc.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gv.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ne.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dy.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ow.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gl.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bf.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hd.huixinmuqiang.cn

[B03] switch / match / case
来源：http://nm.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qo.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ai.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yy.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nw.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rd.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yt.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qc.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sc.jianghongdianzi.cn

[B04] for 计数循环
来源：http://qq.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://lr.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qo.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lx.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gc.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ol.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gh.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://xj.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://de.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://cg.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ij.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sk.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ld.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ds.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mp.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bq.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://pm.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://av.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://fe.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ke.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sr.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kz.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kc.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yo.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ah.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oz.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yf.szxytkj.cn

[B07] while 循环
来源：http://xa.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://ja.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ny.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://fo.521024.cn

TS:   while (i < 10) { i++; }
来源：http://ga.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://hw.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://yf.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://io.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://wn.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://xh.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://th.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://pt.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://zw.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://xs.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fh.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dg.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://zt.9csxet.cn

[B09] break 与 continue
来源：http://ra.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bm.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ox.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lz.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fj.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ym.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ca.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://im.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://px.nszjky.cn

[B10] 遍历同时拿索引
来源：http://zk.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bm.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rf.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lk.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wi.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://md.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iu.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wb.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rz.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://dw.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://wn.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://ev.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ac.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ei.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://in.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yn.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://zt.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zi.szxytkj.cn

[B12] 跳出多层循环
来源：http://rc.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cj.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cz.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uk.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cf.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vl.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lp.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zd.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qh.newstarts.cn

[B13] 判断是否为数字
来源：http://vh.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://rz.colortex.cn

PHP:  is_numeric($x)
来源：http://jf.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lt.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://us.521024.cn

Java: x instanceof Number
来源：http://gd.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bv.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://qr.hnjuh.cn

C#:   x is int or double or decimal
来源：http://pu.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://qn.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pt.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://go.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://op.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://ne.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://aq.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dh.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hq.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uc.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://ao.yuntaijiaju.cn

Py:   a and b or not c
来源：http://sj.colortex.cn

PHP:  $a && $b || !$c
来源：http://ln.521024.cn

JS:   a && b || !c
来源：http://rw.bjjhwx.cn

TS:   a && b || !c
来源：http://fb.shtwfgs.cn

Java: a && b || !c
来源：http://hs.huixiangedu.cn


<!-- 参考信息 -->