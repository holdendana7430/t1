代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://ew.gzmigu.cn

[A15] 空值判断与默认值
来源：http://dn.asd995.cn

Py:   value = data or "默认值"
来源：http://rn.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://ll.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://pw.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://vm.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cj.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://fd.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://zi.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://gr.colortex.cn

[A16] 真假值判断规则
来源：http://wx.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cb.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qs.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://km.wgjwhj.cn

TS:   if (!x) {}
来源：http://rt.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://he.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ga.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kd.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://al.jctech888.com.cn

[A17] 位运算
来源：http://he.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://or.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yq.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gz.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://da.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ur.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ki.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xw.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://tc.asd995.cn

Py:   ord("A"); chr(65)
来源：http://sf.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://ck.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://me.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://my.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://pd.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pe.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://jg.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://qm.hahajie.cn

[A19] 交换两个变量
来源：http://px.huixiangedu.cn

Py:   a, b = b, a
来源：http://nl.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ue.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://eq.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://iw.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://gr.chemitech.net.cn

Go:   a, b = b, a
来源：http://ne.nszjky.cn

Ruby: a, b = b, a
来源：http://is.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://lz.shxzskj.cn

[A20] 读取标准输入
来源：http://bh.nszjky.cn

Py:   name = input("请输入：")
来源：http://hm.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cu.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yq.521024.cn

TS:   // Node.js：readline 模块
来源：http://cr.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://vw.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bk.shxzskj.cn

Ruby: gets.chomp
来源：http://jl.colortex.cn

C#:   Console.ReadLine();
来源：http://zl.newstarts.cn

[A21] 保留指定小数位输出
来源：http://at.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://wa.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sr.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://fc.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://xb.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://ag.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gv.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://eu.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://wp.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://mb.521024.cn

Py:   len(s)
来源：http://ei.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kz.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rc.hnjuh.cn

TS:   s.length
来源：http://fp.9csxet.cn

Java: s.length()
来源：http://ud.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://js.szsharing.cn

Ruby: s.length
来源：http://sh.521024.cn

C#:   s.Length
来源：http://qw.jianghongdianzi.cn

[A23] 大小写转换
来源：http://nv.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://br.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://he.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://te.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fz.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://td.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lv.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tc.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sy.huanxung.cn

[A24] 去除首尾空白
来源：http://td.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dk.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://so.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sx.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ys.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pg.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://gp.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hw.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oh.shxzskj.cn

[A25] 字符串比较
来源：http://fn.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://ev.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bt.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xr.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kz.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oy.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pb.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sr.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wd.huanxung.cn

[A26] 类型转换总览
来源：http://yr.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pa.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kg.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vq.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://lm.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ur.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pk.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pp.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mi.bookmarksfly.cn

================================================================================
来源：http://kk.bookmarksfly.cn

B. 流程控制
来源：http://wc.shxzukj.cn

================================================================================
来源：http://yu.asd995.cn

[B01] 条件判断 if / else
来源：http://lu.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://by.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ku.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kv.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://at.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qt.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ze.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wi.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fs.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://kc.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eg.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yg.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wk.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tf.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xi.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aj.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dv.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wj.gzmigu.cn

[B03] switch / match / case
来源：http://gx.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://km.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tt.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zu.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tj.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uy.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ei.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gf.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qd.nszjky.cn

[B04] for 计数循环
来源：http://fy.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://hh.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pp.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ic.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cj.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nf.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vj.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://nz.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://su.521024.cn

[B05] 遍历数组 / 列表
来源：http://ff.nicolike.cn

Py:   for item in arr: print(item)
来源：http://mt.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cq.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pw.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wv.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sj.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pb.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://nc.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oi.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://ne.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ie.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gy.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ax.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://be.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nq.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qr.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vt.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://va.nicolike.cn

[B07] while 循环
来源：http://dq.newstarts.cn

Py:   while i < 10: i += 1
来源：http://jn.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ba.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://he.521024.cn

TS:   while (i < 10) { i++; }
来源：http://qo.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://uj.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://um.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://io.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://cc.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://bb.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://ks.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sy.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://do.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://ei.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://ox.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hl.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xy.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://cs.gzmigu.cn

[B09] break 与 continue
来源：http://yi.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eh.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wz.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vo.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://je.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sc.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://we.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fe.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://xi.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ff.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vs.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://am.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rl.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ej.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iv.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mf.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dx.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://fn.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://wp.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://on.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gb.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gw.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oc.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qm.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://ij.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lm.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://bs.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mm.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eu.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ux.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tx.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hq.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rv.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mc.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vn.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://ca.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://bi.nszjky.cn

PHP:  is_numeric($x)
来源：http://om.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dc.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lm.shtwfgs.cn

Java: x instanceof Number
来源：http://kk.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zo.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://or.newstarts.cn

C#:   x is int or double or decimal
来源：http://ql.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://cp.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vv.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vi.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://qb.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://lm.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qi.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dm.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rd.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yp.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://od.jctech888.com.cn

Py:   a and b or not c
来源：http://yf.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://vv.huanxung.cn

JS:   a && b || !c
来源：http://ik.yuexingan06.cn

TS:   a && b || !c
来源：http://pq.lnxyls.cn

Java: a && b || !c
来源：http://su.jctech888.com.cn

Go:   a && b || !c
来源：http://ag.haigaiapp.cn

Ruby: a && b || !c
来源：http://oy.szsharing.cn

C#:   a && b || !c
来源：http://zt.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://og.wgjwhj.cn

Py:   if not data: return
来源：http://vi.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://rw.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://ii.huanxung.cn

TS:   if (!data) return;
来源：http://vr.nicolike.cn

Java: if (data == null) return;
来源：http://kw.nszjky.cn

Go:   if data == nil { return }
来源：http://rx.huanxung.cn

Ruby: return if data.nil?
来源：http://ya.gzmigu.cn

C#:   if (data == null) return;
来源：http://xw.asd995.cn

================================================================================
来源：http://zn.nszjky.cn

C. 函数与作用域
来源：http://ma.shxzukj.cn

================================================================================
来源：http://ab.bjjhwx.cn

[C01] 定义函数
来源：http://oy.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://va.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ij.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://dp.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qt.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ti.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tj.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://zx.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ax.shxzskj.cn

[C02] 默认参数
来源：http://ng.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://pm.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ra.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://si.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ll.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ut.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pr.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://ye.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://zi.jianghongdianzi.cn

[C03] 可变参数
来源：http://tj.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://ge.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ea.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yr.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zm.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tz.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://es.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ln.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ub.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://gw.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pu.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tp.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wx.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://me.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://gu.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://ty.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://mm.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://bp.jctech888.com.cn

[C05] 返回多个值
来源：http://sw.muxihuayi.cn

Py:   return a, b
来源：http://pz.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://fm.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kq.nicolike.cn

TS:   return { a, b };
来源：http://en.shtwfgs.cn


<!-- 参考信息 -->