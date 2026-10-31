代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://tb.521024.cn

[A15] 空值判断与默认值
来源：http://gm.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://tz.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://xp.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://ba.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://gu.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ww.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://rg.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://kg.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://xv.shxzukj.cn

[A16] 真假值判断规则
来源：http://yr.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xg.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://se.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lh.newstarts.cn

TS:   if (!x) {}
来源：http://ak.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qo.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yn.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xt.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cs.asd995.cn

[A17] 位运算
来源：http://uy.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kj.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ro.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mz.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pp.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yj.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ss.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://et.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fg.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://kw.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://cd.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://bu.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ny.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://on.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://iv.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fl.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://rt.asd995.cn

C#:   (int)'A'; (char)65
来源：http://ge.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://an.shxzukj.cn

Py:   a, b = b, a
来源：http://nf.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tk.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://hm.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://ec.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://iq.bjjhwx.cn

Go:   a, b = b, a
来源：http://eo.szsharing.cn

Ruby: a, b = b, a
来源：http://wv.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://eh.huixiangedu.cn

[A20] 读取标准输入
来源：http://gk.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://yw.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rx.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://im.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://ic.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://zo.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fg.newstarts.cn

Ruby: gets.chomp
来源：http://cv.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://ql.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://gy.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://xb.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ju.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://io.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://sx.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://mi.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lg.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://is.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://jr.lnxyls.cn

[A22] 获取字符串长度
来源：http://zc.asd995.cn

Py:   len(s)
来源：http://nd.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kp.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rq.shtwfgs.cn

TS:   s.length
来源：http://rx.yuexingan06.cn

Java: s.length()
来源：http://eo.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bm.lnxyls.cn

Ruby: s.length
来源：http://pw.yuntaijiaju.cn

C#:   s.Length
来源：http://ae.szxytkj.cn

[A23] 大小写转换
来源：http://fs.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hu.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://en.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fx.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bz.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bk.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ms.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kf.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vo.jctech888.com.cn

[A24] 去除首尾空白
来源：http://yl.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pb.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://it.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ln.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://af.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cv.521024.cn

Go:   strings.TrimSpace(s)
来源：http://cz.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://un.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ha.newstarts.cn

[A25] 字符串比较
来源：http://ny.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://nu.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ve.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jd.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cj.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ed.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ef.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ap.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sx.yuexingan06.cn

[A26] 类型转换总览
来源：http://ml.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ih.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fc.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://we.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://xc.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aw.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oq.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sy.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sa.muxihuayi.cn

================================================================================
来源：http://cf.huanxung.cn

B. 流程控制
来源：http://ys.yuntaijiaju.cn

================================================================================
来源：http://sw.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://tv.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sy.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zc.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://us.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jd.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eh.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gh.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ol.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://du.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://tf.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ci.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cx.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pl.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qc.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pw.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cd.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mr.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zz.521024.cn

[B03] switch / match / case
来源：http://fs.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pd.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qf.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lo.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fi.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dl.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xc.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fs.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kb.hahajie.cn

[B04] for 计数循环
来源：http://xz.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://gh.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mn.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tm.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yx.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qo.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zd.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://sa.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zn.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://ub.nicolike.cn

Py:   for item in arr: print(item)
来源：http://wc.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gx.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yq.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ql.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://co.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uu.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://bt.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qv.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://fp.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uu.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mo.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://td.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mt.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xk.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pj.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ch.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hh.huixinmuqiang.cn

[B07] while 循环
来源：http://iz.521024.cn

Py:   while i < 10: i += 1
来源：http://lq.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ct.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://xc.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://hu.asd995.cn

Java: while (i < 10) { i++; }
来源：http://cy.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ts.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://mz.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://vx.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://oq.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://ez.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gs.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://ml.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://um.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://ri.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ss.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ue.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://ye.hahajie.cn

[B09] break 与 continue
来源：http://ig.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kh.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ji.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ut.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cj.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hx.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vd.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gj.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ta.asd995.cn

[B10] 遍历同时拿索引
来源：http://kk.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zj.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tw.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wz.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ub.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bw.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://of.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sn.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://op.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://tj.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ms.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://fp.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nd.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zt.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tq.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lq.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://dj.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ws.hnjuh.cn

[B12] 跳出多层循环
来源：http://yd.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qc.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mb.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jn.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sh.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fl.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xu.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xi.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://it.huanxung.cn

[B13] 判断是否为数字
来源：http://ii.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ye.shxzskj.cn

PHP:  is_numeric($x)
来源：http://pd.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cn.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xw.gzmigu.cn

Java: x instanceof Number
来源：http://sq.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cb.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://pd.shxzskj.cn

C#:   x is int or double or decimal
来源：http://pa.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://hs.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://at.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wi.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://ab.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://ya.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://na.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ph.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wu.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://av.colortex.cn

[B15] 布尔运算与取反
来源：http://bf.9csxet.cn

Py:   a and b or not c
来源：http://kv.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://kt.szxytkj.cn

JS:   a && b || !c
来源：http://sa.huixinmuqiang.cn

TS:   a && b || !c
来源：http://yz.newstarts.cn

Java: a && b || !c
来源：http://bp.nszjky.cn

Go:   a && b || !c
来源：http://nj.hnjuh.cn

Ruby: a && b || !c
来源：http://fp.panjiajie.cn

C#:   a && b || !c
来源：http://dw.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fg.nszjky.cn

Py:   if not data: return
来源：http://kw.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://zw.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://yu.wgjwhj.cn

TS:   if (!data) return;
来源：http://ha.shxzukj.cn

Java: if (data == null) return;
来源：http://vx.asd995.cn

Go:   if data == nil { return }
来源：http://ne.szxytkj.cn

Ruby: return if data.nil?
来源：http://xm.521024.cn

C#:   if (data == null) return;
来源：http://oj.haigaiapp.cn

================================================================================
来源：http://jw.chemitech.net.cn

C. 函数与作用域
来源：http://nc.asd995.cn

================================================================================
来源：http://sw.yuntaijiaju.cn

[C01] 定义函数
来源：http://yc.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://na.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gi.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://nc.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zj.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xn.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mp.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://xu.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tr.hnjuh.cn

[C02] 默认参数
来源：http://vl.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://wt.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rm.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://dn.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wk.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vh.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iw.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://fb.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://bb.jctech888.com.cn

[C03] 可变参数
来源：http://ks.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://iq.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jr.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lr.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://az.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bw.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pz.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vm.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kc.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://vh.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tc.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ea.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://id.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mv.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://wa.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://go.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://ov.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://vc.asd995.cn

[C05] 返回多个值
来源：http://kz.hnjuh.cn

Py:   return a, b
来源：http://si.nicolike.cn

PHP:  return [$a, $b];
来源：http://ew.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hr.hnjuh.cn

TS:   return { a, b };
来源：http://ah.wgjwhj.cn


<!-- 参考信息 -->