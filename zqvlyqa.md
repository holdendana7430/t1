代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://nw.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://jl.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://md.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://rp.colortex.cn

Ruby: value = data || "默认值"
来源：http://vs.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://tl.bjjhwx.cn

[A16] 真假值判断规则
来源：http://fb.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dz.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bn.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bs.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://gz.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iv.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tj.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nn.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mw.yuexingan06.cn

[A17] 位运算
来源：http://jr.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mp.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dj.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hm.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sg.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lo.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rz.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://by.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fl.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://kk.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://jz.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://to.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qf.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wz.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://bx.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cg.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://ny.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://ro.nicolike.cn

[A19] 交换两个变量
来源：http://cm.huixiangedu.cn

Py:   a, b = b, a
来源：http://lz.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xg.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://ju.colortex.cn

TS:   [a, b] = [b, a];
来源：http://mu.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://qd.hnjuh.cn

Go:   a, b = b, a
来源：http://qr.521024.cn

Ruby: a, b = b, a
来源：http://kv.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://gs.haigaiapp.cn

[A20] 读取标准输入
来源：http://il.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://za.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://un.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zf.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://ct.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://oz.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sr.bookmarksfly.cn

Ruby: gets.chomp
来源：http://ao.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://ic.521024.cn

[A21] 保留指定小数位输出
来源：http://ju.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://uw.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://al.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://xb.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://pe.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://lp.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gd.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://rw.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://ch.nicolike.cn

[A22] 获取字符串长度
来源：http://io.shxzskj.cn

Py:   len(s)
来源：http://im.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dg.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wc.szxytkj.cn

TS:   s.length
来源：http://lm.chemitech.net.cn

Java: s.length()
来源：http://bk.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ru.newstarts.cn

Ruby: s.length
来源：http://ml.haigaiapp.cn

C#:   s.Length
来源：http://op.huixinmuqiang.cn

[A23] 大小写转换
来源：http://sx.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tu.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bi.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jm.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uu.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://em.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jg.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jy.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lt.bjjhwx.cn

[A24] 去除首尾空白
来源：http://ff.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yt.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ab.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qd.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qk.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ca.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://yn.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yt.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fm.hnjuh.cn

[A25] 字符串比较
来源：http://aa.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://yg.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vu.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hq.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://al.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ek.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wd.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ft.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://up.521024.cn

[A26] 类型转换总览
来源：http://kd.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hk.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fj.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tn.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://cd.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ky.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tr.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zo.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tj.panjiajie.cn

================================================================================
来源：http://qn.colortex.cn

B. 流程控制
来源：http://el.muxihuayi.cn

================================================================================
来源：http://vb.shxzukj.cn

[B01] 条件判断 if / else
来源：http://kq.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://us.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://af.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fq.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wk.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bu.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tf.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bt.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gs.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://fv.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://db.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ms.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xd.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yd.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vn.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://az.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jh.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bd.jctech888.com.cn

[B03] switch / match / case
来源：http://bu.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dy.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bt.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wj.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hx.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bm.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sh.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hf.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://be.huixinmuqiang.cn

[B04] for 计数循环
来源：http://dl.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://ut.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mh.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cx.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ap.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pq.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ri.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://zn.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ch.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://rh.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://rk.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://is.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ck.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ej.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://by.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sh.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://qq.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gq.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://qt.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cm.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yg.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yc.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pd.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fu.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ln.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lx.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://an.szxytkj.cn

[B07] while 循环
来源：http://pk.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://gp.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zm.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://rb.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://nj.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://hp.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ht.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://ns.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://ka.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://wm.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://su.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cu.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://og.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://pr.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://fm.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dm.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kd.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://kf.szsharing.cn

[B09] break 与 continue
来源：http://sf.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://en.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mi.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ei.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vm.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bs.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zm.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bh.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pz.521024.cn

[B10] 遍历同时拿索引
来源：http://ex.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xo.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vj.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bb.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oe.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jb.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nt.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hv.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lp.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://fo.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://jj.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://zi.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qy.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rz.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zb.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jv.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://iz.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mk.szsharing.cn

[B12] 跳出多层循环
来源：http://cl.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zx.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bo.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bv.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ta.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cp.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ki.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ns.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pf.521024.cn

[B13] 判断是否为数字
来源：http://rz.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://ji.huanxung.cn

PHP:  is_numeric($x)
来源：http://sb.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ce.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fs.shxzskj.cn

Java: x instanceof Number
来源：http://nv.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://be.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://fq.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://dh.huanxung.cn

[B14] 判断值是否在集合内
来源：http://vx.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gq.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://au.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://oq.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://uu.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nv.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vr.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zv.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gy.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://ep.huanxung.cn

Py:   a and b or not c
来源：http://ls.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://kk.yuexingan06.cn

JS:   a && b || !c
来源：http://qv.panjiajie.cn

TS:   a && b || !c
来源：http://pm.bjjhwx.cn

Java: a && b || !c
来源：http://pg.huanxung.cn

Go:   a && b || !c
来源：http://dj.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://up.haigaiapp.cn

C#:   a && b || !c
来源：http://wn.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qf.chemitech.net.cn

Py:   if not data: return
来源：http://nk.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://et.huixiangedu.cn

JS:   if (!data) return;
来源：http://yg.yuexingan06.cn

TS:   if (!data) return;
来源：http://dc.huanxung.cn

Java: if (data == null) return;
来源：http://xd.bjjhwx.cn

Go:   if data == nil { return }
来源：http://iw.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://yp.nicolike.cn

C#:   if (data == null) return;
来源：http://hc.bjjhwx.cn

================================================================================
来源：http://gs.huixinmuqiang.cn

C. 函数与作用域
来源：http://zz.huixiangedu.cn

================================================================================
来源：http://ba.huixiangedu.cn

[C01] 定义函数
来源：http://zp.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://zm.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jz.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://dw.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://el.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://da.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ew.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://dq.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zy.hahajie.cn

[C02] 默认参数
来源：http://tc.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://ws.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uo.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://ak.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pf.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://du.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ys.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://lx.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://um.szxytkj.cn

[C03] 可变参数
来源：http://we.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://jg.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sv.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wx.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uh.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bd.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vs.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ay.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hk.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://tf.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ir.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sl.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mh.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kw.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://xc.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://qh.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://it.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://hv.wgjwhj.cn

[C05] 返回多个值
来源：http://qu.nicolike.cn

Py:   return a, b
来源：http://in.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://yk.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yu.jianghongdianzi.cn

TS:   return { a, b };
来源：http://js.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://di.lnxyls.cn

Go:   return a, b
来源：http://yv.shtwfgs.cn

Ruby: return a, b
来源：http://gy.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://ip.muxihuayi.cn


<!-- 参考信息 -->