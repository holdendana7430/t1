代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://ru.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://at.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://fd.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gj.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://sa.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://mc.newstarts.cn

Py:   value = data or "默认值"
来源：http://my.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://dn.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://ml.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://xk.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ag.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://ht.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://tv.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://xp.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://co.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zd.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ak.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dv.9csxet.cn

TS:   if (!x) {}
来源：http://lx.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://av.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ac.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qg.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ln.nicolike.cn

[A17] 位运算
来源：http://ln.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ss.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fr.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eg.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dl.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ov.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ad.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nt.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sz.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://ea.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://re.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://tc.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mw.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gm.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://wg.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bi.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://fi.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://lp.hahajie.cn

[A19] 交换两个变量
来源：http://dy.shxzukj.cn

Py:   a, b = b, a
来源：http://nu.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fj.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://eq.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://kp.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://cr.szxytkj.cn

Go:   a, b = b, a
来源：http://jd.bjjhwx.cn

Ruby: a, b = b, a
来源：http://ar.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://vx.9csxet.cn

[A20] 读取标准输入
来源：http://vw.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://ea.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tv.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rq.asd995.cn

TS:   // Node.js：readline 模块
来源：http://ll.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://yb.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jw.hahajie.cn

Ruby: gets.chomp
来源：http://jq.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://hn.nszjky.cn

[A21] 保留指定小数位输出
来源：http://xz.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://ba.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xm.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://wk.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ug.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://gd.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gr.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://fj.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://sn.shxzukj.cn

[A22] 获取字符串长度
来源：http://io.wgjwhj.cn

Py:   len(s)
来源：http://la.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wm.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://by.huanxung.cn

TS:   s.length
来源：http://eq.jctech888.com.cn

Java: s.length()
来源：http://cx.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bz.yuntaijiaju.cn

Ruby: s.length
来源：http://fw.shtwfgs.cn

C#:   s.Length
来源：http://dr.asd995.cn

[A23] 大小写转换
来源：http://hd.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://em.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qg.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kr.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://db.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ch.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zv.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lp.szsharing.cn

[A24] 去除首尾空白
来源：http://hi.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kn.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hv.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tx.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://km.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pb.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://fr.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zg.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cx.newstarts.cn

[A25] 字符串比较
来源：http://gj.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://bs.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gd.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ov.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jo.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zl.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kh.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ga.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wn.colortex.cn

[A26] 类型转换总览
来源：http://ox.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qm.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dl.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xt.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://hf.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://py.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ka.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fo.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lt.hnjuh.cn

================================================================================
来源：http://il.jctech888.com.cn

B. 流程控制
来源：http://co.shxzskj.cn

================================================================================
来源：http://zm.gzmigu.cn

[B01] 条件判断 if / else
来源：http://lk.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yb.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xw.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yr.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ol.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hi.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ep.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ot.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rj.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://nb.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iw.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ft.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kv.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vd.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ft.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fh.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ay.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.huanxung.cn

[B03] switch / match / case
来源：http://zc.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gv.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rm.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tg.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xr.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qk.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oh.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cb.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ir.yuexingan06.cn

[B04] for 计数循环
来源：http://am.asd995.cn

Py:   for i in range(10): print(i)
来源：http://dd.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ow.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://by.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gm.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ol.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ae.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://io.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ew.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://fz.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://wj.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cw.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zm.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yl.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://du.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ts.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://gv.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zw.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://ia.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jm.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nb.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://od.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://co.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://su.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ai.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lq.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zc.huixinmuqiang.cn

[B07] while 循环
来源：http://te.nicolike.cn

Py:   while i < 10: i += 1
来源：http://gi.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hb.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://vn.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://do.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://on.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ns.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://er.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://vr.asd995.cn

[B08] do-while（至少执行一次）
来源：http://lj.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://er.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kr.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://iv.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://ay.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://ji.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dk.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ik.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://jc.shxzukj.cn

[B09] break 与 continue
来源：http://bc.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ou.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gk.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ln.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wh.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rb.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cj.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bk.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jz.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://dn.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rb.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zl.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bb.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fm.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dj.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hx.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oh.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hy.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://tp.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ja.521024.cn

PHP:  range(0, 10, 2);
来源：http://uv.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wr.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ad.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xs.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kx.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://hx.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bq.nszjky.cn

[B12] 跳出多层循环
来源：http://ee.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ik.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rv.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://el.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qd.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hv.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xx.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ip.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ky.hahajie.cn

[B13] 判断是否为数字
来源：http://lg.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://lx.asd995.cn

PHP:  is_numeric($x)
来源：http://ga.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uy.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zx.asd995.cn

Java: x instanceof Number
来源：http://fp.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lt.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://jd.gzmigu.cn

C#:   x is int or double or decimal
来源：http://tm.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://bw.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vn.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gu.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://wz.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://qd.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nl.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vf.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nn.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pg.shxzukj.cn

[B15] 布尔运算与取反
来源：http://zc.gzmigu.cn

Py:   a and b or not c
来源：http://ds.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://qy.szxytkj.cn

JS:   a && b || !c
来源：http://zs.szsharing.cn

TS:   a && b || !c
来源：http://lw.chemitech.net.cn

Java: a && b || !c
来源：http://pf.szxytkj.cn

Go:   a && b || !c
来源：http://ti.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://xo.521024.cn

C#:   a && b || !c
来源：http://db.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ii.9csxet.cn

Py:   if not data: return
来源：http://zw.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://fu.jctech888.com.cn

JS:   if (!data) return;
来源：http://ij.jctech888.com.cn

TS:   if (!data) return;
来源：http://oo.shxzukj.cn

Java: if (data == null) return;
来源：http://me.szxytkj.cn

Go:   if data == nil { return }
来源：http://jq.shtwfgs.cn

Ruby: return if data.nil?
来源：http://gj.hahajie.cn

C#:   if (data == null) return;
来源：http://uc.521024.cn

================================================================================
来源：http://yf.chemitech.net.cn

C. 函数与作用域
来源：http://ek.newstarts.cn

================================================================================
来源：http://ma.colortex.cn

[C01] 定义函数
来源：http://js.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://bq.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aw.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://wx.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ux.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yz.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pf.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://wq.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hp.shxzukj.cn

[C02] 默认参数
来源：http://lo.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ht.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://se.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://gb.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yt.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ch.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dx.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://wf.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://jc.yuntaijiaju.cn

[C03] 可变参数
来源：http://qo.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://qh.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ew.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zu.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jw.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wx.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kl.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bj.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vl.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://wp.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tv.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pi.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oo.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iv.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://sq.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://en.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://ms.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://qo.muxihuayi.cn

[C05] 返回多个值
来源：http://ql.newstarts.cn


<!-- 参考信息 -->