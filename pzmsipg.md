代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://fh.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://km.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://kh.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hs.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qx.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iw.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://vw.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://so.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dn.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bi.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://pf.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vf.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zi.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://zn.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://yb.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://au.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uk.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://qr.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://zw.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ct.hahajie.cn

Py:   "第一行\n第二行"
来源：http://na.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://ve.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://gk.colortex.cn

TS:   "第一行\n第二行"
来源：http://nt.shxzukj.cn

Java: "第一行\n第二行"
来源：http://xg.521024.cn

Go:   "第一行\n第二行"
来源：http://jn.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://bm.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://ni.nicolike.cn

[A14] 注释写法
来源：http://ao.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tp.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ax.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://pm.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://pi.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://he.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://pb.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xy.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://be.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://sr.szxytkj.cn

Py:   value = data or "默认值"
来源：http://hb.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://rw.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://ex.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://uf.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kx.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://gm.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://qy.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://ez.shtwfgs.cn

[A16] 真假值判断规则
来源：http://wd.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jo.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ut.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tn.szsharing.cn

TS:   if (!x) {}
来源：http://fm.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jg.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tf.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nc.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qt.hnjuh.cn

[A17] 位运算
来源：http://kp.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gh.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jq.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wl.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ua.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jf.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wn.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dg.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zs.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://ft.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://ky.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://ng.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ym.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xe.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://oa.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dg.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://yv.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://wh.newstarts.cn

[A19] 交换两个变量
来源：http://fg.szsharing.cn

Py:   a, b = b, a
来源：http://ro.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://um.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://px.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://ej.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://kz.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://xi.szxytkj.cn

Ruby: a, b = b, a
来源：http://te.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://rn.9csxet.cn

[A20] 读取标准输入
来源：http://mv.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://wi.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eu.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://en.asd995.cn

TS:   // Node.js：readline 模块
来源：http://lm.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://li.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jd.521024.cn

Ruby: gets.chomp
来源：http://eg.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://du.hahajie.cn

[A21] 保留指定小数位输出
来源：http://yk.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://ml.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vt.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://ep.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://rl.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ka.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pz.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://yd.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://gx.shtwfgs.cn

[A22] 获取字符串长度
来源：http://jq.hnjuh.cn

Py:   len(s)
来源：http://io.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://au.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sr.jianghongdianzi.cn

TS:   s.length
来源：http://me.panjiajie.cn

Java: s.length()
来源：http://mh.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kn.szxytkj.cn

Ruby: s.length
来源：http://dz.asd995.cn

C#:   s.Length
来源：http://tq.asd995.cn

[A23] 大小写转换
来源：http://vl.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rl.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cx.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uh.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ox.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wt.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cc.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vk.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://la.wgjwhj.cn

[A24] 去除首尾空白
来源：http://rk.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ex.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://op.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xr.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lg.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vk.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://kx.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yh.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wk.colortex.cn

[A25] 字符串比较
来源：http://hf.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://ht.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lp.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nf.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jc.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dz.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ju.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tp.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hh.szsharing.cn

[A26] 类型转换总览
来源：http://bx.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xc.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mt.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://co.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://pz.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bl.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ej.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kf.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sg.huixiangedu.cn

================================================================================
来源：http://vj.bjjhwx.cn

B. 流程控制
来源：http://mz.newstarts.cn

================================================================================
来源：http://zl.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://gz.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ts.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lo.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mo.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://au.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qf.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ir.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pa.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rg.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://vb.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jj.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pg.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kq.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aa.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ab.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bq.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ab.521024.cn

[B03] switch / match / case
来源：http://aw.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vg.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dl.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sn.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wz.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vb.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nx.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ur.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lk.haigaiapp.cn

[B04] for 计数循环
来源：http://yq.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://gn.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dl.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lj.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://al.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ta.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hj.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://li.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xx.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://vk.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://vj.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://df.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eh.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qk.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dz.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kr.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://ge.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://em.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://uz.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iv.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cv.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://it.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lc.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kl.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yz.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vl.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ru.huixinmuqiang.cn

[B07] while 循环
来源：http://pu.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://dd.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ky.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://jq.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://xs.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://ye.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://or.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://aq.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://iy.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://xz.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://ha.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qu.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://vd.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://jh.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://gs.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nu.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://et.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://zx.hnjuh.cn

[B09] break 与 continue
来源：http://qd.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sm.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gu.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vt.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yj.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hr.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iq.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zx.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://um.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://zh.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yq.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xb.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gz.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eb.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hu.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://em.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fd.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ib.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://lu.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://jr.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://yl.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xm.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yg.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xl.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://es.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://hv.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vq.hahajie.cn

[B12] 跳出多层循环
来源：http://ue.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wg.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ln.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cn.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ru.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rl.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qa.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rt.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sq.haigaiapp.cn

[B13] 判断是否为数字
来源：http://fh.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://mq.newstarts.cn

PHP:  is_numeric($x)
来源：http://sx.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cj.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jg.huanxung.cn

Java: x instanceof Number
来源：http://gz.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yb.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://vh.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://hp.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://an.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dl.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nq.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://sr.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ch.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ma.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hx.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mt.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dp.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://zt.haigaiapp.cn

Py:   a and b or not c
来源：http://lx.szsharing.cn

PHP:  $a && $b || !$c
来源：http://rh.haigaiapp.cn

JS:   a && b || !c
来源：http://ku.newstarts.cn

TS:   a && b || !c
来源：http://vd.shxzskj.cn

Java: a && b || !c
来源：http://ng.haigaiapp.cn

Go:   a && b || !c
来源：http://gq.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://xa.jianghongdianzi.cn

C#:   a && b || !c
来源：http://rd.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tx.shxzskj.cn

Py:   if not data: return
来源：http://lp.colortex.cn

PHP:  if (!$data) { return; }
来源：http://zu.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://yk.yuexingan06.cn

TS:   if (!data) return;
来源：http://vj.asd995.cn

Java: if (data == null) return;
来源：http://ta.muxihuayi.cn

Go:   if data == nil { return }
来源：http://me.chemitech.net.cn

Ruby: return if data.nil?
来源：http://bw.shxzukj.cn

C#:   if (data == null) return;
来源：http://eh.haigaiapp.cn

================================================================================
来源：http://nm.nszjky.cn

C. 函数与作用域
来源：http://hy.asd995.cn

================================================================================
来源：http://km.panjiajie.cn

[C01] 定义函数
来源：http://ml.521024.cn

Py:   def add(a, b): return a + b
来源：http://eo.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zz.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://gc.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pw.shxzskj.cn


<!-- 参考信息 -->