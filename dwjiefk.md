代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://fq.huanxung.cn

[A15] 空值判断与默认值
来源：http://ez.panjiajie.cn

Py:   value = data or "默认值"
来源：http://ir.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://es.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://vb.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://xe.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ls.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://vb.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://hc.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://lw.huixiangedu.cn

[A16] 真假值判断规则
来源：http://to.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ir.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jh.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oc.gzmigu.cn

TS:   if (!x) {}
来源：http://tx.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xa.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kl.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xi.bjjhwx.cn

[A17] 位运算
来源：http://dg.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oh.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xb.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fr.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://al.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ru.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fe.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fp.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pf.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://st.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://on.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://ma.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bp.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sy.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://ek.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dh.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://fz.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://gy.huixiangedu.cn

[A19] 交换两个变量
来源：http://gi.9csxet.cn

Py:   a, b = b, a
来源：http://yi.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pi.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://rn.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://sv.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://xv.shtwfgs.cn

Go:   a, b = b, a
来源：http://td.shxzukj.cn

Ruby: a, b = b, a
来源：http://ek.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://kx.9csxet.cn

[A20] 读取标准输入
来源：http://wx.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://qy.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vl.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://po.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://hi.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://vg.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ov.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://so.lnxyls.cn

C#:   Console.ReadLine();
来源：http://td.hahajie.cn

[A21] 保留指定小数位输出
来源：http://xw.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://ue.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oo.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://zk.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://xt.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://wi.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ax.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://pa.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://nf.huanxung.cn

[A22] 获取字符串长度
来源：http://qq.muxihuayi.cn

Py:   len(s)
来源：http://kk.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ga.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kt.huixiangedu.cn

TS:   s.length
来源：http://xm.chemitech.net.cn

Java: s.length()
来源：http://gx.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://er.gzmigu.cn

Ruby: s.length
来源：http://nr.nszjky.cn

C#:   s.Length
来源：http://sy.huanxung.cn

[A23] 大小写转换
来源：http://hb.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://th.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xu.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lf.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wv.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ar.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ch.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zh.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bm.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://bv.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ic.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nw.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lz.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rl.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vt.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://ui.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://th.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mj.szsharing.cn

[A25] 字符串比较
来源：http://an.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://wr.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lw.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jq.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mg.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sz.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nv.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pa.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hs.asd995.cn

[A26] 类型转换总览
来源：http://fg.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://id.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zk.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ae.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://it.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mp.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://af.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vp.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://af.chemitech.net.cn

================================================================================
来源：http://rd.yuntaijiaju.cn

B. 流程控制
来源：http://js.shxzukj.cn

================================================================================
来源：http://cf.colortex.cn

[B01] 条件判断 if / else
来源：http://ju.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://he.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qe.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gt.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kt.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ts.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ud.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fp.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zf.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://ic.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ez.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vh.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vn.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fq.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ok.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sf.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gu.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://do.yuexingan06.cn

[B03] switch / match / case
来源：http://xo.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uk.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ph.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ng.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wp.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bn.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://us.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bz.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://js.nszjky.cn

[B04] for 计数循环
来源：http://gj.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://ul.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fo.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uu.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hb.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xm.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vs.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://hf.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uv.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://gl.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://qk.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kb.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ao.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rr.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wl.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ve.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://or.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ch.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://ht.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vx.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jh.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tb.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ng.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ih.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cg.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ou.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ou.szsharing.cn

[B07] while 循环
来源：http://xt.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://yn.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kg.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://st.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://ky.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://en.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xo.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://mn.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://md.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://bq.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://yw.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yj.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://li.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://yh.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://wl.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zd.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xq.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://bx.bjjhwx.cn

[B09] break 与 continue
来源：http://uv.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pq.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://la.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://px.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oj.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dx.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mg.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pj.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gz.9csxet.cn

[B10] 遍历同时拿索引
来源：http://kb.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://np.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yf.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xj.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nt.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://on.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sz.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mr.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sl.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://pf.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://xe.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://zv.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xc.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yy.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ul.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qk.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://et.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kr.chemitech.net.cn

[B12] 跳出多层循环
来源：http://rg.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qr.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ax.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nv.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xg.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ll.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mr.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eq.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ja.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://wm.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://mf.huanxung.cn

PHP:  is_numeric($x)
来源：http://uu.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nb.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lj.szxytkj.cn

Java: x instanceof Number
来源：http://pz.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://io.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://jf.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://nz.hahajie.cn

[B14] 判断值是否在集合内
来源：http://bb.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://li.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://od.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://nw.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://yb.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qp.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pf.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dh.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ti.hnjuh.cn

[B15] 布尔运算与取反
来源：http://hr.bookmarksfly.cn

Py:   a and b or not c
来源：http://fy.szsharing.cn

PHP:  $a && $b || !$c
来源：http://rs.bjjhwx.cn

JS:   a && b || !c
来源：http://hb.chemitech.net.cn

TS:   a && b || !c
来源：http://by.wgjwhj.cn

Java: a && b || !c
来源：http://if.nicolike.cn

Go:   a && b || !c
来源：http://vi.521024.cn

Ruby: a && b || !c
来源：http://gg.chemitech.net.cn

C#:   a && b || !c
来源：http://su.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ie.huixinmuqiang.cn

Py:   if not data: return
来源：http://qz.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://qs.bjjhwx.cn

JS:   if (!data) return;
来源：http://kc.haigaiapp.cn

TS:   if (!data) return;
来源：http://yu.panjiajie.cn

Java: if (data == null) return;
来源：http://iu.haigaiapp.cn

Go:   if data == nil { return }
来源：http://jc.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://ua.shxzukj.cn

C#:   if (data == null) return;
来源：http://kl.szxytkj.cn

================================================================================
来源：http://fs.szsharing.cn

C. 函数与作用域
来源：http://zv.newstarts.cn

================================================================================
来源：http://lc.yuexingan06.cn

[C01] 定义函数
来源：http://xp.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://jo.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pi.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://wo.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iq.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ha.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cd.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://da.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ai.hahajie.cn

[C02] 默认参数
来源：http://zb.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://ch.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zt.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://sh.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gh.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://id.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xi.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://xc.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://ny.wgjwhj.cn

[C03] 可变参数
来源：http://eh.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://kh.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lp.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zv.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://up.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fs.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yr.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pc.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ku.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://ez.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gj.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xz.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xo.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mw.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://fe.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://bu.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://vm.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://xp.chemitech.net.cn

[C05] 返回多个值
来源：http://gv.colortex.cn

Py:   return a, b
来源：http://hb.shxzukj.cn

PHP:  return [$a, $b];
来源：http://di.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ad.jianghongdianzi.cn

TS:   return { a, b };
来源：http://yc.huanxung.cn


<!-- 参考信息 -->