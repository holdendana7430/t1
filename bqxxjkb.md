代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://op.asd995.cn

[A11] 条件表达式（三元）
来源：http://nh.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://qj.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://to.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uh.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cl.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://jr.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dy.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gq.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mt.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://fr.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jk.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hc.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://nx.521024.cn

TS:   `Hello, ${name}!`
来源：http://cv.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://up.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://me.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://ii.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://nk.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xt.huanxung.cn

Py:   "第一行\n第二行"
来源：http://cj.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://ii.huanxung.cn

JS:   "第一行\n第二行"
来源：http://im.521024.cn

TS:   "第一行\n第二行"
来源：http://cl.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://pw.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://nr.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://uj.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://up.hahajie.cn

[A14] 注释写法
来源：http://re.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fq.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pv.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://xg.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://ex.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nn.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://zv.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oh.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://fw.shxzukj.cn

[A15] 空值判断与默认值
来源：http://nv.szxytkj.cn

Py:   value = data or "默认值"
来源：http://ve.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://mw.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://zm.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://ta.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tm.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://cc.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://mg.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://nk.newstarts.cn

[A16] 真假值判断规则
来源：http://fl.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hr.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jh.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jd.jctech888.com.cn

TS:   if (!x) {}
来源：http://sd.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tz.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ld.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ui.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ta.hahajie.cn

[A17] 位运算
来源：http://jk.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zw.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gx.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hu.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vh.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dn.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dh.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bj.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dh.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://ik.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://xz.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://wc.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://om.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lt.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://yw.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ol.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://nw.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://bc.521024.cn

[A19] 交换两个变量
来源：http://vg.gzmigu.cn

Py:   a, b = b, a
来源：http://dx.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://da.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://ce.asd995.cn

TS:   [a, b] = [b, a];
来源：http://iz.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://ip.huanxung.cn

Go:   a, b = b, a
来源：http://ms.nicolike.cn

Ruby: a, b = b, a
来源：http://wx.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://wn.nicolike.cn

[A20] 读取标准输入
来源：http://si.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://qz.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ns.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ua.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://pr.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://wd.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bb.szsharing.cn

Ruby: gets.chomp
来源：http://wh.panjiajie.cn

C#:   Console.ReadLine();
来源：http://fp.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://gg.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://bl.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ff.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://zf.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://py.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://pb.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://js.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://wc.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://gx.nicolike.cn

[A22] 获取字符串长度
来源：http://wv.haigaiapp.cn

Py:   len(s)
来源：http://jk.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xo.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hk.shxzukj.cn

TS:   s.length
来源：http://xk.yuntaijiaju.cn

Java: s.length()
来源：http://xy.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nl.yuntaijiaju.cn

Ruby: s.length
来源：http://rh.yuntaijiaju.cn

C#:   s.Length
来源：http://cs.jianghongdianzi.cn

[A23] 大小写转换
来源：http://yz.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ti.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://je.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rj.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vs.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wj.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cm.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ss.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vv.wgjwhj.cn

[A24] 去除首尾空白
来源：http://zh.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ds.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ns.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://na.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pf.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wc.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://hc.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sw.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qp.shxzskj.cn

[A25] 字符串比较
来源：http://tg.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://zo.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lr.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hp.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fd.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jz.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vj.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://af.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pr.huixiangedu.cn

[A26] 类型转换总览
来源：http://bc.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bo.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uc.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xz.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://ev.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vz.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fj.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cm.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lb.521024.cn

================================================================================
来源：http://dg.asd995.cn

B. 流程控制
来源：http://xa.yuntaijiaju.cn

================================================================================
来源：http://cq.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://pl.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tx.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ph.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tm.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nj.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cj.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dp.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dn.asd995.cn

[B02] 多分支 else if / elif
来源：http://gw.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pn.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dy.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xl.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cu.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ac.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lz.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dm.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mg.hahajie.cn

[B03] switch / match / case
来源：http://fs.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ws.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nd.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nk.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uj.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pm.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gk.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ra.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vr.lnxyls.cn

[B04] for 计数循环
来源：http://pe.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://ac.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bg.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jf.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sx.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ag.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ly.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://pu.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://af.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://iv.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://ez.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://li.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fc.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dp.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mi.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ov.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://us.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gw.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://gr.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pl.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://do.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jh.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://so.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ls.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wo.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ww.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gw.panjiajie.cn

[B07] while 循环
来源：http://ky.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://zf.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ox.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://jv.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://gx.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://aa.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eo.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://ec.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://zj.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://xs.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://rj.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://um.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://zm.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://tr.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://mm.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cn.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jg.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://nh.nicolike.cn

[B09] break 与 continue
来源：http://qg.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ap.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://va.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vr.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tj.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pq.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jw.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zc.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://io.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://vm.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kd.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cr.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hn.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qj.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://va.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jk.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ve.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nv.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://qc.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://tk.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://ib.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jw.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gs.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sp.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sz.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://dt.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ah.hahajie.cn

[B12] 跳出多层循环
来源：http://ym.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lu.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kg.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ap.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://se.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nh.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xh.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tb.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eb.yuexingan06.cn

[B13] 判断是否为数字
来源：http://hb.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://ry.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://lc.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qa.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ol.nszjky.cn

Java: x instanceof Number
来源：http://mm.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://td.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://gq.hahajie.cn

C#:   x is int or double or decimal
来源：http://ia.asd995.cn

[B14] 判断值是否在集合内
来源：http://ph.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dp.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ru.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://ky.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://wc.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://va.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ag.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://du.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://db.colortex.cn

[B15] 布尔运算与取反
来源：http://al.521024.cn

Py:   a and b or not c
来源：http://ru.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://cb.lnxyls.cn

JS:   a && b || !c
来源：http://wk.shtwfgs.cn

TS:   a && b || !c
来源：http://xy.9csxet.cn

Java: a && b || !c
来源：http://qm.jctech888.com.cn

Go:   a && b || !c
来源：http://mi.hnjuh.cn

Ruby: a && b || !c
来源：http://iy.panjiajie.cn

C#:   a && b || !c
来源：http://fq.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uz.asd995.cn

Py:   if not data: return
来源：http://ta.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://rj.asd995.cn

JS:   if (!data) return;
来源：http://my.wgjwhj.cn

TS:   if (!data) return;
来源：http://ku.panjiajie.cn

Java: if (data == null) return;
来源：http://ds.szsharing.cn

Go:   if data == nil { return }
来源：http://ve.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://cr.szsharing.cn

C#:   if (data == null) return;
来源：http://sd.hnjuh.cn

================================================================================
来源：http://bj.lnxyls.cn

C. 函数与作用域
来源：http://io.chemitech.net.cn

================================================================================
来源：http://gj.huanxung.cn

[C01] 定义函数
来源：http://qt.521024.cn

Py:   def add(a, b): return a + b
来源：http://dn.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ka.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://cn.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lp.shxzukj.cn


<!-- 参考信息 -->