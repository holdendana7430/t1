代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zm.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iq.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ec.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mr.panjiajie.cn

[A10] 生成随机数
来源：http://qc.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://oa.asd995.cn

PHP:  random_int(1, 100);
来源：http://iw.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cr.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hh.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ci.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dg.chemitech.net.cn

Ruby: rand(1..100)
来源：http://mj.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://ko.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://gr.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://dy.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xz.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://of.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kq.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://zg.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ik.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://da.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xb.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://ij.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rq.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gp.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://gv.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://ho.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://tc.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mv.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://hg.asd995.cn

C#:   $"Hello, {name}!"
来源：http://uz.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gp.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://ky.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://fg.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://zc.hahajie.cn

TS:   "第一行\n第二行"
来源：http://mn.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://sd.szsharing.cn

Go:   "第一行\n第二行"
来源：http://jt.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://lw.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://um.szxytkj.cn

[A14] 注释写法
来源：http://uu.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yv.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dm.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://uw.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://mz.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vf.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://ai.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gq.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://qc.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://hg.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://au.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://uu.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://pq.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://un.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vf.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://uc.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://cr.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://qk.gzmigu.cn

[A16] 真假值判断规则
来源：http://ww.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eo.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yk.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ov.szxytkj.cn

TS:   if (!x) {}
来源：http://fm.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sw.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://av.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fi.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://li.jctech888.com.cn

[A17] 位运算
来源：http://rp.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xx.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zk.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://as.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vh.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ah.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ak.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sg.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gr.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://uy.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://dy.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://si.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dp.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yf.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://ps.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pf.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://oq.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://nz.shtwfgs.cn

[A19] 交换两个变量
来源：http://sb.colortex.cn

Py:   a, b = b, a
来源：http://si.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ds.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://hg.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://hh.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://wr.hahajie.cn

Go:   a, b = b, a
来源：http://ke.yuexingan06.cn

Ruby: a, b = b, a
来源：http://dc.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://in.panjiajie.cn

[A20] 读取标准输入
来源：http://hx.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://xk.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qz.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qp.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://xj.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://pg.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vs.nszjky.cn

Ruby: gets.chomp
来源：http://rh.shxzukj.cn

C#:   Console.ReadLine();
来源：http://bi.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://rd.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://io.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hh.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://oc.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://cw.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://no.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xo.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://zn.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://bi.huanxung.cn

[A22] 获取字符串长度
来源：http://tt.jianghongdianzi.cn

Py:   len(s)
来源：http://gv.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dw.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rv.chemitech.net.cn

TS:   s.length
来源：http://ip.wgjwhj.cn

Java: s.length()
来源：http://gz.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pr.szsharing.cn

Ruby: s.length
来源：http://ce.bjjhwx.cn

C#:   s.Length
来源：http://ly.shtwfgs.cn

[A23] 大小写转换
来源：http://jm.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://iz.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pv.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dx.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nk.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ks.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eq.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fe.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yu.hnjuh.cn

[A24] 去除首尾空白
来源：http://kk.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ah.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tv.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ai.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hm.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sy.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://vu.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cy.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dv.haigaiapp.cn

[A25] 字符串比较
来源：http://nn.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://he.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bm.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ms.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kq.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fx.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://od.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jx.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lq.huanxung.cn

[A26] 类型转换总览
来源：http://ns.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zm.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fz.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gi.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://qk.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qt.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ul.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lt.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ah.panjiajie.cn

================================================================================
来源：http://fc.jianghongdianzi.cn

B. 流程控制
来源：http://tc.bjjhwx.cn

================================================================================
来源：http://gq.hahajie.cn

[B01] 条件判断 if / else
来源：http://va.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kp.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zb.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cl.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vq.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bw.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pi.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cb.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xc.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://na.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fn.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xt.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vc.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lj.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jg.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vf.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lh.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://es.lnxyls.cn

[B03] switch / match / case
来源：http://vk.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cz.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qv.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://px.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hj.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gv.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hn.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eb.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iw.wgjwhj.cn

[B04] for 计数循环
来源：http://js.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://oy.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://od.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yr.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ek.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ev.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vg.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://ia.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ul.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://oa.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://xb.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hj.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zi.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rn.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hm.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zf.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://at.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lp.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://cd.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vh.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ok.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cw.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bw.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://it.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dj.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ct.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eg.nicolike.cn

[B07] while 循环
来源：http://ib.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://ba.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://un.521024.cn

JS:   while (i < 10) { i++; }
来源：http://aa.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://tn.521024.cn

Java: while (i < 10) { i++; }
来源：http://xa.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gc.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://xn.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://lv.colortex.cn

[B08] do-while（至少执行一次）
来源：http://vd.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://cw.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yd.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://hd.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://tc.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://kp.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oo.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uc.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://wx.521024.cn

[B09] break 与 continue
来源：http://nl.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ir.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sx.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gk.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yo.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rr.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pq.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gp.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ik.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bq.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cu.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rg.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lq.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://py.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://im.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gp.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yq.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://vn.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://qg.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://fn.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rm.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rg.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://si.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lo.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://sq.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cr.lnxyls.cn

[B12] 跳出多层循环
来源：http://lz.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fj.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cj.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://he.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yv.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ot.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dk.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gs.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ex.jctech888.com.cn

[B13] 判断是否为数字
来源：http://bf.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://xv.szxytkj.cn

PHP:  is_numeric($x)
来源：http://gn.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cv.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gk.9csxet.cn

Java: x instanceof Number
来源：http://vg.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lz.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://va.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://gu.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://pi.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://th.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wr.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://lx.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://wi.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ex.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mi.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lv.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ci.colortex.cn

[B15] 布尔运算与取反
来源：http://fn.szsharing.cn

Py:   a and b or not c
来源：http://vz.nicolike.cn

PHP:  $a && $b || !$c
来源：http://nw.wgjwhj.cn

JS:   a && b || !c
来源：http://vu.huanxung.cn

TS:   a && b || !c
来源：http://sr.muxihuayi.cn

Java: a && b || !c
来源：http://gp.huixiangedu.cn

Go:   a && b || !c
来源：http://vb.haigaiapp.cn

Ruby: a && b || !c
来源：http://qu.yuexingan06.cn

C#:   a && b || !c
来源：http://zu.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pw.shxzukj.cn

Py:   if not data: return
来源：http://vv.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://bd.colortex.cn

JS:   if (!data) return;
来源：http://xl.521024.cn

TS:   if (!data) return;
来源：http://mq.nszjky.cn


<!-- 参考信息 -->