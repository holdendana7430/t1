代发 wailian999

Py:   "第一行\n第二行"
来源：http://gh.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://cd.nszjky.cn

JS:   "第一行\n第二行"
来源：http://vi.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://cq.asd995.cn

Java: "第一行\n第二行"
来源：http://dr.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://bu.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://ef.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://rb.shxzskj.cn

[A14] 注释写法
来源：http://bp.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xf.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nb.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://bl.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://lh.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hd.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://tp.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vi.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://id.panjiajie.cn

[A15] 空值判断与默认值
来源：http://zx.newstarts.cn

Py:   value = data or "默认值"
来源：http://lp.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://yi.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://ks.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://ck.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rd.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://cy.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://mv.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://ut.colortex.cn

[A16] 真假值判断规则
来源：http://qa.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ra.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bj.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ky.yuexingan06.cn

TS:   if (!x) {}
来源：http://mc.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://io.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tq.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hj.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ph.jctech888.com.cn

[A17] 位运算
来源：http://oq.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iw.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mn.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gx.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gu.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rv.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://if.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vc.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jl.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://tp.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://cm.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://qx.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fi.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qr.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://kh.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fx.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://ax.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://rx.bjjhwx.cn

[A19] 交换两个变量
来源：http://ns.nszjky.cn

Py:   a, b = b, a
来源：http://zk.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zr.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://hp.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://uc.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://ky.nszjky.cn

Go:   a, b = b, a
来源：http://kw.szxytkj.cn

Ruby: a, b = b, a
来源：http://bq.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://hg.panjiajie.cn

[A20] 读取标准输入
来源：http://sj.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://yc.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jr.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bd.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://fk.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://ee.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://su.521024.cn

Ruby: gets.chomp
来源：http://vj.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://bc.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://bn.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://cq.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xb.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://wf.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://rw.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ut.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uf.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://vf.521024.cn

C#:   3.14159.ToString("F2")
来源：http://kt.muxihuayi.cn

[A22] 获取字符串长度
来源：http://ts.shxzukj.cn

Py:   len(s)
来源：http://dg.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wm.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vk.haigaiapp.cn

TS:   s.length
来源：http://yv.hnjuh.cn

Java: s.length()
来源：http://qk.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://on.huixiangedu.cn

Ruby: s.length
来源：http://ig.wgjwhj.cn

C#:   s.Length
来源：http://zn.haigaiapp.cn

[A23] 大小写转换
来源：http://nj.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vq.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wi.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cg.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qe.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yy.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iw.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bu.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gx.chemitech.net.cn

[A24] 去除首尾空白
来源：http://hg.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nh.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bu.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rx.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lm.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qn.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://oh.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gb.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ss.muxihuayi.cn

[A25] 字符串比较
来源：http://vs.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://zs.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pw.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pf.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pc.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fo.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cm.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jm.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://np.newstarts.cn

[A26] 类型转换总览
来源：http://nw.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gv.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yu.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lc.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://uf.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kn.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lj.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ji.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nh.hnjuh.cn

================================================================================
来源：http://jm.chemitech.net.cn

B. 流程控制
来源：http://no.newstarts.cn

================================================================================
来源：http://fv.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://te.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dv.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mm.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ka.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cq.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hv.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://li.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jd.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qt.newstarts.cn

[B02] 多分支 else if / elif
来源：http://up.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mi.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lo.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sj.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zw.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fo.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vt.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dx.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://an.szsharing.cn

[B03] switch / match / case
来源：http://tn.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nv.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pg.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yt.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://af.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vn.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wx.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ls.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lj.nicolike.cn

[B04] for 计数循环
来源：http://lf.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://uj.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oi.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oz.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sv.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ti.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uc.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://iu.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uu.asd995.cn

[B05] 遍历数组 / 列表
来源：http://iv.521024.cn

Py:   for item in arr: print(item)
来源：http://ie.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ht.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gh.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cw.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xj.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ie.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://cj.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cl.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://dn.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ja.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://st.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ns.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yt.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dy.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oo.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://no.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jk.yuntaijiaju.cn

[B07] while 循环
来源：http://nc.newstarts.cn

Py:   while i < 10: i += 1
来源：http://mr.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ql.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://yu.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://ea.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://jo.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mh.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://je.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://gv.521024.cn

[B08] do-while（至少执行一次）
来源：http://mw.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://di.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rk.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://ek.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://gd.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://us.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gb.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xs.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://hr.bookmarksfly.cn

[B09] break 与 continue
来源：http://ak.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dt.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ja.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://in.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ek.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eu.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://on.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ax.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pk.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://tn.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vv.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iy.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vb.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kk.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ct.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hy.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://le.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qi.521024.cn

[B11] 生成数字序列 / 区间
来源：http://ld.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://tc.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://hs.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ti.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kr.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tp.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aj.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://mx.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nq.gzmigu.cn

[B12] 跳出多层循环
来源：http://en.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jf.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wi.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cl.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ih.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://as.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rq.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bg.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ou.chemitech.net.cn

[B13] 判断是否为数字
来源：http://rb.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://iq.nicolike.cn

PHP:  is_numeric($x)
来源：http://sn.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://er.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wz.wgjwhj.cn

Java: x instanceof Number
来源：http://dd.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vr.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://vq.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://hv.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://of.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xi.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://py.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://bs.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://xt.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dz.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kx.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://px.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gk.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://wg.lnxyls.cn

Py:   a and b or not c
来源：http://yq.521024.cn

PHP:  $a && $b || !$c
来源：http://dx.shxzskj.cn

JS:   a && b || !c
来源：http://qu.panjiajie.cn

TS:   a && b || !c
来源：http://gi.bjjhwx.cn

Java: a && b || !c
来源：http://uo.colortex.cn

Go:   a && b || !c
来源：http://cy.haigaiapp.cn

Ruby: a && b || !c
来源：http://is.shtwfgs.cn

C#:   a && b || !c
来源：http://yc.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lf.nicolike.cn

Py:   if not data: return
来源：http://iv.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://ue.panjiajie.cn

JS:   if (!data) return;
来源：http://xs.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://nw.muxihuayi.cn

Java: if (data == null) return;
来源：http://xh.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://jo.9csxet.cn

Ruby: return if data.nil?
来源：http://bh.9csxet.cn

C#:   if (data == null) return;
来源：http://le.asd995.cn

================================================================================
来源：http://bp.hnjuh.cn

C. 函数与作用域
来源：http://ut.yuexingan06.cn

================================================================================
来源：http://cz.yuexingan06.cn

[C01] 定义函数
来源：http://cd.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://vi.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ak.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://zy.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dy.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dx.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ui.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://iz.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fb.chemitech.net.cn

[C02] 默认参数
来源：http://ie.521024.cn

Py:   def greet(name="World"): return name
来源：http://hj.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wq.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://tz.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dp.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://at.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://st.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://rc.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://gr.haigaiapp.cn

[C03] 可变参数
来源：http://lj.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://vx.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kj.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nf.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ls.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ja.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kz.szsharing.cn


<!-- 参考信息 -->