代发 wailian999

Py:   "第一行\n第二行"
来源：http://or.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://dh.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://fg.nszjky.cn

TS:   "第一行\n第二行"
来源：http://og.panjiajie.cn

Java: "第一行\n第二行"
来源：http://ji.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://cs.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://vb.nicolike.cn

C#:   "第一行\n第二行"
来源：http://dk.hahajie.cn

[A14] 注释写法
来源：http://ym.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ws.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qz.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://fl.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://nl.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://me.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://ha.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://om.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://id.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://mu.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://xz.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://rd.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://qc.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://ql.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ws.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://vm.nszjky.cn

Ruby: value = data || "默认值"
来源：http://oh.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://lo.hnjuh.cn

[A16] 真假值判断规则
来源：http://ka.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qc.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tm.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gj.bookmarksfly.cn

TS:   if (!x) {}
来源：http://tn.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mh.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ij.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qx.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rs.nszjky.cn

[A17] 位运算
来源：http://fr.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gn.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rh.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://po.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rb.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ji.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ir.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lo.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yu.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://zn.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://fe.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://we.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uk.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://if.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://le.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wx.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://lw.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://tl.huanxung.cn

[A19] 交换两个变量
来源：http://vc.jctech888.com.cn

Py:   a, b = b, a
来源：http://xk.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jl.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://bz.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://tl.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://nf.wgjwhj.cn

Go:   a, b = b, a
来源：http://rl.nszjky.cn

Ruby: a, b = b, a
来源：http://ob.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://it.shxzukj.cn

[A20] 读取标准输入
来源：http://rr.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://kd.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ih.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xr.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://cc.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://yy.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mu.newstarts.cn

Ruby: gets.chomp
来源：http://pz.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://yb.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://vw.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://kt.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://st.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://ry.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://ud.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://yg.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vr.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://ay.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://ub.yuexingan06.cn

[A22] 获取字符串长度
来源：http://yc.chemitech.net.cn

Py:   len(s)
来源：http://dw.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dv.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ko.hnjuh.cn

TS:   s.length
来源：http://qs.colortex.cn

Java: s.length()
来源：http://pk.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tu.shtwfgs.cn

Ruby: s.length
来源：http://uw.muxihuayi.cn

C#:   s.Length
来源：http://an.bjjhwx.cn

[A23] 大小写转换
来源：http://jb.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tp.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ps.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://py.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nf.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oi.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gn.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yg.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cl.lnxyls.cn

[A24] 去除首尾空白
来源：http://lt.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wd.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ki.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hw.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dr.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sr.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://bl.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ix.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fx.szsharing.cn

[A25] 字符串比较
来源：http://zh.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://wq.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fv.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oi.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mj.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qu.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sr.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hk.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zz.9csxet.cn

[A26] 类型转换总览
来源：http://vl.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ff.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ix.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wh.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://kl.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ip.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kl.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nd.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hp.huanxung.cn

================================================================================
来源：http://nd.muxihuayi.cn

B. 流程控制
来源：http://ng.lnxyls.cn

================================================================================
来源：http://de.shxzukj.cn

[B01] 条件判断 if / else
来源：http://xe.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wr.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ud.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bs.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vm.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eo.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ip.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://et.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rd.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://wb.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sr.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iz.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dv.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eo.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qd.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ae.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lq.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qk.shtwfgs.cn

[B03] switch / match / case
来源：http://qx.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jo.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pi.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vk.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ks.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wa.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uj.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jl.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qe.jctech888.com.cn

[B04] for 计数循环
来源：http://tt.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://pt.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rd.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ed.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bq.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uu.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ls.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://wg.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zo.asd995.cn

[B05] 遍历数组 / 列表
来源：http://vu.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://lh.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eq.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ry.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ub.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://to.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wp.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://mp.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vz.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://nx.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wk.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://es.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nv.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iy.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fv.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sc.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jq.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yu.bookmarksfly.cn

[B07] while 循环
来源：http://jb.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://vk.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vk.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://lb.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://sp.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://rz.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nm.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://sd.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://oq.colortex.cn

[B08] do-while（至少执行一次）
来源：http://cb.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://cy.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nf.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://oq.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://me.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://uv.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fy.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ha.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://iu.huixinmuqiang.cn

[B09] break 与 continue
来源：http://gb.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vo.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iq.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vl.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fc.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ov.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kh.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ps.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://dl.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hp.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pj.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rx.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yy.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jl.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fz.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ot.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yn.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://de.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://mc.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://lx.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ed.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wg.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nb.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rp.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://lt.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jp.newstarts.cn

[B12] 跳出多层循环
来源：http://px.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sl.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uk.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://br.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://of.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nj.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fs.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aa.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xr.wgjwhj.cn

[B13] 判断是否为数字
来源：http://ks.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://cf.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://wm.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ga.shxzskj.cn

Java: x instanceof Number
来源：http://tj.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ks.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://ev.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://nv.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://jt.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ke.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://le.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://sk.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://qb.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://av.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rh.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jp.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lj.nszjky.cn

[B15] 布尔运算与取反
来源：http://wm.hahajie.cn

Py:   a and b or not c
来源：http://td.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://sp.shtwfgs.cn

JS:   a && b || !c
来源：http://di.521024.cn

TS:   a && b || !c
来源：http://re.bookmarksfly.cn

Java: a && b || !c
来源：http://hb.shtwfgs.cn

Go:   a && b || !c
来源：http://mk.colortex.cn

Ruby: a && b || !c
来源：http://ho.newstarts.cn

C#:   a && b || !c
来源：http://oa.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nb.yuntaijiaju.cn

Py:   if not data: return
来源：http://wc.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://hk.shxzskj.cn

JS:   if (!data) return;
来源：http://zv.shtwfgs.cn

TS:   if (!data) return;
来源：http://pp.nszjky.cn

Java: if (data == null) return;
来源：http://kq.shxzukj.cn

Go:   if data == nil { return }
来源：http://qd.szsharing.cn

Ruby: return if data.nil?
来源：http://pj.lnxyls.cn

C#:   if (data == null) return;
来源：http://mw.haigaiapp.cn

================================================================================
来源：http://vl.shxzukj.cn

C. 函数与作用域
来源：http://ty.szxytkj.cn

================================================================================
来源：http://st.wgjwhj.cn

[C01] 定义函数
来源：http://sy.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://ok.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rq.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://kp.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ve.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dp.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qb.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://gt.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zi.huixiangedu.cn

[C02] 默认参数
来源：http://du.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://pr.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sg.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://tu.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uk.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ky.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://df.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://ww.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://ua.huixinmuqiang.cn

[C03] 可变参数
来源：http://lv.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://kx.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://an.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ut.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://od.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oo.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xw.chemitech.net.cn


<!-- 参考信息 -->