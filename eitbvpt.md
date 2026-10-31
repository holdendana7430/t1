代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://xg.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://rs.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://tc.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://gx.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://fz.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://el.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kr.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://zw.newstarts.cn

Ruby: value = data || "默认值"
来源：http://xh.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://zx.yuexingan06.cn

[A16] 真假值判断规则
来源：http://jj.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bw.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eu.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qq.lnxyls.cn

TS:   if (!x) {}
来源：http://ud.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pl.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wa.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yb.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://it.hahajie.cn

[A17] 位运算
来源：http://re.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vl.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ql.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ki.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://av.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rc.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oj.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ce.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ar.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://ve.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://ye.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://mu.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bc.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vr.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://xh.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://up.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://uw.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://xk.huixiangedu.cn

[A19] 交换两个变量
来源：http://wv.muxihuayi.cn

Py:   a, b = b, a
来源：http://qr.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cf.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://on.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://db.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://co.panjiajie.cn

Go:   a, b = b, a
来源：http://rr.521024.cn

Ruby: a, b = b, a
来源：http://dh.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://cv.521024.cn

[A20] 读取标准输入
来源：http://fc.asd995.cn

Py:   name = input("请输入：")
来源：http://is.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ju.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ir.521024.cn

TS:   // Node.js：readline 模块
来源：http://bd.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://ow.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://du.9csxet.cn

Ruby: gets.chomp
来源：http://pg.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://io.nicolike.cn

[A21] 保留指定小数位输出
来源：http://ll.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://vw.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hu.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://nv.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://et.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://eq.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dv.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://dg.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://pj.huixiangedu.cn

[A22] 获取字符串长度
来源：http://vf.yuntaijiaju.cn

Py:   len(s)
来源：http://ob.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cv.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://us.bookmarksfly.cn

TS:   s.length
来源：http://em.9csxet.cn

Java: s.length()
来源：http://wl.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ak.haigaiapp.cn

Ruby: s.length
来源：http://fu.huixinmuqiang.cn

C#:   s.Length
来源：http://ac.hahajie.cn

[A23] 大小写转换
来源：http://ic.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ia.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yi.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xf.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://si.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ea.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yq.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ck.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kb.521024.cn

[A24] 去除首尾空白
来源：http://sg.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rp.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mh.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bt.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jt.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kv.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://yc.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zb.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zg.wgjwhj.cn

[A25] 字符串比较
来源：http://nl.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://jf.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gz.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://in.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bl.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lm.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://di.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mj.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dk.colortex.cn

[A26] 类型转换总览
来源：http://xg.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mq.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fg.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://me.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://ik.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lk.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bt.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ht.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://de.gzmigu.cn

================================================================================
来源：http://gp.wgjwhj.cn

B. 流程控制
来源：http://fu.asd995.cn

================================================================================
来源：http://av.colortex.cn

[B01] 条件判断 if / else
来源：http://pu.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gd.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vn.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yx.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nt.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://do.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pe.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pl.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qm.521024.cn

[B02] 多分支 else if / elif
来源：http://ay.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xs.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ds.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ru.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zf.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ly.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ze.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pp.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ba.jianghongdianzi.cn

[B03] switch / match / case
来源：http://zl.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sf.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ij.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jc.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wy.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uy.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fi.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cl.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yo.bookmarksfly.cn

[B04] for 计数循环
来源：http://jj.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://bh.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bq.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fx.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://br.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zr.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jx.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://jp.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qe.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://qn.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://zv.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bw.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vo.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qe.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vi.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jh.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://eg.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fi.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://kn.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sy.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bu.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cs.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aq.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lp.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rj.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wp.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mu.shxzskj.cn

[B07] while 循环
来源：http://sv.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://hu.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gv.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://na.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://hi.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://hd.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hx.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://bg.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://gp.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://iy.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://vk.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://if.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://up.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://dt.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://es.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rg.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zo.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://kx.shxzskj.cn

[B09] break 与 continue
来源：http://yg.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://od.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ua.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dh.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gn.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dp.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zy.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ii.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://go.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://ju.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dm.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gp.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tl.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zd.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zc.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qw.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ac.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vf.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://al.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://pe.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://kw.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ir.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fq.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zm.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ip.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://jt.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://es.huixiangedu.cn

[B12] 跳出多层循环
来源：http://iq.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lq.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vk.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kt.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iv.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aj.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ax.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mo.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fa.nicolike.cn

[B13] 判断是否为数字
来源：http://tv.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://mi.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://ik.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uj.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jv.9csxet.cn

Java: x instanceof Number
来源：http://oq.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qr.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://hf.colortex.cn

C#:   x is int or double or decimal
来源：http://or.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://fu.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tm.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bu.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://zv.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://tb.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uo.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cg.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vo.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cq.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://ji.gzmigu.cn

Py:   a and b or not c
来源：http://ra.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://oh.nicolike.cn

JS:   a && b || !c
来源：http://jo.9csxet.cn

TS:   a && b || !c
来源：http://cd.wgjwhj.cn

Java: a && b || !c
来源：http://zl.colortex.cn

Go:   a && b || !c
来源：http://jk.521024.cn

Ruby: a && b || !c
来源：http://cz.9csxet.cn

C#:   a && b || !c
来源：http://ec.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aa.bookmarksfly.cn

Py:   if not data: return
来源：http://gf.asd995.cn

PHP:  if (!$data) { return; }
来源：http://ub.chemitech.net.cn

JS:   if (!data) return;
来源：http://rn.wgjwhj.cn

TS:   if (!data) return;
来源：http://sl.jctech888.com.cn

Java: if (data == null) return;
来源：http://ux.panjiajie.cn

Go:   if data == nil { return }
来源：http://ne.hahajie.cn

Ruby: return if data.nil?
来源：http://ni.nszjky.cn

C#:   if (data == null) return;
来源：http://du.nszjky.cn

================================================================================
来源：http://wf.jctech888.com.cn

C. 函数与作用域
来源：http://jv.hnjuh.cn

================================================================================
来源：http://xa.jctech888.com.cn

[C01] 定义函数
来源：http://gj.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://ee.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rq.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://cr.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rb.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://av.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hi.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://wo.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nb.gzmigu.cn

[C02] 默认参数
来源：http://th.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://ej.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nk.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://cr.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dj.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hx.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dt.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://be.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://ln.colortex.cn

[C03] 可变参数
来源：http://we.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://fo.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ny.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gc.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://np.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kc.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ef.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sn.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ae.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://tj.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nk.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tu.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lc.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yr.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://lv.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://cq.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://oy.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://cy.lnxyls.cn

[C05] 返回多个值
来源：http://br.panjiajie.cn

Py:   return a, b
来源：http://jq.nicolike.cn

PHP:  return [$a, $b];
来源：http://fz.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nc.yuexingan06.cn

TS:   return { a, b };
来源：http://mx.haigaiapp.cn


<!-- 参考信息 -->