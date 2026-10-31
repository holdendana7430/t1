代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://qv.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://np.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://mk.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qd.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://vd.nszjky.cn

[A15] 空值判断与默认值
来源：http://gd.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://yb.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://gj.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://sz.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://zl.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qn.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://ph.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://tt.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://ej.colortex.cn

[A16] 真假值判断规则
来源：http://zb.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rn.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fh.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uz.hahajie.cn

TS:   if (!x) {}
来源：http://lu.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mh.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sa.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wj.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://md.yuntaijiaju.cn

[A17] 位运算
来源：http://lc.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rg.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://up.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fj.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uy.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hb.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xh.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ro.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://py.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://uj.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://hb.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://uj.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ns.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qa.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://kg.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ij.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://bz.colortex.cn

C#:   (int)'A'; (char)65
来源：http://rd.huanxung.cn

[A19] 交换两个变量
来源：http://hq.haigaiapp.cn

Py:   a, b = b, a
来源：http://zr.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bd.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://et.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://ac.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://xs.huanxung.cn

Go:   a, b = b, a
来源：http://to.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://zn.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://rv.lnxyls.cn

[A20] 读取标准输入
来源：http://ss.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://st.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lw.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nl.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://uw.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://te.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wd.szxytkj.cn

Ruby: gets.chomp
来源：http://me.gzmigu.cn

C#:   Console.ReadLine();
来源：http://gc.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://ig.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://gg.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tu.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://qc.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://pu.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://lo.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://az.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ku.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://ae.newstarts.cn

[A22] 获取字符串长度
来源：http://vg.newstarts.cn

Py:   len(s)
来源：http://hv.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wf.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pg.yuexingan06.cn

TS:   s.length
来源：http://iq.szxytkj.cn

Java: s.length()
来源：http://is.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nd.wgjwhj.cn

Ruby: s.length
来源：http://gj.newstarts.cn

C#:   s.Length
来源：http://lb.shxzukj.cn

[A23] 大小写转换
来源：http://rm.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gg.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mw.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qp.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vf.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xc.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ga.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jq.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dd.chemitech.net.cn

[A24] 去除首尾空白
来源：http://rf.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xn.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://in.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fb.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tn.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ra.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://lf.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bk.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mk.asd995.cn

[A25] 字符串比较
来源：http://xt.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://mj.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ow.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lw.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tr.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://il.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vo.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hu.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://he.yuexingan06.cn

[A26] 类型转换总览
来源：http://rj.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bt.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://no.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gs.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://dk.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jx.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ce.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vm.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kh.lnxyls.cn

================================================================================
来源：http://jx.lnxyls.cn

B. 流程控制
来源：http://tc.panjiajie.cn

================================================================================
来源：http://si.nszjky.cn

[B01] 条件判断 if / else
来源：http://bo.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wr.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wu.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tp.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fy.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yk.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pz.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fe.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tc.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://xw.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ra.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rl.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ty.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gj.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tv.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hx.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://is.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qx.shtwfgs.cn

[B03] switch / match / case
来源：http://uf.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tj.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://od.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mc.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rt.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zk.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pl.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sn.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fu.asd995.cn

[B04] for 计数循环
来源：http://mc.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://zs.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ce.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dx.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hg.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tm.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dc.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://pl.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://di.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://pc.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://uc.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xl.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://th.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pu.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vt.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://ts.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xh.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://st.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://js.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ai.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sm.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yf.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vm.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hu.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iv.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wo.jianghongdianzi.cn

[B07] while 循环
来源：http://md.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://fm.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ys.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://xi.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://vt.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://we.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gd.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://ex.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://jn.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://vn.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://gw.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lv.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://da.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://ro.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://dt.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sf.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://by.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://dy.wgjwhj.cn

[B09] break 与 continue
来源：http://wd.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sw.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xr.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://in.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ui.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xa.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oa.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zk.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aq.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://ht.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yo.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zf.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qq.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cc.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dx.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sq.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ns.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gp.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://wr.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://ws.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://iw.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pv.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nu.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hi.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xv.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://to.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://df.muxihuayi.cn

[B12] 跳出多层循环
来源：http://na.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cp.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wv.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://po.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dw.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nl.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tq.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ya.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ts.nicolike.cn

[B13] 判断是否为数字
来源：http://fe.521024.cn

Py:   isinstance(x, (int, float))
来源：http://bw.shxzukj.cn

PHP:  is_numeric($x)
来源：http://vb.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xr.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qp.9csxet.cn

Java: x instanceof Number
来源：http://lz.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fz.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://ge.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://bz.asd995.cn

[B14] 判断值是否在集合内
来源：http://ku.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iy.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zu.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://mu.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://mu.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://va.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uu.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gl.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qj.shxzskj.cn

[B15] 布尔运算与取反
来源：http://hn.hahajie.cn

Py:   a and b or not c
来源：http://lq.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://vw.bookmarksfly.cn

JS:   a && b || !c
来源：http://mx.jctech888.com.cn

TS:   a && b || !c
来源：http://wy.bookmarksfly.cn

Java: a && b || !c
来源：http://yk.yuexingan06.cn

Go:   a && b || !c
来源：http://tm.panjiajie.cn

Ruby: a && b || !c
来源：http://jk.bookmarksfly.cn

C#:   a && b || !c
来源：http://ji.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gq.newstarts.cn

Py:   if not data: return
来源：http://xq.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://zm.asd995.cn

JS:   if (!data) return;
来源：http://wb.haigaiapp.cn

TS:   if (!data) return;
来源：http://py.bookmarksfly.cn

Java: if (data == null) return;
来源：http://yf.wgjwhj.cn

Go:   if data == nil { return }
来源：http://kz.bjjhwx.cn

Ruby: return if data.nil?
来源：http://mn.lnxyls.cn

C#:   if (data == null) return;
来源：http://yt.huanxung.cn

================================================================================
来源：http://al.newstarts.cn

C. 函数与作用域
来源：http://xr.yuntaijiaju.cn

================================================================================
来源：http://hn.9csxet.cn

[C01] 定义函数
来源：http://yo.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://qg.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ib.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://jf.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tq.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lr.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ar.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://an.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://au.gzmigu.cn

[C02] 默认参数
来源：http://rw.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://hf.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iz.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://xr.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ss.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xg.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gq.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://nr.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://fp.gzmigu.cn

[C03] 可变参数
来源：http://hq.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://gm.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bp.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hg.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ny.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jj.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iz.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dn.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cc.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://qn.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wj.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gd.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xr.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mm.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://dp.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://wh.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://wy.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://mw.panjiajie.cn

[C05] 返回多个值
来源：http://yw.nszjky.cn


<!-- 参考信息 -->