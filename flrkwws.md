代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yf.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tl.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ty.hnjuh.cn

[A17] 位运算
来源：http://ou.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://le.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zi.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oy.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fv.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ce.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qz.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://md.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hu.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://xp.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://js.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://dc.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ui.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hx.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://ij.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ao.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://ux.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://hh.521024.cn

[A19] 交换两个变量
来源：http://ik.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://js.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uv.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://oo.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://ed.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://gx.yuexingan06.cn

Go:   a, b = b, a
来源：http://vo.nicolike.cn

Ruby: a, b = b, a
来源：http://yd.asd995.cn

C#:   (a, b) = (b, a);
来源：http://tb.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://yl.shxzskj.cn

Py:   name = input("请输入：")
来源：http://ll.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ao.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zh.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://ii.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://hp.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xx.newstarts.cn

Ruby: gets.chomp
来源：http://uw.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://xt.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://cq.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://qr.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nz.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://bh.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://tc.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://ld.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yz.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://hq.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://gq.huixiangedu.cn

[A22] 获取字符串长度
来源：http://ew.jctech888.com.cn

Py:   len(s)
来源：http://sa.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kn.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fk.newstarts.cn

TS:   s.length
来源：http://im.bookmarksfly.cn

Java: s.length()
来源：http://ho.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pp.nszjky.cn

Ruby: s.length
来源：http://is.nszjky.cn

C#:   s.Length
来源：http://pg.nszjky.cn

[A23] 大小写转换
来源：http://jq.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ip.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mz.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zf.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fj.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sn.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wc.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gf.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rr.521024.cn

[A24] 去除首尾空白
来源：http://gc.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sq.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kd.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qn.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dw.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cj.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://ax.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bd.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jb.lnxyls.cn

[A25] 字符串比较
来源：http://ot.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://ek.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gp.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jc.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rb.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xw.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mu.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rf.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vn.huanxung.cn

[A26] 类型转换总览
来源：http://og.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://py.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://it.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hg.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://qf.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pw.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ao.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vn.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gv.wgjwhj.cn

================================================================================
来源：http://cd.shxzukj.cn

B. 流程控制
来源：http://vt.panjiajie.cn

================================================================================
来源：http://mo.9csxet.cn

[B01] 条件判断 if / else
来源：http://ns.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wf.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gx.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ej.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://or.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oj.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://so.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sr.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://io.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://mf.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ts.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gg.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kb.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lh.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yv.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vo.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zw.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jw.jianghongdianzi.cn

[B03] switch / match / case
来源：http://ga.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qp.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://no.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oi.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bi.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hf.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tl.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sz.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xn.nszjky.cn

[B04] for 计数循环
来源：http://oh.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://ov.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tq.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yi.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lg.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pv.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kd.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://tt.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eh.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://rn.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://gn.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jt.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yh.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://co.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qq.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lw.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://cn.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hq.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://wh.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ec.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ns.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ee.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bs.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kg.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pr.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bg.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eu.wgjwhj.cn

[B07] while 循环
来源：http://qv.hahajie.cn

Py:   while i < 10: i += 1
来源：http://uc.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qu.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://ar.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://tj.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://qi.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yu.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://rq.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://iv.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://gq.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://cn.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vt.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://yh.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://gx.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://kc.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eb.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hy.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://am.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ch.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://el.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lm.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://db.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ss.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rt.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eq.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pa.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://it.newstarts.cn

[B10] 遍历同时拿索引
来源：http://qq.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://un.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fo.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sg.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ex.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wz.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hk.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ko.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rk.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://xo.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://lt.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://ai.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cc.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hy.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nn.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ju.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://py.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ng.jctech888.com.cn

[B12] 跳出多层循环
来源：http://od.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tv.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lc.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tx.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pl.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qd.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cu.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mr.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tp.huanxung.cn

[B13] 判断是否为数字
来源：http://fn.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://vq.asd995.cn

PHP:  is_numeric($x)
来源：http://hi.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vv.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bp.9csxet.cn

Java: x instanceof Number
来源：http://pz.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zp.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://hm.colortex.cn

C#:   x is int or double or decimal
来源：http://mu.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://yb.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bh.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zp.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://hd.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://dw.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jn.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hi.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sk.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://py.gzmigu.cn

[B15] 布尔运算与取反
来源：http://du.hnjuh.cn

Py:   a and b or not c
来源：http://yh.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://yf.huixiangedu.cn

JS:   a && b || !c
来源：http://ov.szsharing.cn

TS:   a && b || !c
来源：http://xc.asd995.cn

Java: a && b || !c
来源：http://md.521024.cn

Go:   a && b || !c
来源：http://db.haigaiapp.cn

Ruby: a && b || !c
来源：http://vt.szxytkj.cn

C#:   a && b || !c
来源：http://ce.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://di.yuntaijiaju.cn

Py:   if not data: return
来源：http://ji.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://xi.bookmarksfly.cn

JS:   if (!data) return;
来源：http://rj.hahajie.cn

TS:   if (!data) return;
来源：http://km.haigaiapp.cn

Java: if (data == null) return;
来源：http://eq.hahajie.cn

Go:   if data == nil { return }
来源：http://ba.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://am.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://gq.szxytkj.cn

================================================================================
来源：http://as.muxihuayi.cn

C. 函数与作用域
来源：http://oy.521024.cn

================================================================================
来源：http://ay.muxihuayi.cn

[C01] 定义函数
来源：http://re.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://nz.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hy.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://vl.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yt.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aj.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hu.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://in.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zx.colortex.cn

[C02] 默认参数
来源：http://hq.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://vv.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rf.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://sc.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tr.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://im.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ia.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://zp.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://mx.jctech888.com.cn

[C03] 可变参数
来源：http://tn.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://yy.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kd.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nh.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kb.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qw.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tg.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://th.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://em.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://hl.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fz.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gu.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cu.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iq.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://il.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://zb.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://rg.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://oe.panjiajie.cn

[C05] 返回多个值
来源：http://fb.gzmigu.cn

Py:   return a, b
来源：http://gc.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://zr.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://en.yuntaijiaju.cn

TS:   return { a, b };
来源：http://ne.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fy.shtwfgs.cn

Go:   return a, b
来源：http://ri.muxihuayi.cn

Ruby: return a, b
来源：http://ta.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://fr.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://yr.szsharing.cn

Py:   square = lambda x: x * x
来源：http://rd.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sb.newstarts.cn

JS:   const square = x => x * x;
来源：http://nq.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://lm.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ii.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fu.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://mx.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hu.colortex.cn

[C07] 把函数作为参数传入
来源：http://fu.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xy.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zn.jianghongdianzi.cn


<!-- 参考信息 -->