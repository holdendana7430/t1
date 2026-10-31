代发 wailian999

[A10] 生成随机数
来源：http://fv.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://si.9csxet.cn

PHP:  random_int(1, 100);
来源：http://lq.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cx.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vf.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://bn.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pq.hahajie.cn

Ruby: rand(1..100)
来源：http://wd.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://ku.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://ap.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://ek.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ww.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wy.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sn.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://mq.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://iv.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rz.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://af.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://rb.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://am.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tx.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://nt.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://qt.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://ng.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cx.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://gt.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://nt.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sr.colortex.cn

Py:   "第一行\n第二行"
来源：http://rb.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://lr.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://ca.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://qm.hnjuh.cn

Java: "第一行\n第二行"
来源：http://qr.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://sx.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://hy.szsharing.cn

C#:   "第一行\n第二行"
来源：http://uc.gzmigu.cn

[A14] 注释写法
来源：http://je.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cn.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://so.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://ko.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://qm.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nm.521024.cn

Go:   // 单行；/* 多行 */
来源：http://qp.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://no.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://lz.asd995.cn

[A15] 空值判断与默认值
来源：http://hp.panjiajie.cn

Py:   value = data or "默认值"
来源：http://zp.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://pq.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://gq.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://rg.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bk.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://qq.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://ei.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://qn.asd995.cn

[A16] 真假值判断规则
来源：http://re.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vv.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cy.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uh.chemitech.net.cn

TS:   if (!x) {}
来源：http://wr.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vi.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gk.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://am.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rq.bjjhwx.cn

[A17] 位运算
来源：http://yz.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mk.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wq.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pl.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://se.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mn.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sv.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://he.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qa.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://tl.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://iw.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://vt.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bo.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zm.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://cz.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ux.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://vx.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://ox.asd995.cn

[A19] 交换两个变量
来源：http://rz.szsharing.cn

Py:   a, b = b, a
来源：http://ww.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://py.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://aa.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://kq.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://oh.nszjky.cn

Go:   a, b = b, a
来源：http://xh.nszjky.cn

Ruby: a, b = b, a
来源：http://qs.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://us.panjiajie.cn

[A20] 读取标准输入
来源：http://wn.gzmigu.cn

Py:   name = input("请输入：")
来源：http://fz.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ef.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oi.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://ul.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://fo.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jm.hahajie.cn

Ruby: gets.chomp
来源：http://di.nicolike.cn

C#:   Console.ReadLine();
来源：http://mz.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://ka.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://tf.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mf.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://xh.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://mj.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://ps.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ok.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ww.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://ze.hahajie.cn

[A22] 获取字符串长度
来源：http://fd.9csxet.cn

Py:   len(s)
来源：http://gr.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sr.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jc.bookmarksfly.cn

TS:   s.length
来源：http://yx.newstarts.cn

Java: s.length()
来源：http://zd.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ss.jctech888.com.cn

Ruby: s.length
来源：http://xi.muxihuayi.cn

C#:   s.Length
来源：http://cw.asd995.cn

[A23] 大小写转换
来源：http://gs.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gp.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dc.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ri.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://no.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kg.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ax.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eq.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sd.hahajie.cn

[A24] 去除首尾空白
来源：http://as.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jt.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ls.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gs.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mu.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jf.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://cn.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vx.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://db.shxzskj.cn

[A25] 字符串比较
来源：http://gy.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://pl.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xm.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rs.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cs.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iw.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sf.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wx.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://as.chemitech.net.cn

[A26] 类型转换总览
来源：http://uj.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ag.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jk.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bg.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://gn.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zo.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tj.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://as.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ak.gzmigu.cn

================================================================================
来源：http://qx.wgjwhj.cn

B. 流程控制
来源：http://zl.nszjky.cn

================================================================================
来源：http://sj.asd995.cn

[B01] 条件判断 if / else
来源：http://ay.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ev.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jc.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wb.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lz.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ro.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hu.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zy.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aw.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://vy.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://za.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rh.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xk.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ug.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fj.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sm.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rw.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lj.nicolike.cn

[B03] switch / match / case
来源：http://ia.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xq.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kt.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tb.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fy.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ub.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yr.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sv.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jp.shtwfgs.cn

[B04] for 计数循环
来源：http://ui.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://js.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://px.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kt.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eh.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nv.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rp.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://pj.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tb.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://yx.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://mn.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yb.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://re.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mg.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ui.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nb.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://oq.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vv.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ne.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oe.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ct.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dn.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sk.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pu.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xh.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eq.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xi.huixinmuqiang.cn

[B07] while 循环
来源：http://zv.521024.cn

Py:   while i < 10: i += 1
来源：http://ky.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iw.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://je.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://eu.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://im.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uh.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://nu.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://tp.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://wv.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://wv.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cr.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://lq.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://di.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://ew.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zb.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jp.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://py.huixiangedu.cn

[B09] break 与 continue
来源：http://ts.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dc.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://um.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ya.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ue.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lo.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kg.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lf.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cy.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://wt.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mx.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vw.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kg.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ss.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ft.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zk.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ak.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qo.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://ww.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://hu.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://fn.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bk.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://go.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hy.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bp.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://kv.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://je.hahajie.cn

[B12] 跳出多层循环
来源：http://rw.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mm.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://af.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gv.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wt.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sg.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://du.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oe.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sk.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://di.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://ds.gzmigu.cn

PHP:  is_numeric($x)
来源：http://np.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nm.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oi.asd995.cn

Java: x instanceof Number
来源：http://sd.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qm.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://is.szxytkj.cn

C#:   x is int or double or decimal
来源：http://ef.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://fj.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mp.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dj.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://lt.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://dw.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ny.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xh.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ga.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hg.colortex.cn

[B15] 布尔运算与取反
来源：http://wi.yuexingan06.cn

Py:   a and b or not c
来源：http://az.521024.cn

PHP:  $a && $b || !$c
来源：http://li.haigaiapp.cn

JS:   a && b || !c
来源：http://nj.muxihuayi.cn

TS:   a && b || !c
来源：http://rc.huixinmuqiang.cn

Java: a && b || !c
来源：http://sk.wgjwhj.cn

Go:   a && b || !c
来源：http://tl.hnjuh.cn

Ruby: a && b || !c
来源：http://gt.9csxet.cn

C#:   a && b || !c
来源：http://mr.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hr.gzmigu.cn

Py:   if not data: return
来源：http://vb.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://xu.asd995.cn

JS:   if (!data) return;
来源：http://xb.szsharing.cn

TS:   if (!data) return;
来源：http://bw.huixiangedu.cn

Java: if (data == null) return;
来源：http://ko.szxytkj.cn

Go:   if data == nil { return }
来源：http://zy.asd995.cn

Ruby: return if data.nil?
来源：http://sf.asd995.cn

C#:   if (data == null) return;
来源：http://cf.521024.cn


<!-- 参考信息 -->