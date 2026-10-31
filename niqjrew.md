代发 wailian999

Py:   "第一行\n第二行"
来源：http://do.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://eh.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://vx.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://cs.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://ip.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://de.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://ma.nszjky.cn

C#:   "第一行\n第二行"
来源：http://yw.lnxyls.cn

[A14] 注释写法
来源：http://yu.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sj.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ui.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://ik.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://mw.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pr.521024.cn

Go:   // 单行；/* 多行 */
来源：http://xl.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jn.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://cc.szsharing.cn

[A15] 空值判断与默认值
来源：http://qr.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://no.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://nf.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://wz.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://mv.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oe.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://pz.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://fl.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://hu.shxzukj.cn

[A16] 真假值判断规则
来源：http://lw.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fo.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nw.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ut.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://uj.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gz.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://il.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cw.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yr.lnxyls.cn

[A17] 位运算
来源：http://gl.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nj.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yy.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oe.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oz.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ja.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tn.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://da.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tr.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://bt.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://bf.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://ui.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hp.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ye.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://ry.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qt.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://qu.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://ah.newstarts.cn

[A19] 交换两个变量
来源：http://vo.asd995.cn

Py:   a, b = b, a
来源：http://ft.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uh.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://bg.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://dg.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://jl.bookmarksfly.cn

Go:   a, b = b, a
来源：http://vy.newstarts.cn

Ruby: a, b = b, a
来源：http://nw.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://fh.jctech888.com.cn

[A20] 读取标准输入
来源：http://nd.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://sf.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aj.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nf.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://il.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://oe.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gq.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://cx.9csxet.cn

C#:   Console.ReadLine();
来源：http://rp.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://wg.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://un.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jj.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://gz.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://ut.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://os.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lh.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://rj.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://va.wgjwhj.cn

[A22] 获取字符串长度
来源：http://gf.jctech888.com.cn

Py:   len(s)
来源：http://da.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://es.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fl.haigaiapp.cn

TS:   s.length
来源：http://cj.yuexingan06.cn

Java: s.length()
来源：http://un.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ib.jctech888.com.cn

Ruby: s.length
来源：http://oi.huixinmuqiang.cn

C#:   s.Length
来源：http://eq.yuntaijiaju.cn

[A23] 大小写转换
来源：http://er.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ke.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gj.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qy.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vz.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ql.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zp.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bt.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vk.haigaiapp.cn

[A24] 去除首尾空白
来源：http://nn.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rt.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bz.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lx.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lp.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yd.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://jc.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wn.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://re.shtwfgs.cn

[A25] 字符串比较
来源：http://vu.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://bo.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lk.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zb.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gv.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vx.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xi.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ci.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nx.szxytkj.cn

[A26] 类型转换总览
来源：http://gs.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kd.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aj.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ca.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://ux.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qq.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yc.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zc.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pc.nicolike.cn

================================================================================
来源：http://me.newstarts.cn

B. 流程控制
来源：http://so.521024.cn

================================================================================
来源：http://kz.nszjky.cn

[B01] 条件判断 if / else
来源：http://xo.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nk.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xh.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wm.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://al.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oq.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qy.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gc.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cc.szsharing.cn

[B02] 多分支 else if / elif
来源：http://dv.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ku.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xq.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kn.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ky.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yp.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oj.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uf.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nz.bookmarksfly.cn

[B03] switch / match / case
来源：http://eb.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jo.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rj.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kf.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hs.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sq.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iw.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://no.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rp.huanxung.cn

[B04] for 计数循环
来源：http://qa.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://al.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mx.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ql.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tk.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ik.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ie.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://vc.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sk.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://dv.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://yq.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zy.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qk.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rn.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fa.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gn.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://fc.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qx.521024.cn

[B06] 遍历字典 / 对象
来源：http://yw.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ht.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gv.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nc.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nw.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wk.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bz.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nj.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kw.gzmigu.cn

[B07] while 循环
来源：http://uq.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://du.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oc.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://lm.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://qd.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://fh.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yd.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://dq.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://ie.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://wb.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://ap.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vb.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://bx.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://ua.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://vb.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ot.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qv.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://bc.muxihuayi.cn

[B09] break 与 continue
来源：http://dp.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ie.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jy.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qe.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jt.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lc.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xr.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yg.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vj.521024.cn

[B10] 遍历同时拿索引
来源：http://tx.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aj.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fi.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rb.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sl.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hg.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qo.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lm.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ft.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://fx.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://kf.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://qj.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://da.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zl.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jw.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yv.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://wt.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tp.lnxyls.cn

[B12] 跳出多层循环
来源：http://qm.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tt.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ng.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xw.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://we.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tw.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tc.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://af.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ws.colortex.cn

[B13] 判断是否为数字
来源：http://jp.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://gi.huanxung.cn

PHP:  is_numeric($x)
来源：http://bc.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rr.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bf.521024.cn

Java: x instanceof Number
来源：http://ul.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wj.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://oq.colortex.cn

C#:   x is int or double or decimal
来源：http://ce.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://wy.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hk.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vx.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://wn.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://yh.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pr.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yt.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sg.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nj.asd995.cn

[B15] 布尔运算与取反
来源：http://kd.shxzskj.cn

Py:   a and b or not c
来源：http://qe.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://rt.huixiangedu.cn

JS:   a && b || !c
来源：http://kc.wgjwhj.cn

TS:   a && b || !c
来源：http://cx.wgjwhj.cn

Java: a && b || !c
来源：http://gc.huanxung.cn

Go:   a && b || !c
来源：http://ak.9csxet.cn

Ruby: a && b || !c
来源：http://sb.lnxyls.cn

C#:   a && b || !c
来源：http://rt.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mz.shxzukj.cn

Py:   if not data: return
来源：http://ol.asd995.cn

PHP:  if (!$data) { return; }
来源：http://nn.lnxyls.cn

JS:   if (!data) return;
来源：http://wr.bjjhwx.cn

TS:   if (!data) return;
来源：http://nd.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://wi.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://ss.panjiajie.cn

Ruby: return if data.nil?
来源：http://le.colortex.cn

C#:   if (data == null) return;
来源：http://xm.gzmigu.cn

================================================================================
来源：http://jx.hahajie.cn

C. 函数与作用域
来源：http://tq.nszjky.cn

================================================================================
来源：http://hf.haigaiapp.cn

[C01] 定义函数
来源：http://hn.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://nd.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yy.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://nv.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ql.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mh.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wo.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://jt.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dy.yuexingan06.cn

[C02] 默认参数
来源：http://ex.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://if.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vo.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://aj.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mp.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lk.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mm.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://jg.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://sm.jianghongdianzi.cn

[C03] 可变参数
来源：http://dr.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://wj.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jm.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://az.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vt.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ow.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sf.shxzukj.cn


<!-- 参考信息 -->