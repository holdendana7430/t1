代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qc.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://tm.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://dq.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://eh.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ae.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://bt.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://ha.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jy.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://wf.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://bx.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://fd.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://ub.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://gg.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://ew.521024.cn

Ruby: "第一行\n第二行"
来源：http://nm.szsharing.cn

C#:   "第一行\n第二行"
来源：http://eu.jctech888.com.cn

[A14] 注释写法
来源：http://zt.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ek.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bo.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://ad.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://ly.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uc.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://mf.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dm.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://mp.szsharing.cn

[A15] 空值判断与默认值
来源：http://ac.shxzskj.cn

Py:   value = data or "默认值"
来源：http://tk.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://en.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://rv.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://dm.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xy.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://ay.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://vv.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://rs.huanxung.cn

[A16] 真假值判断规则
来源：http://pb.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ji.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yd.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yl.521024.cn

TS:   if (!x) {}
来源：http://re.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qs.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zl.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yg.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fb.huixinmuqiang.cn

[A17] 位运算
来源：http://wc.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ai.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://go.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fy.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gh.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hf.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://em.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://co.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jj.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://nt.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://wd.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://it.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xk.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xu.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://ef.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ay.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://ku.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://rr.muxihuayi.cn

[A19] 交换两个变量
来源：http://jv.muxihuayi.cn

Py:   a, b = b, a
来源：http://uo.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nk.asd995.cn

JS:   [a, b] = [b, a];
来源：http://gx.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://iy.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://eu.shxzukj.cn

Go:   a, b = b, a
来源：http://yo.huixiangedu.cn

Ruby: a, b = b, a
来源：http://at.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://dn.shxzskj.cn

[A20] 读取标准输入
来源：http://fg.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://ll.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bx.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nd.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://am.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://gz.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ff.newstarts.cn

Ruby: gets.chomp
来源：http://bb.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://pq.nicolike.cn

[A21] 保留指定小数位输出
来源：http://cp.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://lz.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fw.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://zt.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://dy.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://ed.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zy.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://km.521024.cn

C#:   3.14159.ToString("F2")
来源：http://un.hahajie.cn

[A22] 获取字符串长度
来源：http://sa.9csxet.cn

Py:   len(s)
来源：http://gw.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gb.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yg.9csxet.cn

TS:   s.length
来源：http://lx.gzmigu.cn

Java: s.length()
来源：http://zo.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://je.newstarts.cn

Ruby: s.length
来源：http://ce.szsharing.cn

C#:   s.Length
来源：http://sc.chemitech.net.cn

[A23] 大小写转换
来源：http://fk.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jg.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sc.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pa.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ai.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://is.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jp.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wo.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hc.wgjwhj.cn

[A24] 去除首尾空白
来源：http://ro.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pv.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xu.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://co.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vp.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ga.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://ea.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qp.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wl.yuntaijiaju.cn

[A25] 字符串比较
来源：http://cj.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://rb.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jk.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aa.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hw.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://om.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lp.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qv.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ew.yuexingan06.cn

[A26] 类型转换总览
来源：http://dq.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nw.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sz.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ts.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://gw.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://to.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uv.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yt.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ka.huixinmuqiang.cn

================================================================================
来源：http://xq.szsharing.cn

B. 流程控制
来源：http://rr.hahajie.cn

================================================================================
来源：http://ls.huanxung.cn

[B01] 条件判断 if / else
来源：http://jr.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://np.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lt.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xk.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://po.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nf.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aj.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ag.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ml.colortex.cn

[B02] 多分支 else if / elif
来源：http://ma.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mo.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dx.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ei.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ap.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nw.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://io.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cx.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nv.hnjuh.cn

[B03] switch / match / case
来源：http://xw.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ga.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://le.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nu.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vh.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rk.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ax.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yq.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bd.bookmarksfly.cn

[B04] for 计数循环
来源：http://rt.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://mx.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tv.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oe.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cc.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sj.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uu.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://gd.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ft.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://cg.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://yk.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://db.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hc.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uj.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hm.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hj.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://ub.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cr.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://sh.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iv.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zp.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kl.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://on.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ne.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://te.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tr.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yp.bookmarksfly.cn

[B07] while 循环
来源：http://kq.nszjky.cn

Py:   while i < 10: i += 1
来源：http://qa.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qn.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://bi.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://xt.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://bh.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wy.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://fw.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://ie.521024.cn

[B08] do-while（至少执行一次）
来源：http://fr.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://jj.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hu.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://xt.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://bn.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://sq.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ha.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qe.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://lt.shxzskj.cn

[B09] break 与 continue
来源：http://od.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://os.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ci.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lz.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://md.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pe.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bq.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qc.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jn.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://tl.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yq.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sb.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yj.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ha.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qf.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://br.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hl.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dx.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://ml.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://hd.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://qi.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jo.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fl.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kq.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jl.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://by.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tv.huanxung.cn

[B12] 跳出多层循环
来源：http://wv.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xc.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://en.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ke.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ua.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ip.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xk.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xr.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wc.newstarts.cn

[B13] 判断是否为数字
来源：http://uc.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://ck.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://cg.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://li.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nv.bookmarksfly.cn

Java: x instanceof Number
来源：http://gl.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xi.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://dn.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://wf.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://gb.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bv.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zw.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://dd.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://gn.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gs.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nt.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bp.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://he.shxzskj.cn

[B15] 布尔运算与取反
来源：http://de.shxzskj.cn

Py:   a and b or not c
来源：http://wo.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://wm.huanxung.cn

JS:   a && b || !c
来源：http://xr.jianghongdianzi.cn

TS:   a && b || !c
来源：http://sf.gzmigu.cn

Java: a && b || !c
来源：http://pz.panjiajie.cn

Go:   a && b || !c
来源：http://vr.yuexingan06.cn

Ruby: a && b || !c
来源：http://ey.huixiangedu.cn

C#:   a && b || !c
来源：http://gb.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://as.huanxung.cn

Py:   if not data: return
来源：http://hd.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://bf.muxihuayi.cn

JS:   if (!data) return;
来源：http://cl.bjjhwx.cn

TS:   if (!data) return;
来源：http://of.asd995.cn

Java: if (data == null) return;
来源：http://sh.newstarts.cn

Go:   if data == nil { return }
来源：http://wt.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://ax.colortex.cn

C#:   if (data == null) return;
来源：http://eo.nszjky.cn

================================================================================
来源：http://hv.huixinmuqiang.cn

C. 函数与作用域
来源：http://ky.jianghongdianzi.cn

================================================================================
来源：http://ww.newstarts.cn

[C01] 定义函数
来源：http://bw.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://nu.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eu.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://se.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aq.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mh.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://te.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://lw.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ox.hnjuh.cn

[C02] 默认参数
来源：http://iv.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://xz.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://td.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://sl.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zf.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ms.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mg.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://ku.jctech888.com.cn


<!-- 参考信息 -->