代发 wailian999

[A10] 生成随机数
来源：http://wq.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://by.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://rv.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://re.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dr.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://jy.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vz.panjiajie.cn

Ruby: rand(1..100)
来源：http://ri.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://ee.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://qg.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://xu.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gs.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zp.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yc.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://xx.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qh.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ve.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ln.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://fb.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://td.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sj.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://ia.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://tf.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://ff.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ze.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://fb.521024.cn

C#:   $"Hello, {name}!"
来源：http://um.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mi.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://vp.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://dd.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://bq.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://pn.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://zv.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://rn.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://di.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://iu.szsharing.cn

[A14] 注释写法
来源：http://yr.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xl.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lo.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://mt.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://kl.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iq.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://ye.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://po.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://ms.panjiajie.cn

[A15] 空值判断与默认值
来源：http://cb.asd995.cn

Py:   value = data or "默认值"
来源：http://te.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://rv.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://fw.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://qr.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://na.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://tg.nicolike.cn

Ruby: value = data || "默认值"
来源：http://zt.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://eb.szsharing.cn

[A16] 真假值判断规则
来源：http://rc.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fa.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yl.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ku.muxihuayi.cn

TS:   if (!x) {}
来源：http://xy.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qg.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yk.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ll.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xl.hnjuh.cn

[A17] 位运算
来源：http://rh.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rx.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pm.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mx.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ui.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rt.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gf.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fj.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sk.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://he.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://xq.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://gm.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kl.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bg.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://dn.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ly.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://lo.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://vd.szxytkj.cn

[A19] 交换两个变量
来源：http://wi.asd995.cn

Py:   a, b = b, a
来源：http://ec.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fi.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://mm.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://jn.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://vq.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://tt.chemitech.net.cn

Ruby: a, b = b, a
来源：http://tp.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://lz.colortex.cn

[A20] 读取标准输入
来源：http://pa.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://hz.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ck.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wp.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://rd.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://oq.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sw.muxihuayi.cn

Ruby: gets.chomp
来源：http://kw.nszjky.cn

C#:   Console.ReadLine();
来源：http://ec.hahajie.cn

[A21] 保留指定小数位输出
来源：http://vl.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://gc.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ll.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://tc.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://uk.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://rw.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gz.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://pv.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://id.nszjky.cn

[A22] 获取字符串长度
来源：http://ps.haigaiapp.cn

Py:   len(s)
来源：http://ti.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fw.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bw.szsharing.cn

TS:   s.length
来源：http://ij.yuntaijiaju.cn

Java: s.length()
来源：http://ro.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://if.bookmarksfly.cn

Ruby: s.length
来源：http://nw.hahajie.cn

C#:   s.Length
来源：http://je.huixiangedu.cn

[A23] 大小写转换
来源：http://az.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://em.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oc.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kn.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://od.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sd.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xm.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pj.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rj.shxzskj.cn

[A24] 去除首尾空白
来源：http://pp.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ng.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ug.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wq.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pw.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nl.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://qs.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ea.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zp.huixinmuqiang.cn

[A25] 字符串比较
来源：http://gc.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://xu.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ol.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pd.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nm.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bx.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hw.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kd.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://da.asd995.cn

[A26] 类型转换总览
来源：http://sq.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rp.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ao.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ai.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://qc.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wo.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kh.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xy.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ud.shxzskj.cn

================================================================================
来源：http://di.shxzskj.cn

B. 流程控制
来源：http://wt.bookmarksfly.cn

================================================================================
来源：http://zi.huanxung.cn

[B01] 条件判断 if / else
来源：http://xf.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ch.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ka.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iw.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ac.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://km.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qx.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wk.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rd.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://bn.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ls.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ol.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://io.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gc.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://me.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fx.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.haigaiapp.cn

[B03] switch / match / case
来源：http://jr.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ut.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pw.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yf.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ii.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rs.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ep.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wn.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uy.shxzukj.cn

[B04] for 计数循环
来源：http://qm.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://yi.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ed.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fv.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://de.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cy.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lv.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://rz.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vh.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://hv.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://oa.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kv.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ga.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uq.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gq.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bk.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://ze.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yc.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://sw.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ex.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rh.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://st.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mz.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tu.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wf.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pc.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uk.nicolike.cn

[B07] while 循环
来源：http://lo.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://as.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tj.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://st.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://mn.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://ye.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://za.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://ca.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://kr.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://aa.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://ol.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ob.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://im.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://gr.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://nn.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uf.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sw.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://jx.shxzskj.cn

[B09] break 与 continue
来源：http://jv.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ml.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vd.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mp.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qz.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cn.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bc.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://on.hahajie.cn

[B10] 遍历同时拿索引
来源：http://xg.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ih.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mw.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zq.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fe.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ab.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ji.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dr.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://im.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://fe.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://dg.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://ok.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nm.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hd.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fp.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qx.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://ul.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gd.shxzskj.cn

[B12] 跳出多层循环
来源：http://zr.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://et.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zr.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vn.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nk.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lm.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nq.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ta.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vj.9csxet.cn

[B13] 判断是否为数字
来源：http://ch.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://kt.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://lv.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eo.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zm.jctech888.com.cn

Java: x instanceof Number
来源：http://il.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mf.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://sg.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://dt.9csxet.cn

[B14] 判断值是否在集合内
来源：http://dk.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tx.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yc.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://ou.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://ik.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ht.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wa.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dv.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fw.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://ah.bjjhwx.cn

Py:   a and b or not c
来源：http://kd.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://pk.colortex.cn

JS:   a && b || !c
来源：http://so.bjjhwx.cn

TS:   a && b || !c
来源：http://zm.yuntaijiaju.cn

Java: a && b || !c
来源：http://ys.bjjhwx.cn

Go:   a && b || !c
来源：http://lw.huanxung.cn

Ruby: a && b || !c
来源：http://ft.gzmigu.cn

C#:   a && b || !c
来源：http://hx.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://in.9csxet.cn

Py:   if not data: return
来源：http://yd.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://uc.bjjhwx.cn

JS:   if (!data) return;
来源：http://mi.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://xj.nicolike.cn

Java: if (data == null) return;
来源：http://it.9csxet.cn

Go:   if data == nil { return }
来源：http://kr.9csxet.cn

Ruby: return if data.nil?
来源：http://qz.shxzukj.cn

C#:   if (data == null) return;
来源：http://df.hnjuh.cn


<!-- 参考信息 -->