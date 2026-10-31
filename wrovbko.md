代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://am.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://em.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hy.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://dc.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vq.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vi.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fa.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xq.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://an.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mz.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ve.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tc.yuexingan06.cn

[A10] 生成随机数
来源：http://ba.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://uu.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://ui.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yt.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sj.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://ef.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bv.szsharing.cn

Ruby: rand(1..100)
来源：http://vr.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://rv.szsharing.cn

[A11] 条件表达式（三元）
来源：http://wn.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://nz.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ob.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zb.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://va.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://wq.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wn.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iq.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yf.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://zd.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dm.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tt.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://sz.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://wj.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://zy.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gw.521024.cn

Ruby: "Hello, #{name}!"
来源：http://ao.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://kg.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sl.huanxung.cn

Py:   "第一行\n第二行"
来源：http://tv.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://wb.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://yd.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://ol.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://sj.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://su.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://tg.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://ef.jianghongdianzi.cn

[A14] 注释写法
来源：http://xm.hnjuh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dr.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rt.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://hb.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://mc.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cn.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://up.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jb.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://vz.nicolike.cn

[A15] 空值判断与默认值
来源：http://sf.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://yb.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://ee.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://ir.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://xc.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ss.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://fp.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://he.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://ns.jctech888.com.cn

[A16] 真假值判断规则
来源：http://zf.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zw.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ut.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ph.9csxet.cn

TS:   if (!x) {}
来源：http://gm.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zn.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://de.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ct.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bx.yuexingan06.cn

[A17] 位运算
来源：http://wv.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ob.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dy.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ra.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://al.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ky.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rh.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yw.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ps.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://en.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://ma.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://du.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vy.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pr.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://vc.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vl.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://go.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://vm.szsharing.cn

[A19] 交换两个变量
来源：http://bt.9csxet.cn

Py:   a, b = b, a
来源：http://rb.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mt.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://ec.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://le.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://st.szxytkj.cn

Go:   a, b = b, a
来源：http://md.gzmigu.cn

Ruby: a, b = b, a
来源：http://ba.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://ap.chemitech.net.cn

[A20] 读取标准输入
来源：http://am.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://wi.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ml.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kt.colortex.cn

TS:   // Node.js：readline 模块
来源：http://mk.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://zw.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ns.chemitech.net.cn

Ruby: gets.chomp
来源：http://yi.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://qx.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://kl.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://ge.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ww.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://xg.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://od.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://tw.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dk.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://le.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://bw.asd995.cn

[A22] 获取字符串长度
来源：http://uq.szxytkj.cn

Py:   len(s)
来源：http://dm.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://le.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ib.nszjky.cn

TS:   s.length
来源：http://ju.chemitech.net.cn

Java: s.length()
来源：http://sb.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wi.nszjky.cn

Ruby: s.length
来源：http://fa.shtwfgs.cn

C#:   s.Length
来源：http://eu.nszjky.cn

[A23] 大小写转换
来源：http://qh.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zw.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ec.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wv.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://in.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kv.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dk.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cj.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://px.huixiangedu.cn

[A24] 去除首尾空白
来源：http://fm.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xd.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cw.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vq.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tt.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zo.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://jy.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://il.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ym.jctech888.com.cn

[A25] 字符串比较
来源：http://ya.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://sy.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qw.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zk.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fg.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tj.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qs.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cu.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kl.muxihuayi.cn

[A26] 类型转换总览
来源：http://rp.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vk.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rx.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dw.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://vs.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hn.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ds.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mx.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qp.haigaiapp.cn

================================================================================
来源：http://ck.jianghongdianzi.cn

B. 流程控制
来源：http://np.hahajie.cn

================================================================================
来源：http://lb.szsharing.cn

[B01] 条件判断 if / else
来源：http://rs.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uv.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hw.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tr.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aa.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cp.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fe.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://we.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qr.colortex.cn

[B02] 多分支 else if / elif
来源：http://tv.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://md.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qr.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oa.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gf.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xi.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wj.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hq.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dh.jctech888.com.cn

[B03] switch / match / case
来源：http://pv.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://by.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cm.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pk.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xb.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ca.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zk.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://or.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dh.9csxet.cn

[B04] for 计数循环
来源：http://pi.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://ur.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fj.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fp.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://do.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lv.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ws.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://ux.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mr.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://bh.szsharing.cn

Py:   for item in arr: print(item)
来源：http://qq.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bc.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://js.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wu.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vc.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fr.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://ww.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mb.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://wr.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tk.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ho.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jy.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ln.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ap.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lr.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pc.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sl.shxzukj.cn

[B07] while 循环
来源：http://eg.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://dt.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zs.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://ib.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://jm.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://ux.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zi.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://cx.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://xb.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://dj.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://kj.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nc.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://vl.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://yw.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://as.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zh.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xy.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://li.lnxyls.cn

[B09] break 与 continue
来源：http://ex.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wt.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lb.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tn.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tk.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ey.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ms.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xp.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ew.9csxet.cn

[B10] 遍历同时拿索引
来源：http://rs.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oa.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nj.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hg.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bt.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vc.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fj.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yd.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bn.521024.cn

[B11] 生成数字序列 / 区间
来源：http://qv.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://mq.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://pz.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tb.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cw.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tq.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://fv.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qm.9csxet.cn

[B12] 跳出多层循环
来源：http://wb.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hg.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nw.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kf.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cr.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ml.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://di.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zm.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://az.wgjwhj.cn

[B13] 判断是否为数字
来源：http://dn.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://vv.szxytkj.cn

PHP:  is_numeric($x)
来源：http://hd.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gk.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vr.wgjwhj.cn

Java: x instanceof Number
来源：http://ac.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xm.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://nk.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://fo.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://st.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qb.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ep.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://gn.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://fw.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kv.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ci.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ur.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bt.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://kz.shxzskj.cn

Py:   a and b or not c
来源：http://aj.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://kh.jianghongdianzi.cn

JS:   a && b || !c
来源：http://ht.huanxung.cn

TS:   a && b || !c
来源：http://lx.hnjuh.cn

Java: a && b || !c
来源：http://de.bjjhwx.cn


<!-- 参考信息 -->