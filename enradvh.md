代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://op.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bf.521024.cn

TS:   if (!x) {}
来源：http://do.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ue.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wt.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://si.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://id.nicolike.cn

[A17] 位运算
来源：http://et.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bj.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jm.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wr.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ym.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://af.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nx.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hj.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nv.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://az.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://lx.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://wm.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://us.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uh.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://ly.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wb.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://bq.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://yy.newstarts.cn

[A19] 交换两个变量
来源：http://ag.wgjwhj.cn

Py:   a, b = b, a
来源：http://nr.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hh.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://mt.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://kf.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://od.jctech888.com.cn

Go:   a, b = b, a
来源：http://wb.szsharing.cn

Ruby: a, b = b, a
来源：http://mu.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://xr.chemitech.net.cn

[A20] 读取标准输入
来源：http://kr.newstarts.cn

Py:   name = input("请输入：")
来源：http://iq.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kb.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mt.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://bv.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://qm.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bx.huanxung.cn

Ruby: gets.chomp
来源：http://cx.lnxyls.cn

C#:   Console.ReadLine();
来源：http://gt.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://ek.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://bv.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oi.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://as.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://an.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://qw.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://aq.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://tr.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://do.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://io.nicolike.cn

Py:   len(s)
来源：http://wn.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gg.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cn.hnjuh.cn

TS:   s.length
来源：http://uw.asd995.cn

Java: s.length()
来源：http://oz.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cr.hnjuh.cn

Ruby: s.length
来源：http://tt.szsharing.cn

C#:   s.Length
来源：http://eg.shtwfgs.cn

[A23] 大小写转换
来源：http://mh.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://um.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://go.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mx.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cz.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ja.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xh.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uo.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yq.shxzukj.cn

[A24] 去除首尾空白
来源：http://dy.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lv.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dk.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bx.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vb.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fa.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://ab.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pe.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fl.newstarts.cn

[A25] 字符串比较
来源：http://dg.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://rx.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aj.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://je.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://il.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zf.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ym.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ez.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gz.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://wv.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gi.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://is.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ez.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://hb.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mq.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zd.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oa.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kh.shtwfgs.cn

================================================================================
来源：http://sd.yuexingan06.cn

B. 流程控制
来源：http://ht.bookmarksfly.cn

================================================================================
来源：http://pl.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://oa.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rz.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jn.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://db.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sj.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aw.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bv.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bc.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ga.521024.cn

[B02] 多分支 else if / elif
来源：http://qe.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kt.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aj.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://is.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ep.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ev.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yo.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mb.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.nicolike.cn

[B03] switch / match / case
来源：http://yl.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ao.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ug.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ws.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ro.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vd.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://my.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://io.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://re.wgjwhj.cn

[B04] for 计数循环
来源：http://hr.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://bg.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jy.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oi.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tm.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mn.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pf.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://ra.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mm.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://zs.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://dq.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dd.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kr.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gs.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ix.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tn.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://cp.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aw.colortex.cn

[B06] 遍历字典 / 对象
来源：http://lb.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rt.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hv.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dg.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bo.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zv.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://or.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://me.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ih.haigaiapp.cn

[B07] while 循环
来源：http://pf.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://og.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wo.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://xt.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://el.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://lj.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dz.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://eh.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://or.colortex.cn

[B08] do-while（至少执行一次）
来源：http://cw.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://bk.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bl.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://mk.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://dr.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://fd.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jz.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zs.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://ea.haigaiapp.cn

[B09] break 与 continue
来源：http://tg.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bx.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xv.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fa.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hn.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://du.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ne.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xd.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sy.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://kw.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ml.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qy.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zh.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ag.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xz.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cl.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cm.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fk.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://fi.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://jf.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://iu.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wh.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wi.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bt.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yx.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://gg.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yb.521024.cn

[B12] 跳出多层循环
来源：http://ck.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xn.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vv.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://id.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zh.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xp.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xw.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dw.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cm.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://zi.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://in.nszjky.cn

PHP:  is_numeric($x)
来源：http://et.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jr.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dr.jianghongdianzi.cn

Java: x instanceof Number
来源：http://zw.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oq.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://si.gzmigu.cn

C#:   x is int or double or decimal
来源：http://tg.hahajie.cn

[B14] 判断值是否在集合内
来源：http://dr.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ao.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ak.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://zu.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://yu.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ra.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bn.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yz.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lq.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://se.bjjhwx.cn

Py:   a and b or not c
来源：http://bv.521024.cn

PHP:  $a && $b || !$c
来源：http://ic.yuntaijiaju.cn

JS:   a && b || !c
来源：http://zs.lnxyls.cn

TS:   a && b || !c
来源：http://tf.yuexingan06.cn

Java: a && b || !c
来源：http://na.lnxyls.cn

Go:   a && b || !c
来源：http://of.9csxet.cn

Ruby: a && b || !c
来源：http://jl.jctech888.com.cn

C#:   a && b || !c
来源：http://iz.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pg.jianghongdianzi.cn

Py:   if not data: return
来源：http://jj.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://to.shxzskj.cn

JS:   if (!data) return;
来源：http://sm.9csxet.cn

TS:   if (!data) return;
来源：http://xk.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://xc.huanxung.cn

Go:   if data == nil { return }
来源：http://zs.shtwfgs.cn

Ruby: return if data.nil?
来源：http://ib.asd995.cn

C#:   if (data == null) return;
来源：http://pl.newstarts.cn

================================================================================
来源：http://ub.shtwfgs.cn

C. 函数与作用域
来源：http://om.bookmarksfly.cn

================================================================================
来源：http://tp.newstarts.cn

[C01] 定义函数
来源：http://on.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://na.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pv.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://pa.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zi.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zn.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sw.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://fc.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lo.shxzskj.cn

[C02] 默认参数
来源：http://zz.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://rq.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ly.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://ze.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kw.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wj.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mw.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://rv.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://in.hahajie.cn

[C03] 可变参数
来源：http://gk.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://bp.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ql.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gp.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yh.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fl.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iq.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xl.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ep.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://fd.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eh.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mz.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xl.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kw.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://bp.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://be.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://xf.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://hj.yuexingan06.cn

[C05] 返回多个值
来源：http://sv.shxzukj.cn

Py:   return a, b
来源：http://yl.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://re.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ar.9csxet.cn

TS:   return { a, b };
来源：http://kf.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aj.hnjuh.cn

Go:   return a, b
来源：http://rq.nszjky.cn

Ruby: return a, b
来源：http://my.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://pp.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://nw.hahajie.cn

Py:   square = lambda x: x * x
来源：http://op.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ii.newstarts.cn

JS:   const square = x => x * x;
来源：http://ds.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://ei.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lo.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ew.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://sa.nszjky.cn


<!-- 参考信息 -->