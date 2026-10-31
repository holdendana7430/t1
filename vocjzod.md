代发 wailian999

Ruby: value = data || "默认值"
来源：http://yd.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://iq.colortex.cn

[A16] 真假值判断规则
来源：http://lh.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xk.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qf.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oo.gzmigu.cn

TS:   if (!x) {}
来源：http://dy.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aw.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nq.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wk.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fc.szsharing.cn

[A17] 位运算
来源：http://qz.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vo.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lz.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tu.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://at.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ve.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rt.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qi.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qe.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://is.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://fl.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://so.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oq.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gs.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://rc.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zj.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://ld.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://zr.521024.cn

[A19] 交换两个变量
来源：http://ff.bookmarksfly.cn

Py:   a, b = b, a
来源：http://qb.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rp.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://lb.521024.cn

TS:   [a, b] = [b, a];
来源：http://oc.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://wh.asd995.cn

Go:   a, b = b, a
来源：http://pp.9csxet.cn

Ruby: a, b = b, a
来源：http://la.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://nr.colortex.cn

[A20] 读取标准输入
来源：http://ns.shxzukj.cn

Py:   name = input("请输入：")
来源：http://jh.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yr.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zb.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://on.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://ra.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://db.asd995.cn

Ruby: gets.chomp
来源：http://oh.szsharing.cn

C#:   Console.ReadLine();
来源：http://fq.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://wj.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://qj.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pt.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://zj.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://dc.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://hj.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://td.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://sw.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://uj.521024.cn

[A22] 获取字符串长度
来源：http://sv.lnxyls.cn

Py:   len(s)
来源：http://dt.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xb.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sz.haigaiapp.cn

TS:   s.length
来源：http://mw.521024.cn

Java: s.length()
来源：http://ld.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mw.huixinmuqiang.cn

Ruby: s.length
来源：http://we.szsharing.cn

C#:   s.Length
来源：http://or.jctech888.com.cn

[A23] 大小写转换
来源：http://xq.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yl.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fq.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lj.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oi.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kh.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ly.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tj.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jn.panjiajie.cn

[A24] 去除首尾空白
来源：http://pt.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rc.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://io.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jj.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lc.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sr.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://qe.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zk.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ug.gzmigu.cn

[A25] 字符串比较
来源：http://pa.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://yp.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zl.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yd.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zd.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://us.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vt.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vc.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ro.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://ag.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://us.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gm.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lq.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://zj.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vy.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iq.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jb.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://og.muxihuayi.cn

================================================================================
来源：http://bw.yuexingan06.cn

B. 流程控制
来源：http://ay.lnxyls.cn

================================================================================
来源：http://ij.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://hi.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lc.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yj.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cp.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ov.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gm.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oo.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tf.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nn.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://zb.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nb.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qa.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://or.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ud.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ah.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ss.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qm.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sc.hahajie.cn

[B03] switch / match / case
来源：http://yf.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ap.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uw.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vn.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rc.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cv.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pz.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hq.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nu.huanxung.cn

[B04] for 计数循环
来源：http://gb.asd995.cn

Py:   for i in range(10): print(i)
来源：http://hl.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://id.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bh.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sw.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hw.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ok.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://bk.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oy.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://er.521024.cn

Py:   for item in arr: print(item)
来源：http://ux.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lu.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ha.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kt.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jv.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rm.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://kb.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pi.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://zu.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xs.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ao.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eq.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rb.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ea.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jj.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wd.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ib.szxytkj.cn

[B07] while 循环
来源：http://sr.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://xv.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sz.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://dr.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://il.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://cj.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gj.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://al.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://vb.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://ge.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://bs.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://te.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://vb.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://vc.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://hg.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://te.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xu.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://mz.lnxyls.cn

[B09] break 与 continue
来源：http://lh.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mr.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gh.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xs.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ui.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ou.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rg.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hx.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://pf.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ky.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mm.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jb.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rx.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ku.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yv.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nn.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fi.521024.cn

[B11] 生成数字序列 / 区间
来源：http://dn.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://hr.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://ne.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://km.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://os.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ds.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ov.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://ak.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gc.jctech888.com.cn

[B12] 跳出多层循环
来源：http://tt.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hh.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hv.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jv.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nk.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rh.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pj.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pv.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kk.huanxung.cn

[B13] 判断是否为数字
来源：http://md.521024.cn

Py:   isinstance(x, (int, float))
来源：http://dl.lnxyls.cn

PHP:  is_numeric($x)
来源：http://we.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aa.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qm.9csxet.cn

Java: x instanceof Number
来源：http://rj.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ou.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://un.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://ox.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://ph.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jw.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xl.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://mg.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://me.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mb.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nz.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yn.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bf.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://km.521024.cn

Py:   a and b or not c
来源：http://oc.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://fz.huixiangedu.cn

JS:   a && b || !c
来源：http://rr.nszjky.cn

TS:   a && b || !c
来源：http://nl.gzmigu.cn

Java: a && b || !c
来源：http://ev.shxzskj.cn

Go:   a && b || !c
来源：http://mg.lnxyls.cn

Ruby: a && b || !c
来源：http://yt.yuntaijiaju.cn

C#:   a && b || !c
来源：http://uv.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jf.huanxung.cn

Py:   if not data: return
来源：http://mg.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://ne.panjiajie.cn

JS:   if (!data) return;
来源：http://rs.nszjky.cn

TS:   if (!data) return;
来源：http://jp.wgjwhj.cn

Java: if (data == null) return;
来源：http://ld.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://lg.9csxet.cn

Ruby: return if data.nil?
来源：http://mw.szxytkj.cn

C#:   if (data == null) return;
来源：http://fq.panjiajie.cn

================================================================================
来源：http://gr.shxzskj.cn

C. 函数与作用域
来源：http://us.yuntaijiaju.cn

================================================================================
来源：http://hq.521024.cn

[C01] 定义函数
来源：http://mi.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://mf.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jm.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://xo.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ce.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ht.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://da.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://ml.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vz.nicolike.cn

[C02] 默认参数
来源：http://mj.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://lf.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hf.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://dm.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xl.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kw.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xs.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://rk.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://gl.szxytkj.cn

[C03] 可变参数
来源：http://xl.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://mg.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oo.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gq.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://is.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mt.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ul.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ur.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dq.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://wn.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hc.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vs.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zb.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://by.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://ak.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://mk.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://yh.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://kl.bookmarksfly.cn

[C05] 返回多个值
来源：http://wk.panjiajie.cn

Py:   return a, b
来源：http://as.huanxung.cn

PHP:  return [$a, $b];
来源：http://om.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kj.jctech888.com.cn

TS:   return { a, b };
来源：http://pf.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cy.yuexingan06.cn

Go:   return a, b
来源：http://yy.szsharing.cn

Ruby: return a, b
来源：http://wk.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://ek.521024.cn

[C06] 匿名函数 / lambda
来源：http://vm.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://at.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qp.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://ch.huanxung.cn


<!-- 参考信息 -->