代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://ho.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://ha.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://eg.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://re.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rm.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sz.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://of.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kr.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aj.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wh.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://dt.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://le.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ay.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://md.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://wx.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://mw.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ig.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://vm.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://ni.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gl.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://bi.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://ez.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://zp.521024.cn

TS:   "第一行\n第二行"
来源：http://dq.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://qp.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://ts.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://az.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://rb.521024.cn

[A14] 注释写法
来源：http://qu.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ny.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cj.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://ld.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://ze.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rk.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://hm.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hr.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://nb.lnxyls.cn

[A15] 空值判断与默认值
来源：http://wo.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://ez.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://vh.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://qv.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://xa.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ef.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://bq.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://df.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://zl.chemitech.net.cn

[A16] 真假值判断规则
来源：http://iz.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cr.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lh.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cv.yuexingan06.cn

TS:   if (!x) {}
来源：http://zo.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ii.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wp.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hp.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tr.hahajie.cn

[A17] 位运算
来源：http://xy.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tl.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bq.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pj.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xj.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://db.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ak.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ga.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jg.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://yg.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://ie.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://bd.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tt.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bj.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://lf.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ou.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://te.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://eg.wgjwhj.cn

[A19] 交换两个变量
来源：http://ea.9csxet.cn

Py:   a, b = b, a
来源：http://ox.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dr.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://kd.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://kg.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://ol.panjiajie.cn

Go:   a, b = b, a
来源：http://mb.bjjhwx.cn

Ruby: a, b = b, a
来源：http://tf.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://jd.chemitech.net.cn

[A20] 读取标准输入
来源：http://wx.hnjuh.cn

Py:   name = input("请输入：")
来源：http://qd.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wc.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zc.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://ha.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://sx.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ex.nszjky.cn

Ruby: gets.chomp
来源：http://vv.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://rd.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://sl.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://vv.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zw.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://oe.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://gq.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://jg.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iu.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://wa.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://ph.lnxyls.cn

[A22] 获取字符串长度
来源：http://dy.hnjuh.cn

Py:   len(s)
来源：http://ie.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://at.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://en.colortex.cn

TS:   s.length
来源：http://md.shxzukj.cn

Java: s.length()
来源：http://cw.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hg.newstarts.cn

Ruby: s.length
来源：http://if.shxzukj.cn

C#:   s.Length
来源：http://tw.nicolike.cn

[A23] 大小写转换
来源：http://ny.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qt.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zw.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zp.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kt.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hm.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wo.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pj.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://if.huixiangedu.cn

[A24] 去除首尾空白
来源：http://gq.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fp.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zr.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://un.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://im.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tl.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://hr.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sa.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wj.gzmigu.cn

[A25] 字符串比较
来源：http://ue.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://qj.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fb.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ln.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ho.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cl.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kt.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://py.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hv.huixiangedu.cn

[A26] 类型转换总览
来源：http://tk.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eb.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aj.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ef.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://fh.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mo.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ja.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ik.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uw.yuexingan06.cn

================================================================================
来源：http://de.jctech888.com.cn

B. 流程控制
来源：http://qy.9csxet.cn

================================================================================
来源：http://ti.9csxet.cn

[B01] 条件判断 if / else
来源：http://yp.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hg.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ac.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://el.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ge.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vu.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ze.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sb.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zi.521024.cn

[B02] 多分支 else if / elif
来源：http://yk.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ie.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://le.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wb.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rp.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oa.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hw.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vj.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zb.521024.cn

[B03] switch / match / case
来源：http://lg.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://to.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hb.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nw.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kj.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ds.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mz.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zr.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pp.huixinmuqiang.cn

[B04] for 计数循环
来源：http://xy.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://hc.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ic.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cr.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rn.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ka.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sq.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://ed.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ss.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://no.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://pi.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lz.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://di.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rd.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ea.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nn.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://mg.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xt.colortex.cn

[B06] 遍历字典 / 对象
来源：http://qe.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vf.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qb.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lm.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ts.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pm.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://co.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yv.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hn.asd995.cn

[B07] while 循环
来源：http://ox.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://dm.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://np.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://ir.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://ox.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://tv.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cd.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://od.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://yl.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://pl.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://qy.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ul.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://rf.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://es.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://ez.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vm.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hx.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://sc.hnjuh.cn

[B09] break 与 continue
来源：http://cc.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rg.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cs.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pn.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iz.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://af.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ms.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rw.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mo.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://sk.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wy.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wi.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nm.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zb.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rg.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ek.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uz.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ui.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://rw.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://yc.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://gq.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bk.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uj.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ag.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://os.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://wg.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jk.haigaiapp.cn

[B12] 跳出多层循环
来源：http://ow.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fj.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pl.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dq.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nn.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hu.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tx.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ko.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://li.9csxet.cn

[B13] 判断是否为数字
来源：http://hc.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://qk.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://ji.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yf.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://db.chemitech.net.cn

Java: x instanceof Number
来源：http://of.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://px.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://wp.9csxet.cn

C#:   x is int or double or decimal
来源：http://ww.colortex.cn

[B14] 判断值是否在集合内
来源：http://jb.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oa.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ch.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://xq.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://jc.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dy.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ep.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ri.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xa.colortex.cn

[B15] 布尔运算与取反
来源：http://im.shxzskj.cn

Py:   a and b or not c
来源：http://zy.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://qg.huixiangedu.cn

JS:   a && b || !c
来源：http://nc.asd995.cn

TS:   a && b || !c
来源：http://ov.9csxet.cn

Java: a && b || !c
来源：http://uz.huixiangedu.cn

Go:   a && b || !c
来源：http://fq.shxzskj.cn

Ruby: a && b || !c
来源：http://pu.huixinmuqiang.cn

C#:   a && b || !c
来源：http://hn.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zh.colortex.cn

Py:   if not data: return
来源：http://wy.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://kh.nicolike.cn

JS:   if (!data) return;
来源：http://of.521024.cn

TS:   if (!data) return;
来源：http://gi.9csxet.cn

Java: if (data == null) return;
来源：http://wp.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://ub.wgjwhj.cn

Ruby: return if data.nil?
来源：http://mp.hahajie.cn

C#:   if (data == null) return;
来源：http://vj.haigaiapp.cn

================================================================================
来源：http://pg.newstarts.cn

C. 函数与作用域
来源：http://vn.szxytkj.cn

================================================================================
来源：http://iy.gzmigu.cn

[C01] 定义函数
来源：http://zt.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://sm.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nm.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://dx.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://as.9csxet.cn


<!-- 参考信息 -->