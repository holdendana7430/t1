代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lm.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://yp.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kz.huixiangedu.cn

Ruby: rand(1..100)
来源：http://gu.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://ms.521024.cn

[A11] 条件表达式（三元）
来源：http://lt.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://ih.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nd.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xq.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yp.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://vd.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lh.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nt.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kv.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://oe.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://af.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dj.asd995.cn

JS:   `Hello, ${name}!`
来源：http://eg.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://jw.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://xd.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://be.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://kj.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://pw.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mk.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://kx.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://fl.asd995.cn

JS:   "第一行\n第二行"
来源：http://py.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://sq.9csxet.cn

Java: "第一行\n第二行"
来源：http://sj.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://at.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://gb.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://vo.szsharing.cn

[A14] 注释写法
来源：http://lf.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://um.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hv.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://ad.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://zw.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dm.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://kr.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jy.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://id.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://qz.panjiajie.cn

Py:   value = data or "默认值"
来源：http://hp.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://oz.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://qg.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://um.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hl.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://wt.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://wj.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://fm.asd995.cn

[A16] 真假值判断规则
来源：http://ta.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hj.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ik.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://to.muxihuayi.cn

TS:   if (!x) {}
来源：http://ze.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sg.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yo.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ui.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sv.bjjhwx.cn

[A17] 位运算
来源：http://lo.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ki.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zx.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://al.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://au.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://po.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uh.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://if.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tx.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://kq.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://kw.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://ue.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pc.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mz.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://bv.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fi.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://xi.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://rx.bookmarksfly.cn

[A19] 交换两个变量
来源：http://xz.chemitech.net.cn

Py:   a, b = b, a
来源：http://we.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ak.colortex.cn

JS:   [a, b] = [b, a];
来源：http://fn.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://iy.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://bb.szxytkj.cn

Go:   a, b = b, a
来源：http://ho.shxzukj.cn

Ruby: a, b = b, a
来源：http://fo.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://at.asd995.cn

[A20] 读取标准输入
来源：http://gt.nicolike.cn

Py:   name = input("请输入：")
来源：http://pd.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://on.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ks.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://my.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://hc.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zr.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://tx.hnjuh.cn

C#:   Console.ReadLine();
来源：http://ie.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://tv.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://xl.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sd.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ad.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://yh.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://dk.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gv.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://tu.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://kf.shxzskj.cn

[A22] 获取字符串长度
来源：http://te.lnxyls.cn

Py:   len(s)
来源：http://ar.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ka.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wc.lnxyls.cn

TS:   s.length
来源：http://ij.muxihuayi.cn

Java: s.length()
来源：http://sc.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fw.hahajie.cn

Ruby: s.length
来源：http://bz.bjjhwx.cn

C#:   s.Length
来源：http://ul.yuntaijiaju.cn

[A23] 大小写转换
来源：http://fj.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dw.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cb.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yx.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sh.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nb.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nv.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ic.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eq.huanxung.cn

[A24] 去除首尾空白
来源：http://mz.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iz.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kq.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pb.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bo.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vq.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://ng.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wy.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tr.asd995.cn

[A25] 字符串比较
来源：http://ff.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://ym.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pa.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jg.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lz.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rn.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oi.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pd.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hx.panjiajie.cn

[A26] 类型转换总览
来源：http://av.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sy.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://es.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cn.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://tw.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jd.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ji.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lv.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ej.shxzukj.cn

================================================================================
来源：http://ev.yuexingan06.cn

B. 流程控制
来源：http://xc.chemitech.net.cn

================================================================================
来源：http://av.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://jz.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://db.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mv.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ry.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yn.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gm.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ui.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bw.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tm.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://pl.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uv.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zt.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hb.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ci.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ko.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gn.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ag.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.huixiangedu.cn

[B03] switch / match / case
来源：http://hc.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://np.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qy.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ut.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mv.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sm.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xj.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gb.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ss.colortex.cn

[B04] for 计数循环
来源：http://ea.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://ue.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pq.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xd.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://df.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mg.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lt.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://lf.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mf.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://ir.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://wo.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wn.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xb.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yy.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://st.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://up.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://vx.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sk.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://aj.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ig.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yt.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cg.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ft.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bc.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yv.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mm.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bn.9csxet.cn

[B07] while 循环
来源：http://rv.newstarts.cn

Py:   while i < 10: i += 1
来源：http://cd.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qr.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://gc.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://th.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://gh.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yq.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://bu.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://wi.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://ei.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://cq.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vu.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://um.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://mc.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://uv.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yg.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xm.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://eh.asd995.cn

[B09] break 与 continue
来源：http://zd.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ur.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ad.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zc.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fv.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://su.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lp.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://od.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ez.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://ht.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://du.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tv.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pt.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sn.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gf.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sq.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tz.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bv.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://sz.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://xi.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://mi.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ys.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ue.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ji.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gn.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://cx.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mp.521024.cn

[B12] 跳出多层循环
来源：http://ml.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lj.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mj.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kp.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hx.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dr.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yr.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iv.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fl.szxytkj.cn

[B13] 判断是否为数字
来源：http://yj.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://dg.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://jf.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tv.gzmigu.cn

Java: x instanceof Number
来源：http://dy.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rr.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://sc.gzmigu.cn

C#:   x is int or double or decimal
来源：http://sh.hahajie.cn

[B14] 判断值是否在集合内
来源：http://if.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ju.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rj.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ab.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://zu.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vu.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rp.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qs.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kr.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://cj.yuexingan06.cn

Py:   a and b or not c
来源：http://nr.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://lh.shxzukj.cn

JS:   a && b || !c
来源：http://fi.shxzukj.cn

TS:   a && b || !c
来源：http://nq.szsharing.cn

Java: a && b || !c
来源：http://hy.jianghongdianzi.cn

Go:   a && b || !c
来源：http://tl.bjjhwx.cn

Ruby: a && b || !c
来源：http://ye.chemitech.net.cn

C#:   a && b || !c
来源：http://fw.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cc.shtwfgs.cn

Py:   if not data: return
来源：http://om.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://pa.wgjwhj.cn

JS:   if (!data) return;
来源：http://zm.asd995.cn

TS:   if (!data) return;
来源：http://qm.asd995.cn

Java: if (data == null) return;
来源：http://im.shxzskj.cn

Go:   if data == nil { return }
来源：http://wl.9csxet.cn

Ruby: return if data.nil?
来源：http://el.gzmigu.cn

C#:   if (data == null) return;
来源：http://jd.szsharing.cn

================================================================================
来源：http://oz.szsharing.cn

C. 函数与作用域
来源：http://lf.haigaiapp.cn

================================================================================
来源：http://bs.shxzukj.cn

[C01] 定义函数
来源：http://qf.asd995.cn


<!-- 参考信息 -->