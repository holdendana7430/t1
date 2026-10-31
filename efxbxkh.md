代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hq.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://ii.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://ga.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rg.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rc.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ko.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://rp.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ew.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://eg.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rq.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://rf.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mb.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wp.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://aa.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://fm.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://vj.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jb.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://bv.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://dw.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ag.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://rm.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://zv.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://ax.nicolike.cn

TS:   "第一行\n第二行"
来源：http://hk.asd995.cn

Java: "第一行\n第二行"
来源：http://ia.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://xg.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://ft.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://oy.yuexingan06.cn

[A14] 注释写法
来源：http://yh.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://he.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ws.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://go.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://bt.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xa.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://tz.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lh.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://bf.colortex.cn

[A15] 空值判断与默认值
来源：http://ni.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://wm.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://qh.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://hp.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://lk.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sq.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://sv.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://em.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://yd.hnjuh.cn

[A16] 真假值判断规则
来源：http://gj.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cn.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uu.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wq.9csxet.cn

TS:   if (!x) {}
来源：http://lm.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tj.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mj.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zv.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://by.shtwfgs.cn

[A17] 位运算
来源：http://ur.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://na.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jm.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bu.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ym.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rf.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://je.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sz.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ii.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://oh.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://mh.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://yr.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zm.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hn.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://wh.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hw.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://wi.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://ch.szxytkj.cn

[A19] 交换两个变量
来源：http://tl.newstarts.cn

Py:   a, b = b, a
来源：http://bn.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gn.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://ig.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://pe.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://zk.muxihuayi.cn

Go:   a, b = b, a
来源：http://wh.chemitech.net.cn

Ruby: a, b = b, a
来源：http://sg.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://bl.lnxyls.cn

[A20] 读取标准输入
来源：http://wp.nicolike.cn

Py:   name = input("请输入：")
来源：http://bq.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://di.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://my.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://wf.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://iz.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rq.lnxyls.cn

Ruby: gets.chomp
来源：http://dc.hnjuh.cn

C#:   Console.ReadLine();
来源：http://na.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://fw.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://zj.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vi.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://ep.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://vy.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://hk.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://io.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://jw.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://qz.szsharing.cn

[A22] 获取字符串长度
来源：http://zx.huanxung.cn

Py:   len(s)
来源：http://np.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uc.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ea.wgjwhj.cn

TS:   s.length
来源：http://ss.bookmarksfly.cn

Java: s.length()
来源：http://pg.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xg.nicolike.cn

Ruby: s.length
来源：http://uf.huixiangedu.cn

C#:   s.Length
来源：http://ff.shtwfgs.cn

[A23] 大小写转换
来源：http://kv.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oi.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://na.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fo.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qn.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wd.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bs.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vi.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ye.shxzukj.cn

[A24] 去除首尾空白
来源：http://gq.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yy.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lm.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dm.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://am.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jy.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://sy.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rd.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vs.9csxet.cn

[A25] 字符串比较
来源：http://vn.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://do.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://il.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qt.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cm.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hk.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zx.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gs.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vz.lnxyls.cn

[A26] 类型转换总览
来源：http://fk.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fj.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xe.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sg.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://gc.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ma.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ac.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wx.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hg.hahajie.cn

================================================================================
来源：http://ik.chemitech.net.cn

B. 流程控制
来源：http://pv.shxzukj.cn

================================================================================
来源：http://zh.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://aq.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wz.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yc.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pm.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tp.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://au.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xp.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vs.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ml.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://qp.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ns.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ft.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jy.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://om.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xw.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://on.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ve.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://at.asd995.cn

[B03] switch / match / case
来源：http://lg.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pp.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ro.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gx.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eb.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lm.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wz.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wr.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ds.hahajie.cn

[B04] for 计数循环
来源：http://cm.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://wy.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ny.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ns.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bx.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jg.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mf.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://uo.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zw.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://ze.nicolike.cn

Py:   for item in arr: print(item)
来源：http://wn.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ql.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://es.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ti.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zf.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cu.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://xb.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fz.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://vg.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mf.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sg.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bg.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wu.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uh.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xy.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ky.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ax.bookmarksfly.cn

[B07] while 循环
来源：http://kt.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://ib.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nt.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://al.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://ut.colortex.cn

Java: while (i < 10) { i++; }
来源：http://kd.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lw.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://go.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://as.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://kz.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://vt.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rv.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://gx.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://gd.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://vy.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yg.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bg.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://ou.szxytkj.cn

[B09] break 与 continue
来源：http://cj.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uc.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zn.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zz.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://as.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xw.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wn.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://do.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gb.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ex.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hr.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xo.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mp.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://at.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ot.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pm.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iu.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ae.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://qh.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://wa.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://rb.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://js.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wl.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fe.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pq.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://nr.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qs.hnjuh.cn

[B12] 跳出多层循环
来源：http://qy.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tx.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sc.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nc.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://le.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qp.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iq.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zp.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wf.bjjhwx.cn

[B13] 判断是否为数字
来源：http://yo.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://vi.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://md.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zh.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sr.szsharing.cn

Java: x instanceof Number
来源：http://tq.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fp.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://kw.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://jk.asd995.cn

[B14] 判断值是否在集合内
来源：http://nc.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cr.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bv.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://kj.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://gt.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dy.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xv.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://af.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gc.shxzskj.cn

[B15] 布尔运算与取反
来源：http://xt.yuntaijiaju.cn

Py:   a and b or not c
来源：http://hl.huanxung.cn

PHP:  $a && $b || !$c
来源：http://nc.huanxung.cn

JS:   a && b || !c
来源：http://si.jianghongdianzi.cn

TS:   a && b || !c
来源：http://hf.hnjuh.cn

Java: a && b || !c
来源：http://le.jctech888.com.cn

Go:   a && b || !c
来源：http://xn.hahajie.cn

Ruby: a && b || !c
来源：http://ob.nicolike.cn

C#:   a && b || !c
来源：http://cq.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fo.szsharing.cn

Py:   if not data: return
来源：http://uv.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://gn.bjjhwx.cn

JS:   if (!data) return;
来源：http://mb.huixiangedu.cn

TS:   if (!data) return;
来源：http://fk.hahajie.cn

Java: if (data == null) return;
来源：http://ge.hnjuh.cn

Go:   if data == nil { return }
来源：http://pj.shtwfgs.cn

Ruby: return if data.nil?
来源：http://cc.lnxyls.cn

C#:   if (data == null) return;
来源：http://zt.nicolike.cn

================================================================================
来源：http://yv.wgjwhj.cn

C. 函数与作用域
来源：http://gy.newstarts.cn

================================================================================
来源：http://nq.bookmarksfly.cn

[C01] 定义函数
来源：http://nu.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://zy.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ev.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://ox.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rt.lnxyls.cn


<!-- 参考信息 -->