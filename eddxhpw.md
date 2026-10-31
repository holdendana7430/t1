代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://ba.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ay.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://mj.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://si.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://ly.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://xb.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://mw.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://dq.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://yr.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://cq.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xs.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://jx.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://cu.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://lm.lnxyls.cn

[A16] 真假值判断规则
来源：http://uq.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kw.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ut.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eh.wgjwhj.cn

TS:   if (!x) {}
来源：http://mw.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gk.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pb.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wk.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fq.bjjhwx.cn

[A17] 位运算
来源：http://ah.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://or.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://az.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nc.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bz.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://de.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://di.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dw.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iv.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://ec.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://vm.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://zz.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rt.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wf.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://tj.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yd.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://qr.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://do.szxytkj.cn

[A19] 交换两个变量
来源：http://lk.yuexingan06.cn

Py:   a, b = b, a
来源：http://kg.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ct.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://cj.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://qc.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://ag.nicolike.cn

Go:   a, b = b, a
来源：http://hh.chemitech.net.cn

Ruby: a, b = b, a
来源：http://wl.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://so.muxihuayi.cn

[A20] 读取标准输入
来源：http://zb.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://oo.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://of.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rn.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://yd.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://yk.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fo.gzmigu.cn

Ruby: gets.chomp
来源：http://ev.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://jr.nicolike.cn

[A21] 保留指定小数位输出
来源：http://bl.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://tn.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://go.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://bs.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://ff.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://pg.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ez.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://me.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://lo.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://fx.gzmigu.cn

Py:   len(s)
来源：http://of.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gk.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iq.bookmarksfly.cn

TS:   s.length
来源：http://uu.hahajie.cn

Java: s.length()
来源：http://pv.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wm.szxytkj.cn

Ruby: s.length
来源：http://xb.yuntaijiaju.cn

C#:   s.Length
来源：http://tg.huanxung.cn

[A23] 大小写转换
来源：http://fv.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zq.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ep.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ay.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bt.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ot.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ao.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://el.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ds.lnxyls.cn

[A24] 去除首尾空白
来源：http://wo.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bl.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fl.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qx.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ab.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sa.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://bc.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ij.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ob.jctech888.com.cn

[A25] 字符串比较
来源：http://ox.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://cr.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ps.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gk.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ul.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pu.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yk.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cu.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qx.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://wk.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ws.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fz.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://la.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://ug.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fj.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fu.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lx.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qe.haigaiapp.cn

================================================================================
来源：http://jm.nicolike.cn

B. 流程控制
来源：http://lb.yuntaijiaju.cn

================================================================================
来源：http://ik.szxytkj.cn

[B01] 条件判断 if / else
来源：http://yt.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://se.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ck.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ia.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hy.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bh.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vc.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tw.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lt.nszjky.cn

[B02] 多分支 else if / elif
来源：http://ha.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lm.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kl.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eg.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qe.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ef.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hh.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rd.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hw.szxytkj.cn

[B03] switch / match / case
来源：http://qr.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hj.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fo.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://di.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aa.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://du.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rl.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://of.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oj.panjiajie.cn

[B04] for 计数循环
来源：http://hn.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://qp.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zf.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vt.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://of.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://la.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ub.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://ar.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gr.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://va.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ug.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nd.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tb.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rk.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ga.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cg.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://ii.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rr.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://fo.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pb.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tg.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tn.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dd.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qy.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ud.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ea.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://py.asd995.cn

[B07] while 循环
来源：http://tz.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://tg.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ee.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://wi.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://gf.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://ug.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rm.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://kt.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://ph.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://xs.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://eb.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ys.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://jb.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://pd.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://fz.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ji.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xk.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://ht.hnjuh.cn

[B09] break 与 continue
来源：http://os.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kt.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kq.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kt.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zl.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hi.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ko.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ok.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sm.nszjky.cn

[B10] 遍历同时拿索引
来源：http://wf.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yo.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dn.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vz.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://et.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qg.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rg.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sb.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://or.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://yd.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://va.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://bx.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sa.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ci.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oo.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lx.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://lg.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cm.bjjhwx.cn

[B12] 跳出多层循环
来源：http://vp.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uc.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rt.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lg.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lo.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wn.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tl.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dx.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://be.wgjwhj.cn

[B13] 判断是否为数字
来源：http://tj.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://uw.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://di.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ve.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.asd995.cn

Java: x instanceof Number
来源：http://me.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dn.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://sp.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://sg.colortex.cn

[B14] 判断值是否在集合内
来源：http://yp.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xd.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kw.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://at.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://cz.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ix.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ls.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zo.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ah.asd995.cn

[B15] 布尔运算与取反
来源：http://oy.521024.cn

Py:   a and b or not c
来源：http://go.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://bw.lnxyls.cn

JS:   a && b || !c
来源：http://xy.hnjuh.cn

TS:   a && b || !c
来源：http://hz.shxzskj.cn

Java: a && b || !c
来源：http://xw.gzmigu.cn

Go:   a && b || !c
来源：http://ws.nszjky.cn

Ruby: a && b || !c
来源：http://pk.szsharing.cn

C#:   a && b || !c
来源：http://bm.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xa.gzmigu.cn

Py:   if not data: return
来源：http://xy.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://mb.hnjuh.cn

JS:   if (!data) return;
来源：http://qs.shxzskj.cn

TS:   if (!data) return;
来源：http://sy.newstarts.cn

Java: if (data == null) return;
来源：http://la.hahajie.cn

Go:   if data == nil { return }
来源：http://ij.521024.cn

Ruby: return if data.nil?
来源：http://am.gzmigu.cn

C#:   if (data == null) return;
来源：http://gn.521024.cn

================================================================================
来源：http://yn.bjjhwx.cn

C. 函数与作用域
来源：http://zc.huixiangedu.cn

================================================================================
来源：http://bc.521024.cn

[C01] 定义函数
来源：http://km.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://ds.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ig.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://ke.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sb.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xc.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://re.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://ay.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mk.gzmigu.cn

[C02] 默认参数
来源：http://ja.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://kq.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kq.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://mx.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cl.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xz.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gk.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://rj.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://if.521024.cn

[C03] 可变参数
来源：http://zz.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://jy.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pw.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vx.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gd.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nq.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dr.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ef.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bl.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ds.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vs.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ba.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oi.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rg.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://fg.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://qz.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://qd.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://gr.hahajie.cn

[C05] 返回多个值
来源：http://ff.szxytkj.cn


<!-- 参考信息 -->