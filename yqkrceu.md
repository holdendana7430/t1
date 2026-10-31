代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ct.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://os.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tw.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jj.panjiajie.cn

[A10] 生成随机数
来源：http://fc.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://sx.huanxung.cn

PHP:  random_int(1, 100);
来源：http://bo.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ak.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zl.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://cq.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oa.jctech888.com.cn

Ruby: rand(1..100)
来源：http://xt.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://qe.9csxet.cn

[A11] 条件表达式（三元）
来源：http://ci.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://zr.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sw.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cb.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://or.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://tc.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lu.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ql.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ux.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://of.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://av.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bh.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://ia.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://kv.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://pu.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yq.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://eg.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://md.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vh.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://gd.521024.cn

PHP:  "第一行\n第二行"
来源：http://nr.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://ms.nicolike.cn

TS:   "第一行\n第二行"
来源：http://fo.asd995.cn

Java: "第一行\n第二行"
来源：http://kk.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://hv.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://jt.asd995.cn

C#:   "第一行\n第二行"
来源：http://vf.szxytkj.cn

[A14] 注释写法
来源：http://rx.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ai.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sy.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://ug.521024.cn

TS:   // 单行；/* 多行 */
来源：http://ys.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tf.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://ki.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qc.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://at.szxytkj.cn

[A15] 空值判断与默认值
来源：http://vf.colortex.cn

Py:   value = data or "默认值"
来源：http://im.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://jp.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://nx.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://ai.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ba.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://ym.newstarts.cn

Ruby: value = data || "默认值"
来源：http://ee.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://zw.521024.cn

[A16] 真假值判断规则
来源：http://gw.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://el.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dw.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ez.chemitech.net.cn

TS:   if (!x) {}
来源：http://xd.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://to.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mc.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tq.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ks.asd995.cn

[A17] 位运算
来源：http://nk.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tf.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tw.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nl.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ly.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wn.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nk.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qz.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://en.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://yb.521024.cn

Py:   ord("A"); chr(65)
来源：http://py.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://tc.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pb.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hb.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://kl.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dd.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://oo.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://xb.shtwfgs.cn

[A19] 交换两个变量
来源：http://or.szsharing.cn

Py:   a, b = b, a
来源：http://qo.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ex.asd995.cn

JS:   [a, b] = [b, a];
来源：http://eq.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://jq.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://ch.bookmarksfly.cn

Go:   a, b = b, a
来源：http://qo.szxytkj.cn

Ruby: a, b = b, a
来源：http://bn.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://cn.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://lg.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://dr.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ab.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gv.asd995.cn

TS:   // Node.js：readline 模块
来源：http://bk.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://qx.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cl.shxzskj.cn

Ruby: gets.chomp
来源：http://as.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://mb.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://ji.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://wr.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mt.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://gj.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://ag.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ij.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gn.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://kl.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://bw.lnxyls.cn

[A22] 获取字符串长度
来源：http://si.9csxet.cn

Py:   len(s)
来源：http://db.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qv.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ks.wgjwhj.cn

TS:   s.length
来源：http://es.521024.cn

Java: s.length()
来源：http://jc.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nj.huixinmuqiang.cn

Ruby: s.length
来源：http://kq.panjiajie.cn

C#:   s.Length
来源：http://ng.hahajie.cn

[A23] 大小写转换
来源：http://yc.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://js.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bn.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nq.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tt.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ry.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zp.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ot.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ly.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://mc.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lk.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qt.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fw.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tm.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tc.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://ro.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ct.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gj.nszjky.cn

[A25] 字符串比较
来源：http://ln.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://ae.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jn.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pz.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rw.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kz.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sc.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fw.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fw.hahajie.cn

[A26] 类型转换总览
来源：http://fe.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pp.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lp.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mj.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://yi.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ri.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pk.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zy.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ia.shxzskj.cn

================================================================================
来源：http://bv.szxytkj.cn

B. 流程控制
来源：http://hx.huixiangedu.cn

================================================================================
来源：http://dj.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://ee.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://io.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://co.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fr.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jk.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ic.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fc.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://on.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ew.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://da.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oh.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fy.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hk.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eo.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yr.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://io.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rg.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fc.szxytkj.cn

[B03] switch / match / case
来源：http://ly.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ev.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jp.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ds.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qs.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tu.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qp.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://am.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mf.haigaiapp.cn

[B04] for 计数循环
来源：http://jl.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://an.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xy.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lm.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wj.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iq.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ig.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ve.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hp.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://fh.9csxet.cn

Py:   for item in arr: print(item)
来源：http://qc.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jl.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ez.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ze.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ll.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://az.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://qc.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wt.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://pm.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sf.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ce.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mo.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dm.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ho.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lr.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ho.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qb.hnjuh.cn

[B07] while 循环
来源：http://lu.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://bl.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sw.521024.cn

JS:   while (i < 10) { i++; }
来源：http://ve.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://da.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://lw.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wo.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://gl.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://va.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ye.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ts.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vs.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://ll.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://vu.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://wh.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://re.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://et.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://un.asd995.cn

[B09] break 与 continue
来源：http://mt.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ri.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bg.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ig.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://en.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oq.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kv.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zw.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kv.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://en.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vv.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oe.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sy.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fd.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cq.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mg.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jr.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hm.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://oo.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://ax.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://wt.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uh.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zz.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mm.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fq.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://qb.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uy.szsharing.cn

[B12] 跳出多层循环
来源：http://zl.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hv.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://et.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nn.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ud.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yv.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gq.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qf.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jt.nszjky.cn

[B13] 判断是否为数字
来源：http://fb.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://tw.hahajie.cn

PHP:  is_numeric($x)
来源：http://kc.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lq.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kd.521024.cn

Java: x instanceof Number
来源：http://yj.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ot.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://nh.hnjuh.cn

C#:   x is int or double or decimal
来源：http://qn.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://re.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lf.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hx.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://eg.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://am.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://up.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zi.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eb.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://im.asd995.cn

[B15] 布尔运算与取反
来源：http://nr.hnjuh.cn

Py:   a and b or not c
来源：http://he.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://zm.muxihuayi.cn

JS:   a && b || !c
来源：http://nr.nicolike.cn

TS:   a && b || !c
来源：http://ya.shxzskj.cn

Java: a && b || !c
来源：http://ur.yuntaijiaju.cn

Go:   a && b || !c
来源：http://tj.huixiangedu.cn

Ruby: a && b || !c
来源：http://dm.bjjhwx.cn

C#:   a && b || !c
来源：http://kd.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lv.newstarts.cn

Py:   if not data: return
来源：http://pv.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://dv.colortex.cn

JS:   if (!data) return;
来源：http://tv.huixiangedu.cn

TS:   if (!data) return;
来源：http://ke.huanxung.cn


<!-- 参考信息 -->