代发 wailian999

Ruby: value = data || "默认值"
来源：http://tq.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://xv.lnxyls.cn

[A16] 真假值判断规则
来源：http://vb.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kp.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nv.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tm.hnjuh.cn

TS:   if (!x) {}
来源：http://pw.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tt.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oy.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cu.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dw.colortex.cn

[A17] 位运算
来源：http://cs.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nc.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ua.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qx.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hj.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vu.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ux.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://as.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lv.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://xe.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://xv.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://dz.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uh.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://za.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://ea.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ej.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://su.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://dc.yuexingan06.cn

[A19] 交换两个变量
来源：http://cp.wgjwhj.cn

Py:   a, b = b, a
来源：http://kf.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vf.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://ez.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://ci.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://ay.panjiajie.cn

Go:   a, b = b, a
来源：http://fj.asd995.cn

Ruby: a, b = b, a
来源：http://sq.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://eh.szsharing.cn

[A20] 读取标准输入
来源：http://gn.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://np.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gx.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://px.asd995.cn

TS:   // Node.js：readline 模块
来源：http://vm.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://qk.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ev.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://hn.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://od.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://de.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://yq.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nc.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://qy.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://pj.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://oh.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tu.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ld.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://ap.huixiangedu.cn

[A22] 获取字符串长度
来源：http://qg.huixiangedu.cn

Py:   len(s)
来源：http://ru.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mu.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fu.muxihuayi.cn

TS:   s.length
来源：http://ko.huixiangedu.cn

Java: s.length()
来源：http://pp.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bd.wgjwhj.cn

Ruby: s.length
来源：http://bx.panjiajie.cn

C#:   s.Length
来源：http://bp.shxzskj.cn

[A23] 大小写转换
来源：http://ak.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zb.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kq.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qa.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lf.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hs.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://km.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ic.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xa.newstarts.cn

[A24] 去除首尾空白
来源：http://rl.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rx.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kx.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ec.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ch.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rz.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://hl.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nh.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oa.szxytkj.cn

[A25] 字符串比较
来源：http://yd.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://uq.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uw.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://an.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://do.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wd.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hj.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qy.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jl.colortex.cn

[A26] 类型转换总览
来源：http://lw.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ph.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mq.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://go.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://hd.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tu.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ni.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://is.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fq.asd995.cn

================================================================================
来源：http://vf.wgjwhj.cn

B. 流程控制
来源：http://nv.bjjhwx.cn

================================================================================
来源：http://jm.hnjuh.cn

[B01] 条件判断 if / else
来源：http://lz.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ct.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sz.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wv.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ws.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ch.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vs.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zk.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://an.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://bx.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ar.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zt.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uf.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bm.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xt.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kf.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fo.yuntaijiaju.cn

[B03] switch / match / case
来源：http://cr.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yu.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hn.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yb.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jz.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qg.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hd.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://du.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://si.colortex.cn

[B04] for 计数循环
来源：http://ks.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://qa.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sp.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ya.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://el.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eu.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sd.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://bi.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ig.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://sm.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://co.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ee.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zw.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ws.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bi.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gw.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://vz.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ac.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://xy.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xw.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bi.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://af.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tm.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qq.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ji.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gr.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yy.panjiajie.cn

[B07] while 循环
来源：http://rb.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://kg.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://of.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://ss.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://xl.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://nz.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ec.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://tm.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://oq.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://fz.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://sl.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cm.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://lc.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://zt.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://de.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nk.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jx.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://qh.newstarts.cn

[B09] break 与 continue
来源：http://tl.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rs.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ik.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xg.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ux.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rn.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ne.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qk.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ri.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://zm.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wt.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dd.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ga.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qx.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eq.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tp.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aj.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lc.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://hj.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://sl.521024.cn

PHP:  range(0, 10, 2);
来源：http://ox.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nv.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hn.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ac.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vf.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://je.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://du.szsharing.cn

[B12] 跳出多层循环
来源：http://yi.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gm.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ex.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kb.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xm.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://js.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oq.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yi.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cb.wgjwhj.cn

[B13] 判断是否为数字
来源：http://cc.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://ie.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://vm.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pb.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qx.jianghongdianzi.cn

Java: x instanceof Number
来源：http://wh.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xd.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://tm.szxytkj.cn

C#:   x is int or double or decimal
来源：http://dq.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://iz.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cb.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lo.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://gk.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://ec.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eg.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oj.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wf.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hd.huanxung.cn

[B15] 布尔运算与取反
来源：http://aj.nicolike.cn

Py:   a and b or not c
来源：http://kv.colortex.cn

PHP:  $a && $b || !$c
来源：http://mm.colortex.cn

JS:   a && b || !c
来源：http://ih.hahajie.cn

TS:   a && b || !c
来源：http://cq.nicolike.cn

Java: a && b || !c
来源：http://se.huixinmuqiang.cn

Go:   a && b || !c
来源：http://bt.521024.cn

Ruby: a && b || !c
来源：http://pi.nszjky.cn

C#:   a && b || !c
来源：http://eo.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ak.jctech888.com.cn

Py:   if not data: return
来源：http://dx.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://lr.lnxyls.cn

JS:   if (!data) return;
来源：http://vk.haigaiapp.cn

TS:   if (!data) return;
来源：http://oz.huanxung.cn

Java: if (data == null) return;
来源：http://ap.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://fx.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://iz.shtwfgs.cn

C#:   if (data == null) return;
来源：http://ua.shxzukj.cn

================================================================================
来源：http://rp.hahajie.cn

C. 函数与作用域
来源：http://sh.shtwfgs.cn

================================================================================
来源：http://uc.lnxyls.cn

[C01] 定义函数
来源：http://vk.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://vn.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pc.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://ii.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yi.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gn.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jc.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://wy.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gg.shxzukj.cn

[C02] 默认参数
来源：http://gl.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://tp.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oh.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://pu.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://du.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fz.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wh.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://hx.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://fk.yuntaijiaju.cn

[C03] 可变参数
来源：http://uo.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://mr.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://co.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zv.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bk.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sl.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yb.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lo.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pe.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://ud.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cu.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fd.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bp.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ml.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://nl.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://hg.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://gq.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://qu.bookmarksfly.cn

[C05] 返回多个值
来源：http://rw.hnjuh.cn

Py:   return a, b
来源：http://aj.huanxung.cn

PHP:  return [$a, $b];
来源：http://ro.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gv.bjjhwx.cn

TS:   return { a, b };
来源：http://wn.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cg.hnjuh.cn

Go:   return a, b
来源：http://bi.lnxyls.cn

Ruby: return a, b
来源：http://sh.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://zf.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://eh.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://um.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cf.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://px.chemitech.net.cn


<!-- 参考信息 -->