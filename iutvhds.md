代发 wailian999

[A14] 注释写法
来源：http://xc.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jo.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yb.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://eb.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://ms.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cy.521024.cn

Go:   // 单行；/* 多行 */
来源：http://na.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ci.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://vz.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://wj.gzmigu.cn

Py:   value = data or "默认值"
来源：http://uy.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://cl.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://qg.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://wn.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ac.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://uo.521024.cn

Ruby: value = data || "默认值"
来源：http://yu.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://hj.chemitech.net.cn

[A16] 真假值判断规则
来源：http://gd.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zp.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iq.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fe.hahajie.cn

TS:   if (!x) {}
来源：http://gz.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qc.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nh.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xm.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://do.bookmarksfly.cn

[A17] 位运算
来源：http://dv.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ag.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qg.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pt.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qz.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pw.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sz.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sj.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uk.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://zd.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://mc.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://df.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bs.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ip.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://hh.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ei.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://me.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://vs.szxytkj.cn

[A19] 交换两个变量
来源：http://zc.9csxet.cn

Py:   a, b = b, a
来源：http://wu.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ef.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://ab.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://qp.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://ia.521024.cn

Go:   a, b = b, a
来源：http://gy.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://uu.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://gs.szxytkj.cn

[A20] 读取标准输入
来源：http://mk.newstarts.cn

Py:   name = input("请输入：")
来源：http://fl.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mb.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gg.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://vm.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://fz.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rf.panjiajie.cn

Ruby: gets.chomp
来源：http://bu.newstarts.cn

C#:   Console.ReadLine();
来源：http://gj.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://em.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://ch.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://on.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://xj.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ni.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://of.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cv.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://xt.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://cb.gzmigu.cn

[A22] 获取字符串长度
来源：http://ub.lnxyls.cn

Py:   len(s)
来源：http://yz.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sx.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oq.jianghongdianzi.cn

TS:   s.length
来源：http://du.nicolike.cn

Java: s.length()
来源：http://en.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ec.newstarts.cn

Ruby: s.length
来源：http://wn.muxihuayi.cn

C#:   s.Length
来源：http://cq.yuexingan06.cn

[A23] 大小写转换
来源：http://yx.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xt.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ra.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://og.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bp.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sc.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ik.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gq.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uc.521024.cn

[A24] 去除首尾空白
来源：http://un.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rv.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wb.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xj.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yh.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kk.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://qu.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zs.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gm.hnjuh.cn

[A25] 字符串比较
来源：http://nq.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://mf.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bc.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sp.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lt.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cj.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sj.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hd.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://as.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://hv.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lt.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gn.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hi.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://av.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xb.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ie.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ga.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://me.newstarts.cn

================================================================================
来源：http://nh.9csxet.cn

B. 流程控制
来源：http://cm.szxytkj.cn

================================================================================
来源：http://jl.szxytkj.cn

[B01] 条件判断 if / else
来源：http://gs.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lu.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://so.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zh.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://na.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eb.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://co.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xn.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dq.nicolike.cn

[B02] 多分支 else if / elif
来源：http://nq.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wt.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iu.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ol.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iv.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ta.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wa.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hp.jianghongdianzi.cn

[B03] switch / match / case
来源：http://fd.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://at.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tp.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nx.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dj.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pl.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zk.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cx.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qt.huixiangedu.cn

[B04] for 计数循环
来源：http://vv.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://gf.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://al.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ij.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tn.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ml.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wu.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://hk.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hm.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://hg.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://cp.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oy.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://im.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qa.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lf.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tg.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ak.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ay.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://wj.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lc.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://af.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ky.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ad.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zk.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dl.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gf.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mu.yuntaijiaju.cn

[B07] while 循环
来源：http://wf.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://ua.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mh.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://sw.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://ur.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://pe.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qo.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://af.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://wi.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://tn.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ny.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mk.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://xu.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://cd.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://ex.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://to.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fq.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://uh.jctech888.com.cn

[B09] break 与 continue
来源：http://lp.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zl.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tp.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vm.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dg.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ee.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fm.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dh.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://re.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://cb.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zf.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hm.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ii.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mj.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ck.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sh.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wo.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dx.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://ia.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://ub.colortex.cn

PHP:  range(0, 10, 2);
来源：http://po.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fw.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://db.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nt.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://it.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://eo.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ax.shxzskj.cn

[B12] 跳出多层循环
来源：http://gw.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ua.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dh.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rl.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mf.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uo.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qk.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://st.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uw.bjjhwx.cn

[B13] 判断是否为数字
来源：http://rb.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://cq.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://vn.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kn.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jx.gzmigu.cn

Java: x instanceof Number
来源：http://pk.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jj.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://og.hahajie.cn

C#:   x is int or double or decimal
来源：http://cb.szsharing.cn

[B14] 判断值是否在集合内
来源：http://ha.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fz.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://it.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://ss.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://fq.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xn.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sb.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://op.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vw.521024.cn

[B15] 布尔运算与取反
来源：http://oq.gzmigu.cn

Py:   a and b or not c
来源：http://md.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://gf.yuntaijiaju.cn

JS:   a && b || !c
来源：http://rb.haigaiapp.cn

TS:   a && b || !c
来源：http://db.jianghongdianzi.cn

Java: a && b || !c
来源：http://gq.9csxet.cn

Go:   a && b || !c
来源：http://fx.chemitech.net.cn

Ruby: a && b || !c
来源：http://vg.shxzukj.cn

C#:   a && b || !c
来源：http://ba.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zf.nicolike.cn

Py:   if not data: return
来源：http://vb.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://ok.hnjuh.cn

JS:   if (!data) return;
来源：http://co.gzmigu.cn

TS:   if (!data) return;
来源：http://zg.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://vf.szsharing.cn

Go:   if data == nil { return }
来源：http://zo.hahajie.cn

Ruby: return if data.nil?
来源：http://tg.521024.cn

C#:   if (data == null) return;
来源：http://iu.bookmarksfly.cn

================================================================================
来源：http://gb.shxzukj.cn

C. 函数与作用域
来源：http://uh.9csxet.cn

================================================================================
来源：http://tj.yuexingan06.cn

[C01] 定义函数
来源：http://og.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://dy.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://th.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://hp.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://if.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qb.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wc.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://pp.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bm.haigaiapp.cn

[C02] 默认参数
来源：http://rg.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://su.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qv.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://jg.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mz.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jr.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uh.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://bp.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://eo.huixiangedu.cn

[C03] 可变参数
来源：http://cg.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://hy.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ut.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kt.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yo.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lt.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dl.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rx.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gr.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://tf.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vr.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aq.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gx.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sa.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://ji.asd995.cn


<!-- 参考信息 -->