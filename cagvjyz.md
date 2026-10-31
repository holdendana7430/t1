代发 wailian999

Ruby: value = data || "默认值"
来源：http://qc.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://jh.shtwfgs.cn

[A16] 真假值判断规则
来源：http://no.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vl.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qd.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mx.haigaiapp.cn

TS:   if (!x) {}
来源：http://xa.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ox.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bd.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mq.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://as.yuexingan06.cn

[A17] 位运算
来源：http://vm.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lj.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sr.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fv.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dp.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zg.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ng.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bh.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fk.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://vu.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://tu.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://kp.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bd.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jg.521024.cn

Java: (int) 'A'; (char) 65
来源：http://oz.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://it.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://yn.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://ly.huanxung.cn

[A19] 交换两个变量
来源：http://dy.newstarts.cn

Py:   a, b = b, a
来源：http://wb.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ko.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://ul.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://mq.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://uw.shxzukj.cn

Go:   a, b = b, a
来源：http://kb.nicolike.cn

Ruby: a, b = b, a
来源：http://ak.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://ae.bjjhwx.cn

[A20] 读取标准输入
来源：http://mf.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://ff.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oi.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ah.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://oi.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://rk.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ae.hnjuh.cn

Ruby: gets.chomp
来源：http://ia.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://qf.9csxet.cn

[A21] 保留指定小数位输出
来源：http://tk.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://ij.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kx.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://yq.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://do.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://ls.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://py.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://uk.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://gy.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://wl.asd995.cn

Py:   len(s)
来源：http://bi.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gx.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://it.521024.cn

TS:   s.length
来源：http://cf.nicolike.cn

Java: s.length()
来源：http://aq.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qs.szxytkj.cn

Ruby: s.length
来源：http://np.gzmigu.cn

C#:   s.Length
来源：http://dj.muxihuayi.cn

[A23] 大小写转换
来源：http://lf.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xp.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bw.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yh.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eg.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xm.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zj.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://da.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://aj.shxzukj.cn

[A24] 去除首尾空白
来源：http://ub.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vs.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://of.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ia.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mf.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ps.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://at.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dy.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qn.haigaiapp.cn

[A25] 字符串比较
来源：http://ky.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://gx.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://js.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pi.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yr.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kd.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xd.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://db.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ng.521024.cn

[A26] 类型转换总览
来源：http://fx.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hu.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sf.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nj.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://bi.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mw.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xn.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vr.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bf.wgjwhj.cn

================================================================================
来源：http://xs.colortex.cn

B. 流程控制
来源：http://np.shxzskj.cn

================================================================================
来源：http://hh.nicolike.cn

[B01] 条件判断 if / else
来源：http://ce.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ag.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gu.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://it.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wh.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jh.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ce.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jv.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uq.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://pc.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qg.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vm.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://el.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wp.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://de.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xm.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vr.bookmarksfly.cn

[B03] switch / match / case
来源：http://bb.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uv.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lq.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yd.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kq.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uy.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ez.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ao.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ck.521024.cn

[B04] for 计数循环
来源：http://gt.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://yn.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fk.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ge.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sm.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sw.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ht.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://ok.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yi.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://jf.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://rd.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kt.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iz.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ly.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://op.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qg.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://kb.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dm.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://zq.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ci.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mt.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lq.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qu.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pc.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qw.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wl.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ki.newstarts.cn

[B07] while 循环
来源：http://df.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://hj.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lp.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://jj.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://eq.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://vy.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jj.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://vu.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://yr.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://rn.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://rs.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://za.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://wz.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://rj.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://yo.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fs.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kd.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://kw.haigaiapp.cn

[B09] break 与 continue
来源：http://he.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fo.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xo.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://er.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ua.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hk.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hn.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xp.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zz.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://pn.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pw.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://av.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mh.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hi.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://os.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ip.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gj.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zf.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://te.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://md.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://pi.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ge.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bk.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yj.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gl.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://vt.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nq.521024.cn

[B12] 跳出多层循环
来源：http://pf.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hy.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ua.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ix.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ml.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kq.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hq.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rp.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kw.wgjwhj.cn

[B13] 判断是否为数字
来源：http://cv.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://um.asd995.cn

PHP:  is_numeric($x)
来源：http://cv.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rf.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zy.szsharing.cn

Java: x instanceof Number
来源：http://ha.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ln.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://qz.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://sk.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://xc.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sp.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://br.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ut.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://pc.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dd.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ff.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qv.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yx.nicolike.cn

[B15] 布尔运算与取反
来源：http://eg.haigaiapp.cn

Py:   a and b or not c
来源：http://ol.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://np.bjjhwx.cn

JS:   a && b || !c
来源：http://bi.newstarts.cn

TS:   a && b || !c
来源：http://rr.huixinmuqiang.cn

Java: a && b || !c
来源：http://xq.colortex.cn

Go:   a && b || !c
来源：http://jo.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://fp.chemitech.net.cn

C#:   a && b || !c
来源：http://al.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ki.hahajie.cn

Py:   if not data: return
来源：http://mh.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://ka.9csxet.cn

JS:   if (!data) return;
来源：http://qr.haigaiapp.cn

TS:   if (!data) return;
来源：http://kl.nicolike.cn

Java: if (data == null) return;
来源：http://rn.jctech888.com.cn

Go:   if data == nil { return }
来源：http://sm.muxihuayi.cn

Ruby: return if data.nil?
来源：http://mh.haigaiapp.cn

C#:   if (data == null) return;
来源：http://md.lnxyls.cn

================================================================================
来源：http://nl.chemitech.net.cn

C. 函数与作用域
来源：http://yb.hahajie.cn

================================================================================
来源：http://ot.shtwfgs.cn

[C01] 定义函数
来源：http://vr.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://mf.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jv.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://ad.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qm.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fj.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jk.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://qo.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aj.chemitech.net.cn

[C02] 默认参数
来源：http://bd.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://sw.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ub.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://bs.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ok.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vc.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lq.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://gy.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://gt.hahajie.cn

[C03] 可变参数
来源：http://es.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://xf.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ab.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lm.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mh.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://de.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://te.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mw.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hf.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://ux.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iu.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bg.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ua.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://np.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://us.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://gd.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ei.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://zp.wgjwhj.cn

[C05] 返回多个值
来源：http://cm.szsharing.cn

Py:   return a, b
来源：http://fg.panjiajie.cn

PHP:  return [$a, $b];
来源：http://ap.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wx.9csxet.cn

TS:   return { a, b };
来源：http://du.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ky.bookmarksfly.cn

Go:   return a, b
来源：http://mw.newstarts.cn

Ruby: return a, b
来源：http://lf.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ck.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://xr.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://pd.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vf.9csxet.cn

JS:   const square = x => x * x;
来源：http://vs.bjjhwx.cn


<!-- 参考信息 -->