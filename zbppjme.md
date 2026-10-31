代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qw.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dg.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iw.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hg.huixiangedu.cn

[A10] 生成随机数
来源：http://ki.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://kv.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://en.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ta.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oq.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://wl.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wr.lnxyls.cn

Ruby: rand(1..100)
来源：http://lf.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://pi.asd995.cn

[A11] 条件表达式（三元）
来源：http://gh.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://lr.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pr.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tr.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gq.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://jh.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vv.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://de.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mw.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://xb.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lk.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ci.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://gk.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://ya.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://wp.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pw.521024.cn

Ruby: "Hello, #{name}!"
来源：http://ra.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://vx.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sg.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://sn.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://ir.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://ev.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://vi.panjiajie.cn

Java: "第一行\n第二行"
来源：http://sf.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://aa.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://ie.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://wj.muxihuayi.cn

[A14] 注释写法
来源：http://wh.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nx.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xw.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://uz.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://ez.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lb.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://ng.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fy.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://qq.hnjuh.cn

[A15] 空值判断与默认值
来源：http://cv.asd995.cn

Py:   value = data or "默认值"
来源：http://xp.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://eq.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://ss.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://pj.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mx.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://eb.nszjky.cn

Ruby: value = data || "默认值"
来源：http://bv.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://en.shtwfgs.cn

[A16] 真假值判断规则
来源：http://ix.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gk.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pu.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mw.shxzskj.cn

TS:   if (!x) {}
来源：http://zq.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://op.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dx.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ly.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rs.yuntaijiaju.cn

[A17] 位运算
来源：http://el.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xn.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://op.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tp.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xf.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sa.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tx.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gd.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ct.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://ln.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://us.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://nc.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gt.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iu.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://up.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lu.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://kp.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://fv.asd995.cn

[A19] 交换两个变量
来源：http://sc.shxzskj.cn

Py:   a, b = b, a
来源：http://dq.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ob.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://va.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://ky.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://ez.lnxyls.cn

Go:   a, b = b, a
来源：http://rr.huanxung.cn

Ruby: a, b = b, a
来源：http://vb.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://vu.colortex.cn

[A20] 读取标准输入
来源：http://sr.huanxung.cn

Py:   name = input("请输入：")
来源：http://qh.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cu.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://um.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://px.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://on.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vg.chemitech.net.cn

Ruby: gets.chomp
来源：http://ro.hahajie.cn

C#:   Console.ReadLine();
来源：http://nz.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://xp.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://je.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oc.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://hs.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://jv.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://up.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sy.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://lm.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://xa.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://yk.jianghongdianzi.cn

Py:   len(s)
来源：http://wq.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ks.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yq.nicolike.cn

TS:   s.length
来源：http://xs.bookmarksfly.cn

Java: s.length()
来源：http://lt.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gy.huixiangedu.cn

Ruby: s.length
来源：http://dq.wgjwhj.cn

C#:   s.Length
来源：http://ju.shxzukj.cn

[A23] 大小写转换
来源：http://gi.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://da.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nl.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wn.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ij.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fl.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jp.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nh.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qn.shxzukj.cn

[A24] 去除首尾空白
来源：http://xo.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tx.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tc.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tf.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://or.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zv.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://sa.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ln.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://un.nszjky.cn

[A25] 字符串比较
来源：http://rm.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://ta.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xf.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pp.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yk.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ze.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pa.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tf.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://me.hnjuh.cn

[A26] 类型转换总览
来源：http://dr.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vy.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cp.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yd.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://kr.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ok.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bm.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hs.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dg.huanxung.cn

================================================================================
来源：http://aw.lnxyls.cn

B. 流程控制
来源：http://sj.521024.cn

================================================================================
来源：http://no.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://ic.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zf.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kb.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ko.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wq.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vi.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fm.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sc.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ck.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://ag.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eo.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ca.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wd.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lq.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sv.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mi.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pe.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gq.chemitech.net.cn

[B03] switch / match / case
来源：http://sl.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qv.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://du.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sv.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://li.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cb.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://as.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cj.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ya.521024.cn

[B04] for 计数循环
来源：http://hg.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://uf.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ar.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://er.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ux.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://au.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xi.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://pf.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kf.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://hq.9csxet.cn

Py:   for item in arr: print(item)
来源：http://xg.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qo.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fa.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uk.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oh.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cs.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://jv.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sf.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://td.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://re.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cc.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mt.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zj.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bk.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xu.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cs.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zf.chemitech.net.cn

[B07] while 循环
来源：http://yd.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://fn.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wj.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://dl.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://yx.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://aq.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lh.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ey.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://po.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://az.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://iz.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nm.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://qm.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://kx.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://yk.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://li.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ao.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://ai.szxytkj.cn

[B09] break 与 continue
来源：http://re.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ku.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kd.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xf.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gw.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qm.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ti.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pe.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wi.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://eb.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ma.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xy.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rj.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cj.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ec.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dm.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wa.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uo.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://al.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://la.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://wv.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ax.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://os.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bx.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zy.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://ey.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uj.9csxet.cn

[B12] 跳出多层循环
来源：http://jq.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ui.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nk.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ut.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mm.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wy.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dr.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://to.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://on.shtwfgs.cn

[B13] 判断是否为数字
来源：http://yx.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://bi.gzmigu.cn

PHP:  is_numeric($x)
来源：http://bw.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://he.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fd.haigaiapp.cn

Java: x instanceof Number
来源：http://de.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hr.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://fk.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://dg.hahajie.cn

[B14] 判断值是否在集合内
来源：http://wv.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tm.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wa.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://um.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://al.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fq.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nt.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sd.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ha.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://vf.szsharing.cn

Py:   a and b or not c
来源：http://or.huanxung.cn

PHP:  $a && $b || !$c
来源：http://ed.hahajie.cn

JS:   a && b || !c
来源：http://hl.muxihuayi.cn

TS:   a && b || !c
来源：http://hp.haigaiapp.cn

Java: a && b || !c
来源：http://wh.shxzskj.cn

Go:   a && b || !c
来源：http://dt.wgjwhj.cn

Ruby: a && b || !c
来源：http://pz.chemitech.net.cn

C#:   a && b || !c
来源：http://pu.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zi.hnjuh.cn

Py:   if not data: return
来源：http://ql.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://qa.colortex.cn

JS:   if (!data) return;
来源：http://td.asd995.cn

TS:   if (!data) return;
来源：http://rb.muxihuayi.cn


<!-- 参考信息 -->