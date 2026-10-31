代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kz.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xp.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://id.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xh.lnxyls.cn

[A10] 生成随机数
来源：http://mc.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://qc.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://dl.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mb.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zo.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://kc.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kz.hnjuh.cn

Ruby: rand(1..100)
来源：http://na.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://aa.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://xx.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://to.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xu.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nf.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sx.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://aw.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oo.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cy.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xk.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://ut.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oq.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://up.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://aj.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://vj.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://tb.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xk.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://br.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://et.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eu.asd995.cn

Py:   "第一行\n第二行"
来源：http://jn.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://rz.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://pp.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://lg.hahajie.cn

Java: "第一行\n第二行"
来源：http://qv.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://bq.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://ej.newstarts.cn

C#:   "第一行\n第二行"
来源：http://zq.jctech888.com.cn

[A14] 注释写法
来源：http://am.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oe.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vo.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://va.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://ih.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lc.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://zi.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rt.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://ps.huanxung.cn

[A15] 空值判断与默认值
来源：http://tk.hnjuh.cn

Py:   value = data or "默认值"
来源：http://av.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://cz.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://mf.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://ej.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://la.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://kk.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://bv.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://uz.jctech888.com.cn

[A16] 真假值判断规则
来源：http://aq.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qu.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hv.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ul.wgjwhj.cn

TS:   if (!x) {}
来源：http://ae.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nw.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wb.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tb.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vs.newstarts.cn

[A17] 位运算
来源：http://kb.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ra.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wt.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://js.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jz.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ga.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xy.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bz.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://oe.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://yr.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://xi.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fq.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ms.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://eu.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uj.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://or.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://am.521024.cn

[A19] 交换两个变量
来源：http://ho.huanxung.cn

Py:   a, b = b, a
来源：http://ky.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mw.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://yh.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://wh.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://ra.panjiajie.cn

Go:   a, b = b, a
来源：http://lm.szxytkj.cn

Ruby: a, b = b, a
来源：http://if.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://sr.szsharing.cn

[A20] 读取标准输入
来源：http://ve.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://sj.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kj.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ck.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://qq.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://rr.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://er.panjiajie.cn

Ruby: gets.chomp
来源：http://mo.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://km.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://ot.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://pa.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yw.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://kg.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://nz.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://rs.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lc.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://ig.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://yg.szsharing.cn

[A22] 获取字符串长度
来源：http://jy.521024.cn

Py:   len(s)
来源：http://ka.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nz.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cg.shtwfgs.cn

TS:   s.length
来源：http://kv.szsharing.cn

Java: s.length()
来源：http://ag.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yt.shxzukj.cn

Ruby: s.length
来源：http://mq.asd995.cn

C#:   s.Length
来源：http://cl.shtwfgs.cn

[A23] 大小写转换
来源：http://uh.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hk.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uk.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jy.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://va.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://or.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mu.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hr.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ta.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://ib.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ot.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gi.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kx.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jm.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lm.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://lo.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lf.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://op.521024.cn

[A25] 字符串比较
来源：http://ux.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://kl.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cr.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bq.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mm.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tr.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wd.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ka.huanxung.cn

[A26] 类型转换总览
来源：http://mj.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vu.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gk.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fb.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://mb.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ft.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dt.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ab.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vi.colortex.cn

================================================================================
来源：http://vm.chemitech.net.cn

B. 流程控制
来源：http://ey.szsharing.cn

================================================================================
来源：http://xv.asd995.cn

[B01] 条件判断 if / else
来源：http://ti.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uj.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yq.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oj.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rc.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ss.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://du.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fk.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aj.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://pb.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://no.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zb.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ht.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://og.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cz.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uc.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gk.9csxet.cn

[B03] switch / match / case
来源：http://gn.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bs.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qv.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bx.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ga.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iq.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zt.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zo.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://co.lnxyls.cn

[B04] for 计数循环
来源：http://uq.colortex.cn

Py:   for i in range(10): print(i)
来源：http://kk.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aq.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gt.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ng.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kc.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fd.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://dl.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ne.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://iw.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://ui.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://on.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ks.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oy.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cf.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zx.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://ji.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ub.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://mt.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nz.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gs.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ki.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ui.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ra.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ey.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wv.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cx.nszjky.cn

[B07] while 循环
来源：http://ew.9csxet.cn

Py:   while i < 10: i += 1
来源：http://mr.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nu.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://lp.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://kn.colortex.cn

Java: while (i < 10) { i++; }
来源：http://td.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oc.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://yo.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://zl.colortex.cn

[B08] do-while（至少执行一次）
来源：http://bx.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://pw.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bv.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://of.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://mi.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://sa.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zp.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pn.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://yw.colortex.cn

[B09] break 与 continue
来源：http://ro.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://go.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ud.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bf.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dg.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cz.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fa.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sx.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wb.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://rs.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rn.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dj.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ww.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wi.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sr.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ql.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zl.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dl.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://mu.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://gy.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://qz.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tu.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ux.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://co.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lj.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://zj.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hc.haigaiapp.cn

[B12] 跳出多层循环
来源：http://sp.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bz.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mk.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gc.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wz.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vb.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vp.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bv.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mc.hnjuh.cn

[B13] 判断是否为数字
来源：http://rs.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://ph.hahajie.cn

PHP:  is_numeric($x)
来源：http://us.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nt.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://az.huixinmuqiang.cn

Java: x instanceof Number
来源：http://tr.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jn.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://cf.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://zl.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://il.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xf.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zz.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://ju.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://mr.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ss.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kg.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vt.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dr.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://ku.shxzukj.cn

Py:   a and b or not c
来源：http://mh.huanxung.cn

PHP:  $a && $b || !$c
来源：http://ay.jianghongdianzi.cn

JS:   a && b || !c
来源：http://ru.yuexingan06.cn

TS:   a && b || !c
来源：http://at.panjiajie.cn

Java: a && b || !c
来源：http://jd.panjiajie.cn

Go:   a && b || !c
来源：http://zu.hahajie.cn

Ruby: a && b || !c
来源：http://ov.asd995.cn

C#:   a && b || !c
来源：http://gf.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tm.newstarts.cn

Py:   if not data: return
来源：http://yr.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://fr.haigaiapp.cn

JS:   if (!data) return;
来源：http://ps.haigaiapp.cn

TS:   if (!data) return;
来源：http://yh.szsharing.cn


<!-- 参考信息 -->