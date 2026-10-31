代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://md.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://ec.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zo.bjjhwx.cn

Ruby: rand(1..100)
来源：http://nv.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://su.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://cc.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://wk.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://st.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nu.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zl.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://pt.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://aa.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yq.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cj.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://co.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lz.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qy.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://jc.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://bq.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://lv.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hx.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://op.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://nc.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hy.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://hk.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://qo.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://av.colortex.cn

TS:   "第一行\n第二行"
来源：http://vo.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://ks.huanxung.cn

Go:   "第一行\n第二行"
来源：http://ab.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://zt.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://pn.bookmarksfly.cn

[A14] 注释写法
来源：http://ra.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kq.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wi.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://gy.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://cm.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iy.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://im.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://eg.521024.cn

C#:   // 单行；/* 多行 */
来源：http://hk.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://te.9csxet.cn

Py:   value = data or "默认值"
来源：http://ja.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://ci.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://ai.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://xl.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nh.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://kt.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://gv.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://vz.huanxung.cn

[A16] 真假值判断规则
来源：http://vb.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ws.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ep.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ty.9csxet.cn

TS:   if (!x) {}
来源：http://im.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fv.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ps.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ak.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://im.huixiangedu.cn

[A17] 位运算
来源：http://wc.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fl.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tr.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dz.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ug.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cj.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lh.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ky.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cn.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://gk.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://ku.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://oy.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nk.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xi.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://bg.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pw.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://yr.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://yz.newstarts.cn

[A19] 交换两个变量
来源：http://ov.9csxet.cn

Py:   a, b = b, a
来源：http://hz.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://na.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://fb.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://ja.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://sk.gzmigu.cn

Go:   a, b = b, a
来源：http://nf.huanxung.cn

Ruby: a, b = b, a
来源：http://vc.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://fe.colortex.cn

[A20] 读取标准输入
来源：http://pt.newstarts.cn

Py:   name = input("请输入：")
来源：http://uv.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nz.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eb.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://wk.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://yo.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://io.shxzukj.cn

Ruby: gets.chomp
来源：http://qa.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://kv.newstarts.cn

[A21] 保留指定小数位输出
来源：http://ia.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://dm.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bm.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://kf.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://pq.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://jr.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mf.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://md.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://cm.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://cv.colortex.cn

Py:   len(s)
来源：http://ou.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uy.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lr.lnxyls.cn

TS:   s.length
来源：http://vg.521024.cn

Java: s.length()
来源：http://fn.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xd.hnjuh.cn

Ruby: s.length
来源：http://ub.muxihuayi.cn

C#:   s.Length
来源：http://du.wgjwhj.cn

[A23] 大小写转换
来源：http://ge.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fa.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gv.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yj.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ml.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ye.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gr.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wo.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xh.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://pr.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aq.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kn.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lp.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://td.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qy.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://mf.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jf.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uv.lnxyls.cn

[A25] 字符串比较
来源：http://wt.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://bd.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qr.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jv.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qp.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aj.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kg.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vf.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ft.wgjwhj.cn

[A26] 类型转换总览
来源：http://ep.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wo.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jd.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sk.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://bc.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fv.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fn.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yz.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cx.nszjky.cn

================================================================================
来源：http://wt.jianghongdianzi.cn

B. 流程控制
来源：http://al.9csxet.cn

================================================================================
来源：http://aa.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://cl.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yx.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qd.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jx.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://io.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yg.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sc.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iw.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://cj.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jr.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ho.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kv.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bo.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jh.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ct.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ln.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ny.hnjuh.cn

[B03] switch / match / case
来源：http://ut.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lq.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oa.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qc.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jo.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ow.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rp.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mv.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wh.yuexingan06.cn

[B04] for 计数循环
来源：http://xj.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://cj.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pj.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tj.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jc.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zp.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tz.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://zw.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dr.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://nu.nicolike.cn

Py:   for item in arr: print(item)
来源：http://wt.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fs.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yr.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zg.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://an.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ac.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://uv.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://os.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://qo.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iz.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ub.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kp.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oo.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qv.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qp.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gh.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sk.nicolike.cn

[B07] while 循环
来源：http://bn.szsharing.cn

Py:   while i < 10: i += 1
来源：http://rx.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lh.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://rg.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://jp.asd995.cn

Java: while (i < 10) { i++; }
来源：http://sw.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xw.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://ex.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://ww.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://ha.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ze.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dg.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://lj.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://cr.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://nd.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mb.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yd.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://an.haigaiapp.cn

[B09] break 与 continue
来源：http://rn.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uo.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hb.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cg.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pe.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ua.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yq.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sj.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fp.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://pf.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lq.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gx.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gd.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tt.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jo.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gk.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pg.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://em.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://tk.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://rg.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://bn.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ip.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gn.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rm.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gz.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://pw.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bv.yuexingan06.cn

[B12] 跳出多层循环
来源：http://ch.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vy.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gy.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jv.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jg.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ms.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fm.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ra.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tk.jctech888.com.cn

[B13] 判断是否为数字
来源：http://cv.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://uv.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://ul.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fo.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bt.huanxung.cn

Java: x instanceof Number
来源：http://ho.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rq.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://hx.lnxyls.cn

C#:   x is int or double or decimal
来源：http://if.szsharing.cn

[B14] 判断值是否在集合内
来源：http://sf.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pf.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ge.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://nj.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://vf.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ko.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jy.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lf.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pp.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://mf.yuexingan06.cn

Py:   a and b or not c
来源：http://ur.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://ml.szxytkj.cn

JS:   a && b || !c
来源：http://ps.szxytkj.cn

TS:   a && b || !c
来源：http://mr.huixinmuqiang.cn

Java: a && b || !c
来源：http://xg.shxzukj.cn

Go:   a && b || !c
来源：http://sq.shxzukj.cn

Ruby: a && b || !c
来源：http://ni.shxzukj.cn

C#:   a && b || !c
来源：http://fb.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vd.huixiangedu.cn

Py:   if not data: return
来源：http://zn.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://ww.wgjwhj.cn

JS:   if (!data) return;
来源：http://nf.haigaiapp.cn

TS:   if (!data) return;
来源：http://wx.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://ug.huanxung.cn

Go:   if data == nil { return }
来源：http://yg.shtwfgs.cn

Ruby: return if data.nil?
来源：http://jy.szxytkj.cn

C#:   if (data == null) return;
来源：http://sw.bookmarksfly.cn

================================================================================
来源：http://wt.nicolike.cn

C. 函数与作用域
来源：http://kt.chemitech.net.cn

================================================================================
来源：http://fe.haigaiapp.cn

[C01] 定义函数
来源：http://nj.gzmigu.cn


<!-- 参考信息 -->