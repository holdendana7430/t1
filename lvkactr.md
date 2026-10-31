代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wt.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qo.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qw.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://rv.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fy.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lr.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://az.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://td.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gz.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ll.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rd.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://av.gzmigu.cn

[A10] 生成随机数
来源：http://at.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://nh.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://ya.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mm.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wh.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://az.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ec.nicolike.cn

Ruby: rand(1..100)
来源：http://wx.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://si.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://fy.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://op.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://go.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jc.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ge.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://jy.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ib.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vz.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xt.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://wy.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dl.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nu.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://tr.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://kc.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://bm.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bu.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://sd.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://xy.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xx.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://dv.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://qb.nszjky.cn

JS:   "第一行\n第二行"
来源：http://ha.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://bz.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://es.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://km.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://ak.nicolike.cn

C#:   "第一行\n第二行"
来源：http://rt.9csxet.cn

[A14] 注释写法
来源：http://fk.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ll.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jv.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://hw.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://yf.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qp.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://sp.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://se.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://ze.nszjky.cn

[A15] 空值判断与默认值
来源：http://ip.asd995.cn

Py:   value = data or "默认值"
来源：http://sx.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://fc.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://zx.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://gk.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bf.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://rj.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://ya.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://ck.wgjwhj.cn

[A16] 真假值判断规则
来源：http://vm.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qc.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tp.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bc.jctech888.com.cn

TS:   if (!x) {}
来源：http://qn.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qo.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gu.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xb.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ad.huanxung.cn

[A17] 位运算
来源：http://tk.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nl.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sw.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ud.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://da.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mh.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ed.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fl.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kl.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://es.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://li.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://tf.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oj.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ai.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://rv.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hy.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://qi.521024.cn

C#:   (int)'A'; (char)65
来源：http://fy.shtwfgs.cn

[A19] 交换两个变量
来源：http://qn.bookmarksfly.cn

Py:   a, b = b, a
来源：http://cy.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oa.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://pp.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://ee.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://ak.hnjuh.cn

Go:   a, b = b, a
来源：http://qk.colortex.cn

Ruby: a, b = b, a
来源：http://nz.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://ps.asd995.cn

[A20] 读取标准输入
来源：http://ue.panjiajie.cn

Py:   name = input("请输入：")
来源：http://qw.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tr.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ki.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://vm.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://ha.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vk.yuexingan06.cn

Ruby: gets.chomp
来源：http://iq.lnxyls.cn

C#:   Console.ReadLine();
来源：http://bq.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://ph.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://kt.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vd.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://lq.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://gw.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://mv.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kz.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://cl.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://ne.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://tx.nszjky.cn

Py:   len(s)
来源：http://qn.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rn.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cs.gzmigu.cn

TS:   s.length
来源：http://tm.panjiajie.cn

Java: s.length()
来源：http://gj.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mf.yuexingan06.cn

Ruby: s.length
来源：http://fj.gzmigu.cn

C#:   s.Length
来源：http://yv.szsharing.cn

[A23] 大小写转换
来源：http://jw.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yw.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rx.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hh.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yq.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lv.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hm.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oe.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ct.panjiajie.cn

[A24] 去除首尾空白
来源：http://mb.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wt.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mn.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ma.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gq.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jg.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://uu.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ay.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wf.nszjky.cn

[A25] 字符串比较
来源：http://nc.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://dl.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ap.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mn.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bb.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ni.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dk.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fy.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wc.bookmarksfly.cn

[A26] 类型转换总览
来源：http://kb.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ui.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ut.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ab.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://ds.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nq.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bc.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vq.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bn.huixiangedu.cn

================================================================================
来源：http://ti.bjjhwx.cn

B. 流程控制
来源：http://pu.huanxung.cn

================================================================================
来源：http://ew.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://yb.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wy.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://av.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fu.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kt.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mi.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wm.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cu.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xu.newstarts.cn

[B02] 多分支 else if / elif
来源：http://vk.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tt.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ub.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gt.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yl.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://el.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bz.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://az.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iv.yuexingan06.cn

[B03] switch / match / case
来源：http://iu.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kn.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ap.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ku.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sj.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ao.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ir.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yz.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pw.hnjuh.cn

[B04] for 计数循环
来源：http://ov.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://we.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://er.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bh.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jf.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ra.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://na.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://gu.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pp.colortex.cn

[B05] 遍历数组 / 列表
来源：http://jy.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://hg.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ua.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wk.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ch.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dy.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gu.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://jp.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://az.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://uz.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tm.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yd.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ib.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ug.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mk.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ke.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yg.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qh.newstarts.cn

[B07] while 循环
来源：http://cv.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://ek.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ux.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://gw.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://ta.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://zk.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hk.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://nh.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://gq.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://zt.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://tt.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://du.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://rz.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://cy.521024.cn

Java: do { i++; } while (i < 10);
来源：http://cd.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kh.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kl.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://jy.jctech888.com.cn

[B09] break 与 continue
来源：http://vz.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ws.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mb.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://es.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qs.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nn.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wh.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yu.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ih.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://ma.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jg.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://at.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xo.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lo.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uf.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ne.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ex.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xc.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://ja.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://ha.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://rh.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yw.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cl.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nq.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nm.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://eu.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mc.nszjky.cn

[B12] 跳出多层循环
来源：http://xd.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oc.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ld.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://md.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gt.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://su.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jn.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zc.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mc.panjiajie.cn

[B13] 判断是否为数字
来源：http://zt.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://wh.hahajie.cn

PHP:  is_numeric($x)
来源：http://jk.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rp.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ej.bjjhwx.cn

Java: x instanceof Number
来源：http://fd.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fp.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://uu.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://oh.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://cl.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rj.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vr.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://ky.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://vi.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cj.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jl.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zy.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cg.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://th.haigaiapp.cn

Py:   a and b or not c
来源：http://sb.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://pz.chemitech.net.cn

JS:   a && b || !c
来源：http://jl.huixinmuqiang.cn

TS:   a && b || !c
来源：http://rn.muxihuayi.cn

Java: a && b || !c
来源：http://wt.huanxung.cn


<!-- 参考信息 -->