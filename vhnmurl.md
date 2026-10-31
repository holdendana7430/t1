代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mh.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nx.shxzukj.cn

TS:   if (!x) {}
来源：http://jt.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zo.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://st.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://le.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://os.szxytkj.cn

[A17] 位运算
来源：http://eu.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jl.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ck.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dn.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fc.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yk.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bg.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zx.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://df.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://on.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://ix.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://qk.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pw.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://at.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://yl.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vx.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://ku.521024.cn

C#:   (int)'A'; (char)65
来源：http://ht.shxzskj.cn

[A19] 交换两个变量
来源：http://qj.bookmarksfly.cn

Py:   a, b = b, a
来源：http://yi.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qd.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://rq.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://kl.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://bk.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://rb.nicolike.cn

Ruby: a, b = b, a
来源：http://iq.521024.cn

C#:   (a, b) = (b, a);
来源：http://se.shtwfgs.cn

[A20] 读取标准输入
来源：http://hj.gzmigu.cn

Py:   name = input("请输入：")
来源：http://gd.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://re.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://es.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://ms.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://em.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jv.huixiangedu.cn

Ruby: gets.chomp
来源：http://vt.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://iy.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://dr.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://pz.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ce.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://tv.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://dm.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://wr.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vv.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://be.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://tu.yuexingan06.cn

[A22] 获取字符串长度
来源：http://ff.nicolike.cn

Py:   len(s)
来源：http://ok.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rc.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hd.szsharing.cn

TS:   s.length
来源：http://fw.haigaiapp.cn

Java: s.length()
来源：http://jr.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xa.jctech888.com.cn

Ruby: s.length
来源：http://wu.newstarts.cn

C#:   s.Length
来源：http://xc.szsharing.cn

[A23] 大小写转换
来源：http://hn.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cd.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xd.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ew.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fq.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gy.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://af.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fz.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ns.hnjuh.cn

[A24] 去除首尾空白
来源：http://sn.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yv.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qg.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kl.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://at.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ao.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://sc.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qv.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qy.jctech888.com.cn

[A25] 字符串比较
来源：http://ce.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://yg.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://md.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ai.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sl.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jx.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yh.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qx.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wj.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://zh.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kj.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vb.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fz.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://dd.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iy.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bj.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wi.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jp.newstarts.cn

================================================================================
来源：http://da.yuexingan06.cn

B. 流程控制
来源：http://kh.jctech888.com.cn

================================================================================
来源：http://ib.gzmigu.cn

[B01] 条件判断 if / else
来源：http://gq.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ey.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ra.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kl.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yo.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lo.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uh.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sg.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cx.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://ox.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eh.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aw.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://si.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ik.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dq.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ab.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gm.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.haigaiapp.cn

[B03] switch / match / case
来源：http://jn.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://or.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xb.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mo.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vq.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zi.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://us.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rc.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://th.nszjky.cn

[B04] for 计数循环
来源：http://kb.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://vl.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tx.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mt.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wn.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lf.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fn.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://jb.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mm.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://hu.szsharing.cn

Py:   for item in arr: print(item)
来源：http://xj.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lm.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mc.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ra.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wa.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ct.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://ne.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ik.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://xs.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ot.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kc.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wh.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xu.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://up.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yi.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://op.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qp.huixiangedu.cn

[B07] while 循环
来源：http://ot.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://wz.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pd.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://fz.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://co.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://rq.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://al.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://kp.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://fy.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://yq.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ze.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ps.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://iz.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://eu.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://hq.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pb.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ab.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://sn.muxihuayi.cn

[B09] break 与 continue
来源：http://fg.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fp.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tn.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hj.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bb.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tb.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://of.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vw.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nr.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://xw.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rn.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gg.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fd.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wo.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ox.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mq.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sp.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wt.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://uy.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://zw.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://zt.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qe.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fj.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pl.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://az.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://of.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zd.jctech888.com.cn

[B12] 跳出多层循环
来源：http://hn.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dr.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bk.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://by.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kz.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ad.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dg.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fi.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nu.szxytkj.cn

[B13] 判断是否为数字
来源：http://yg.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://hk.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://ra.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uh.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ue.haigaiapp.cn

Java: x instanceof Number
来源：http://co.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jn.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://vm.shxzukj.cn

C#:   x is int or double or decimal
来源：http://nr.newstarts.cn

[B14] 判断值是否在集合内
来源：http://wx.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yx.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zm.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://hy.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://ep.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://am.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ff.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ty.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zv.newstarts.cn

[B15] 布尔运算与取反
来源：http://xp.wgjwhj.cn

Py:   a and b or not c
来源：http://uh.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://mh.bookmarksfly.cn

JS:   a && b || !c
来源：http://cv.yuexingan06.cn

TS:   a && b || !c
来源：http://fe.newstarts.cn

Java: a && b || !c
来源：http://xq.wgjwhj.cn

Go:   a && b || !c
来源：http://wq.huanxung.cn

Ruby: a && b || !c
来源：http://ks.9csxet.cn

C#:   a && b || !c
来源：http://kh.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ej.nicolike.cn

Py:   if not data: return
来源：http://qw.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://rv.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://ei.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://mn.521024.cn

Java: if (data == null) return;
来源：http://jn.shtwfgs.cn

Go:   if data == nil { return }
来源：http://zy.wgjwhj.cn

Ruby: return if data.nil?
来源：http://ag.wgjwhj.cn

C#:   if (data == null) return;
来源：http://nj.haigaiapp.cn

================================================================================
来源：http://ho.lnxyls.cn

C. 函数与作用域
来源：http://nw.szsharing.cn

================================================================================
来源：http://ru.hnjuh.cn

[C01] 定义函数
来源：http://yl.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://nx.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ga.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://al.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mt.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cn.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dq.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://my.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ls.haigaiapp.cn

[C02] 默认参数
来源：http://mq.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://zu.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tj.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://sh.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dh.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ya.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gf.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://mj.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://qd.huanxung.cn

[C03] 可变参数
来源：http://sh.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://de.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rd.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yl.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dm.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://an.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gg.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yd.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nd.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://ns.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ks.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ce.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fh.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://py.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://rs.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://ox.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ol.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://bj.shxzskj.cn

[C05] 返回多个值
来源：http://cw.huanxung.cn

Py:   return a, b
来源：http://tt.hahajie.cn

PHP:  return [$a, $b];
来源：http://tt.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ac.huanxung.cn

TS:   return { a, b };
来源：http://nl.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vj.hnjuh.cn

Go:   return a, b
来源：http://qh.asd995.cn

Ruby: return a, b
来源：http://jz.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ih.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://bq.szsharing.cn

Py:   square = lambda x: x * x
来源：http://pj.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://va.colortex.cn

JS:   const square = x => x * x;
来源：http://ik.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://kw.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yy.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ut.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://fr.yuntaijiaju.cn


<!-- 参考信息 -->