代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://qb.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://np.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://qw.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://ti.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://gd.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://lp.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bh.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://wc.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://vb.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://fo.nicolike.cn

[A16] 真假值判断规则
来源：http://hi.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://du.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zn.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lh.9csxet.cn

TS:   if (!x) {}
来源：http://ya.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ah.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gi.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wo.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sz.bookmarksfly.cn

[A17] 位运算
来源：http://zu.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sk.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ym.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qu.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ms.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qz.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zr.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://by.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://io.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://qx.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://qf.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://st.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://an.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ah.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://lq.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dv.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://ss.colortex.cn

C#:   (int)'A'; (char)65
来源：http://ms.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://wb.chemitech.net.cn

Py:   a, b = b, a
来源：http://wz.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://er.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://gw.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://nc.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://ft.haigaiapp.cn

Go:   a, b = b, a
来源：http://cc.gzmigu.cn

Ruby: a, b = b, a
来源：http://pv.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://iv.chemitech.net.cn

[A20] 读取标准输入
来源：http://ni.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://jq.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qa.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ya.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://hx.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://ih.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lb.jctech888.com.cn

Ruby: gets.chomp
来源：http://vb.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://bk.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://zu.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://pj.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gx.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://wa.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://hg.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://rk.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iq.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://nu.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://tp.yuexingan06.cn

[A22] 获取字符串长度
来源：http://ye.szxytkj.cn

Py:   len(s)
来源：http://gz.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kd.huixiangedu.cn

TS:   s.length
来源：http://gt.panjiajie.cn

Java: s.length()
来源：http://wc.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://na.huixiangedu.cn

Ruby: s.length
来源：http://on.newstarts.cn

C#:   s.Length
来源：http://zl.9csxet.cn

[A23] 大小写转换
来源：http://np.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fa.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iu.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gs.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://th.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pv.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mf.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eh.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yj.shtwfgs.cn

[A24] 去除首尾空白
来源：http://pq.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gb.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://de.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://um.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uq.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pt.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://am.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ea.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ls.huixiangedu.cn

[A25] 字符串比较
来源：http://jk.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://xs.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ku.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xm.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xh.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fi.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://im.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xs.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zf.shtwfgs.cn

[A26] 类型转换总览
来源：http://wz.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lb.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jk.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mn.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://yy.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zy.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lh.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zi.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cq.bookmarksfly.cn

================================================================================
来源：http://ra.yuexingan06.cn

B. 流程控制
来源：http://kw.newstarts.cn

================================================================================
来源：http://au.panjiajie.cn

[B01] 条件判断 if / else
来源：http://sp.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oh.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fv.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://la.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uy.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dx.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gc.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://po.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zx.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://pl.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pi.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qu.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ds.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://et.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wk.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ns.shxzukj.cn

[B03] switch / match / case
来源：http://fu.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ns.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lu.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bc.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fc.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cs.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://la.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ek.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ul.bookmarksfly.cn

[B04] for 计数循环
来源：http://zb.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://eg.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ax.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://va.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ir.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fm.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bg.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://jj.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fp.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://fk.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://bi.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xp.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oa.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ln.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lf.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ff.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://es.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://za.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://pt.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sm.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bw.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fq.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lr.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jt.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fe.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ua.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xd.asd995.cn

[B07] while 循环
来源：http://ny.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://be.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hs.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://yw.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://mq.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://gh.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dn.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://am.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://xx.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://qh.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://qn.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cu.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://nv.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://ar.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://dn.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jy.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kj.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://jt.yuntaijiaju.cn

[B09] break 与 continue
来源：http://vi.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wj.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rb.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xm.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gh.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ub.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zq.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.colortex.cn

[B10] 遍历同时拿索引
来源：http://nc.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fw.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fn.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zk.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wn.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gv.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zc.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pk.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://db.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://ia.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ja.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://mq.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ii.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://da.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bw.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pp.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://es.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ru.haigaiapp.cn

[B12] 跳出多层循环
来源：http://ge.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vr.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zg.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://li.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lv.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pm.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qf.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wr.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pa.9csxet.cn

[B13] 判断是否为数字
来源：http://gm.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://zn.asd995.cn

PHP:  is_numeric($x)
来源：http://nv.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tq.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nz.shxzskj.cn

Java: x instanceof Number
来源：http://fl.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ei.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://al.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://za.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://io.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://au.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ni.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://xk.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://pc.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tj.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qd.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oj.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mv.huanxung.cn

[B15] 布尔运算与取反
来源：http://dj.lnxyls.cn

Py:   a and b or not c
来源：http://sb.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ir.shtwfgs.cn

JS:   a && b || !c
来源：http://ur.gzmigu.cn

TS:   a && b || !c
来源：http://mq.hnjuh.cn

Java: a && b || !c
来源：http://xg.hahajie.cn

Go:   a && b || !c
来源：http://hr.shxzukj.cn

Ruby: a && b || !c
来源：http://pp.wgjwhj.cn

C#:   a && b || !c
来源：http://jb.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bu.jianghongdianzi.cn

Py:   if not data: return
来源：http://gs.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://gr.szxytkj.cn

JS:   if (!data) return;
来源：http://rj.9csxet.cn

TS:   if (!data) return;
来源：http://yt.9csxet.cn

Java: if (data == null) return;
来源：http://nx.panjiajie.cn

Go:   if data == nil { return }
来源：http://nx.muxihuayi.cn

Ruby: return if data.nil?
来源：http://lq.nszjky.cn

C#:   if (data == null) return;
来源：http://mz.jianghongdianzi.cn

================================================================================
来源：http://zf.huanxung.cn

C. 函数与作用域
来源：http://bw.9csxet.cn

================================================================================
来源：http://xh.yuexingan06.cn

[C01] 定义函数
来源：http://eu.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://la.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ww.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://uq.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ir.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xi.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nr.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://yz.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qu.huixinmuqiang.cn

[C02] 默认参数
来源：http://nw.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://uf.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dt.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://sx.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ck.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ly.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fk.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://rd.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://cr.shtwfgs.cn

[C03] 可变参数
来源：http://fx.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://le.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wa.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xf.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kn.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xe.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dx.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tz.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ub.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://av.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ai.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://or.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lr.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xc.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://xc.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://ci.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://tf.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://ro.gzmigu.cn

[C05] 返回多个值
来源：http://uz.yuntaijiaju.cn

Py:   return a, b
来源：http://ct.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://kp.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://du.shxzukj.cn

TS:   return { a, b };
来源：http://pz.gzmigu.cn


<!-- 参考信息 -->