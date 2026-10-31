代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yc.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://op.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ys.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tl.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gr.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nu.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lm.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pm.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://it.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://au.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://fe.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cl.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kq.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://mu.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gj.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://bp.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://ra.bjjhwx.cn

[A19] 交换两个变量
来源：http://gm.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://dw.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hq.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://hl.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://jy.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://ri.hnjuh.cn

Go:   a, b = b, a
来源：http://kt.shtwfgs.cn

Ruby: a, b = b, a
来源：http://ch.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://ma.chemitech.net.cn

[A20] 读取标准输入
来源：http://wz.gzmigu.cn

Py:   name = input("请输入：")
来源：http://kk.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hn.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nx.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://zy.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://xs.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zd.gzmigu.cn

Ruby: gets.chomp
来源：http://ao.nicolike.cn

C#:   Console.ReadLine();
来源：http://yx.colortex.cn

[A21] 保留指定小数位输出
来源：http://zf.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://fb.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kn.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://yx.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://zr.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://du.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ob.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://cc.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://pl.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://mj.gzmigu.cn

Py:   len(s)
来源：http://pv.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uk.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tb.wgjwhj.cn

TS:   s.length
来源：http://bo.asd995.cn

Java: s.length()
来源：http://vn.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mh.gzmigu.cn

Ruby: s.length
来源：http://rn.jctech888.com.cn

C#:   s.Length
来源：http://im.bookmarksfly.cn

[A23] 大小写转换
来源：http://nx.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rk.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dj.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://so.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://td.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ba.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nf.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cj.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cb.nszjky.cn

[A24] 去除首尾空白
来源：http://as.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://do.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tk.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dn.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jk.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://em.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://wa.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://go.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qe.muxihuayi.cn

[A25] 字符串比较
来源：http://ms.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://vj.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tr.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://co.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jm.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gz.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pk.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hm.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://us.shxzukj.cn

[A26] 类型转换总览
来源：http://aq.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zp.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qg.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cg.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://be.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ok.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ma.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zi.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zz.asd995.cn

================================================================================
来源：http://og.gzmigu.cn

B. 流程控制
来源：http://ih.nszjky.cn

================================================================================
来源：http://fx.szsharing.cn

[B01] 条件判断 if / else
来源：http://hj.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://es.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yi.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uy.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lt.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ee.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pv.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zk.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wp.colortex.cn

[B02] 多分支 else if / elif
来源：http://ce.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ke.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ke.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kb.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://il.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tg.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jw.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gd.nicolike.cn

[B03] switch / match / case
来源：http://jy.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mq.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cq.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iq.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vt.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oo.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dx.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bb.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nj.shxzukj.cn

[B04] for 计数循环
来源：http://sj.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://ny.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ex.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://md.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qr.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zp.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fe.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://zc.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wb.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://za.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://wn.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pa.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cs.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rc.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sp.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jc.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://wz.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kr.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://dg.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yb.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aw.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ur.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qc.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qk.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sf.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iw.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mp.yuexingan06.cn

[B07] while 循环
来源：http://gd.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://bk.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bp.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://tb.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://td.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://jc.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rq.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://jb.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://ny.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://bc.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://xd.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://py.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://bx.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://dd.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://rv.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ey.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qw.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://va.haigaiapp.cn

[B09] break 与 continue
来源：http://kj.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://td.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ot.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://um.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pb.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://um.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jf.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://np.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lo.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://wy.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rc.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iy.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fr.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zw.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uh.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://og.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dm.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wi.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://sx.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://he.asd995.cn

PHP:  range(0, 10, 2);
来源：http://ty.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ff.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ie.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://al.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ob.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://zh.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xy.shxzskj.cn

[B12] 跳出多层循环
来源：http://cm.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sk.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nd.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kh.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qt.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mh.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ym.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dt.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pw.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://pr.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://zg.gzmigu.cn

PHP:  is_numeric($x)
来源：http://xl.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yf.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ih.jianghongdianzi.cn

Java: x instanceof Number
来源：http://vf.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gz.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://vp.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://nh.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://fr.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ry.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ut.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://de.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://zs.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sj.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ke.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sd.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ox.nicolike.cn

[B15] 布尔运算与取反
来源：http://ao.szsharing.cn

Py:   a and b or not c
来源：http://vj.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://lt.huixiangedu.cn

JS:   a && b || !c
来源：http://in.bookmarksfly.cn

TS:   a && b || !c
来源：http://lg.shtwfgs.cn

Java: a && b || !c
来源：http://uf.szxytkj.cn

Go:   a && b || !c
来源：http://ow.huixiangedu.cn

Ruby: a && b || !c
来源：http://ma.jianghongdianzi.cn

C#:   a && b || !c
来源：http://kc.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://is.jianghongdianzi.cn

Py:   if not data: return
来源：http://lw.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://wj.asd995.cn

JS:   if (!data) return;
来源：http://ny.shxzskj.cn

TS:   if (!data) return;
来源：http://pv.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://bu.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://cm.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://bc.szxytkj.cn

C#:   if (data == null) return;
来源：http://ek.haigaiapp.cn

================================================================================
来源：http://yj.szxytkj.cn

C. 函数与作用域
来源：http://yj.521024.cn

================================================================================
来源：http://mc.colortex.cn

[C01] 定义函数
来源：http://qg.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://mw.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://na.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://sm.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ok.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tl.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://js.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://wn.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://om.szsharing.cn

[C02] 默认参数
来源：http://xo.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://dg.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yt.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://nl.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fa.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mq.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tv.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://gg.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://py.9csxet.cn

[C03] 可变参数
来源：http://sr.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://vo.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vw.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sa.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dl.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dg.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://al.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cm.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pt.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://su.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nd.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hn.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zx.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jh.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://ue.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://qv.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ha.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://bv.shtwfgs.cn

[C05] 返回多个值
来源：http://qy.colortex.cn

Py:   return a, b
来源：http://sz.panjiajie.cn

PHP:  return [$a, $b];
来源：http://oc.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rj.521024.cn

TS:   return { a, b };
来源：http://mc.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iz.wgjwhj.cn

Go:   return a, b
来源：http://rb.szsharing.cn

Ruby: return a, b
来源：http://ik.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://go.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://yt.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://hd.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uq.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://bz.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://un.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rj.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pn.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://tv.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ch.521024.cn

[C07] 把函数作为参数传入
来源：http://ul.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://in.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zo.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xu.521024.cn

TS:   arr.map(String)
来源：http://tx.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qo.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wb.haigaiapp.cn


<!-- 参考信息 -->