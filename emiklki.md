代发 wailian999

Ruby: value = data || "默认值"
来源：http://tu.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://mf.shxzukj.cn

[A16] 真假值判断规则
来源：http://fs.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xq.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iz.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aw.colortex.cn

TS:   if (!x) {}
来源：http://rh.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kw.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xy.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xl.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mr.gzmigu.cn

[A17] 位运算
来源：http://dy.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fi.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://at.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dc.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gn.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fw.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tg.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zq.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dc.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://zb.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://bq.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://ba.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xw.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://el.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://rb.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://on.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://oa.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://qg.wgjwhj.cn

[A19] 交换两个变量
来源：http://dy.jctech888.com.cn

Py:   a, b = b, a
来源：http://mk.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jd.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://as.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://tq.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://cg.huixiangedu.cn

Go:   a, b = b, a
来源：http://tf.haigaiapp.cn

Ruby: a, b = b, a
来源：http://pn.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://kz.chemitech.net.cn

[A20] 读取标准输入
来源：http://bk.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://sm.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zy.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fk.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://jz.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://tp.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lm.bookmarksfly.cn

Ruby: gets.chomp
来源：http://mq.gzmigu.cn

C#:   Console.ReadLine();
来源：http://dz.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://oh.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://dk.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mx.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://fq.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://rk.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://dz.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qo.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://xv.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://ur.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://vp.huanxung.cn

Py:   len(s)
来源：http://of.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sp.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pc.yuntaijiaju.cn

TS:   s.length
来源：http://nz.yuntaijiaju.cn

Java: s.length()
来源：http://gs.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xk.shtwfgs.cn

Ruby: s.length
来源：http://oo.szxytkj.cn

C#:   s.Length
来源：http://lp.nicolike.cn

[A23] 大小写转换
来源：http://ja.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gz.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zw.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oa.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xl.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sl.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oy.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dy.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://up.lnxyls.cn

[A24] 去除首尾空白
来源：http://ch.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xy.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rs.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ah.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ug.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://so.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://ue.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cg.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mu.huixiangedu.cn

[A25] 字符串比较
来源：http://kt.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://tp.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zk.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cx.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qx.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wt.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yw.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tv.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rn.hahajie.cn

[A26] 类型转换总览
来源：http://bk.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ok.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fm.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lk.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://of.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://te.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ez.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oa.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rf.huixiangedu.cn

================================================================================
来源：http://jm.haigaiapp.cn

B. 流程控制
来源：http://xm.szxytkj.cn

================================================================================
来源：http://uf.panjiajie.cn

[B01] 条件判断 if / else
来源：http://xs.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ry.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xt.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mn.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yw.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vi.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tr.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qo.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yd.huanxung.cn

[B02] 多分支 else if / elif
来源：http://zf.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xa.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yq.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vo.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fz.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qo.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://we.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nw.shtwfgs.cn

[B03] switch / match / case
来源：http://bx.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ai.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yj.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ts.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kj.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kx.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rj.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uh.haigaiapp.cn

[B04] for 计数循环
来源：http://vr.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://xu.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kf.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kl.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pf.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cb.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://va.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://nz.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://db.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://et.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://rb.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://we.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ak.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sh.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ht.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jc.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://ht.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fe.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://zi.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xt.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wo.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ab.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xc.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iw.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://he.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://we.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://av.hnjuh.cn

[B07] while 循环
来源：http://si.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://kq.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eh.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://he.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://iq.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://bu.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vh.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://ru.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://zp.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://zw.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://ha.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wn.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://la.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://ho.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://yo.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xh.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vc.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://zp.hnjuh.cn

[B09] break 与 continue
来源：http://nl.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hj.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://st.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pl.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fc.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://og.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vf.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uv.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://is.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://qt.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://te.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://su.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ak.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ww.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qf.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kw.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qj.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jm.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://kh.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://gp.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://ub.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lf.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ga.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rx.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ks.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://gz.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ak.nicolike.cn

[B12] 跳出多层循环
来源：http://td.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gf.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ai.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sz.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wz.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ht.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ok.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://on.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ww.521024.cn

[B13] 判断是否为数字
来源：http://ni.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://qo.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://fe.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://he.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mu.nszjky.cn

Java: x instanceof Number
来源：http://ig.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ad.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://sc.lnxyls.cn

C#:   x is int or double or decimal
来源：http://gc.newstarts.cn

[B14] 判断值是否在集合内
来源：http://eo.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wk.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oh.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://lq.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://ie.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eq.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cj.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qd.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lg.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://gm.chemitech.net.cn

Py:   a and b or not c
来源：http://iu.nicolike.cn

PHP:  $a && $b || !$c
来源：http://ot.haigaiapp.cn

JS:   a && b || !c
来源：http://qu.huixiangedu.cn

TS:   a && b || !c
来源：http://yz.bookmarksfly.cn

Java: a && b || !c
来源：http://kt.nicolike.cn

Go:   a && b || !c
来源：http://aq.shtwfgs.cn

Ruby: a && b || !c
来源：http://cz.yuexingan06.cn

C#:   a && b || !c
来源：http://vy.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qd.newstarts.cn

Py:   if not data: return
来源：http://fc.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://ev.wgjwhj.cn

JS:   if (!data) return;
来源：http://yx.chemitech.net.cn

TS:   if (!data) return;
来源：http://dd.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://tz.shxzukj.cn

Go:   if data == nil { return }
来源：http://lw.yuexingan06.cn

Ruby: return if data.nil?
来源：http://ko.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://gi.huixinmuqiang.cn

================================================================================
来源：http://dt.gzmigu.cn

C. 函数与作用域
来源：http://eo.haigaiapp.cn

================================================================================
来源：http://vn.colortex.cn

[C01] 定义函数
来源：http://lk.asd995.cn

Py:   def add(a, b): return a + b
来源：http://tz.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oh.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://pi.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oi.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://io.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://su.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://yj.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sl.szsharing.cn

[C02] 默认参数
来源：http://xj.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://ey.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iv.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://zx.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://or.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pr.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eh.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://wj.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://uo.jianghongdianzi.cn

[C03] 可变参数
来源：http://oq.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://no.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://za.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pf.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ec.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nd.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ff.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yl.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pp.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://kn.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fu.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qf.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xj.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vg.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://yy.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://wf.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://qy.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://mn.shtwfgs.cn

[C05] 返回多个值
来源：http://si.colortex.cn

Py:   return a, b
来源：http://qj.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://ch.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wr.521024.cn

TS:   return { a, b };
来源：http://qd.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sp.huixinmuqiang.cn

Go:   return a, b
来源：http://ps.bjjhwx.cn

Ruby: return a, b
来源：http://mc.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://ym.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://ph.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://gk.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vq.szxytkj.cn

JS:   const square = x => x * x;
来源：http://qt.gzmigu.cn


<!-- 参考信息 -->