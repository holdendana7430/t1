代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://cj.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://yx.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rx.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://zs.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://uj.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://zr.9csxet.cn

[A16] 真假值判断规则
来源：http://iy.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dq.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://go.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ci.gzmigu.cn

TS:   if (!x) {}
来源：http://ey.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kl.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ju.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://af.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gr.shxzskj.cn

[A17] 位运算
来源：http://ji.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nx.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dh.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qn.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nu.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oa.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nh.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rm.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://fu.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://gc.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://kb.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aa.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ii.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://mf.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sz.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://yj.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://rt.panjiajie.cn

[A19] 交换两个变量
来源：http://rs.huanxung.cn

Py:   a, b = b, a
来源：http://ch.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jc.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://ys.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://rk.521024.cn

Java: int t = a; a = b; b = t;
来源：http://zx.shtwfgs.cn

Go:   a, b = b, a
来源：http://xy.shtwfgs.cn

Ruby: a, b = b, a
来源：http://kd.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://ca.huixiangedu.cn

[A20] 读取标准输入
来源：http://np.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://kk.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sa.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ty.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://sa.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ea.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dq.shxzskj.cn

Ruby: gets.chomp
来源：http://be.gzmigu.cn

C#:   Console.ReadLine();
来源：http://ga.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://fm.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://gc.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zo.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://sf.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://op.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://mf.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ha.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://mu.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://xy.shtwfgs.cn

[A22] 获取字符串长度
来源：http://gz.chemitech.net.cn

Py:   len(s)
来源：http://ac.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cg.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ew.haigaiapp.cn

TS:   s.length
来源：http://sr.chemitech.net.cn

Java: s.length()
来源：http://rm.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wu.yuexingan06.cn

Ruby: s.length
来源：http://hi.asd995.cn

C#:   s.Length
来源：http://rx.bjjhwx.cn

[A23] 大小写转换
来源：http://dj.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zp.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://um.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ik.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://na.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://so.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cj.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oa.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fm.9csxet.cn

[A24] 去除首尾空白
来源：http://xs.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ok.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dz.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mx.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pq.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cu.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://qs.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vf.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kp.szsharing.cn

[A25] 字符串比较
来源：http://ce.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://oh.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xa.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qj.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jw.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eh.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gs.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://am.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wk.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://yz.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://is.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uw.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bz.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://hh.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wx.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ii.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://go.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nc.hnjuh.cn

================================================================================
来源：http://ov.hahajie.cn

B. 流程控制
来源：http://ls.bjjhwx.cn

================================================================================
来源：http://ym.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://is.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cw.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wv.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lr.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ww.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ut.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mf.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jz.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ev.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://tc.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vw.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zf.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nt.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gh.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ai.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bz.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://if.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://og.yuntaijiaju.cn

[B03] switch / match / case
来源：http://en.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yv.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ye.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kg.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kg.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mz.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tr.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://at.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cq.yuexingan06.cn

[B04] for 计数循环
来源：http://uq.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://zi.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ce.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iq.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ut.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kh.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ig.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://ie.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ra.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://ng.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://xs.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wp.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yu.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ki.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dr.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zt.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://wx.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nw.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://lg.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pt.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dn.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ay.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dq.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yc.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vn.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nz.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://di.gzmigu.cn

[B07] while 循环
来源：http://ml.szsharing.cn

Py:   while i < 10: i += 1
来源：http://fy.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rn.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://fr.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://bo.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://fy.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bl.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://ae.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://pa.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://bm.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://xw.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cm.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://ae.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://pd.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://zp.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wg.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yw.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://va.shtwfgs.cn

[B09] break 与 continue
来源：http://ns.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ia.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wd.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sz.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://je.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cy.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xd.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tk.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://md.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://fl.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://le.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ly.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sk.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ql.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nk.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ld.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ft.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ai.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://kj.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://ko.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://tp.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ci.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gh.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wt.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cs.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://gb.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ko.bjjhwx.cn

[B12] 跳出多层循环
来源：http://yg.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cp.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rp.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://st.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://if.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hk.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://su.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://es.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://na.muxihuayi.cn

[B13] 判断是否为数字
来源：http://ez.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://xg.asd995.cn

PHP:  is_numeric($x)
来源：http://my.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gz.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vd.huixiangedu.cn

Java: x instanceof Number
来源：http://xl.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xz.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://kx.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://pt.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://jj.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pr.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sj.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://wx.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://qb.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dw.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fk.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qx.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rt.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://is.nicolike.cn

Py:   a and b or not c
来源：http://ny.asd995.cn

PHP:  $a && $b || !$c
来源：http://pp.muxihuayi.cn

JS:   a && b || !c
来源：http://jt.wgjwhj.cn

TS:   a && b || !c
来源：http://be.yuexingan06.cn

Java: a && b || !c
来源：http://nl.jctech888.com.cn

Go:   a && b || !c
来源：http://rl.yuexingan06.cn

Ruby: a && b || !c
来源：http://os.shxzskj.cn

C#:   a && b || !c
来源：http://bb.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nb.shxzukj.cn

Py:   if not data: return
来源：http://gz.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://ud.shxzukj.cn

JS:   if (!data) return;
来源：http://wa.hnjuh.cn

TS:   if (!data) return;
来源：http://lk.chemitech.net.cn

Java: if (data == null) return;
来源：http://qh.huanxung.cn

Go:   if data == nil { return }
来源：http://mm.gzmigu.cn

Ruby: return if data.nil?
来源：http://uf.haigaiapp.cn

C#:   if (data == null) return;
来源：http://fw.hnjuh.cn

================================================================================
来源：http://ra.jianghongdianzi.cn

C. 函数与作用域
来源：http://oi.newstarts.cn

================================================================================
来源：http://yc.yuntaijiaju.cn

[C01] 定义函数
来源：http://bk.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://ws.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nv.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://bp.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://be.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dg.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wi.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://ko.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qi.chemitech.net.cn

[C02] 默认参数
来源：http://ht.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://xt.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cn.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://pi.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zx.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ts.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nn.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://bs.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://bi.muxihuayi.cn

[C03] 可变参数
来源：http://ob.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://cx.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://my.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bl.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yj.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bk.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ia.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ze.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gj.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://sg.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cq.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://km.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ea.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rm.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://fg.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://hg.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://zt.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://jb.hahajie.cn

[C05] 返回多个值
来源：http://sz.nszjky.cn

Py:   return a, b
来源：http://ea.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://dq.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vu.hnjuh.cn

TS:   return { a, b };
来源：http://on.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://da.shxzskj.cn

Go:   return a, b
来源：http://zt.szsharing.cn

Ruby: return a, b
来源：http://ew.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://ty.szxytkj.cn


<!-- 参考信息 -->