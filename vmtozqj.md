代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://iv.newstarts.cn

[A15] 空值判断与默认值
来源：http://on.hnjuh.cn

Py:   value = data or "默认值"
来源：http://yy.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://wk.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://mf.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://pr.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sh.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://sp.huanxung.cn

Ruby: value = data || "默认值"
来源：http://nb.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://kx.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://zv.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bs.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zt.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mh.szxytkj.cn

TS:   if (!x) {}
来源：http://te.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vh.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qd.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://im.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sw.chemitech.net.cn

[A17] 位运算
来源：http://li.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nj.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://al.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yl.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://az.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cc.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xs.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ly.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://th.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://hw.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://lc.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://qv.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xy.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rs.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://sy.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pz.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://ku.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://xo.huixiangedu.cn

[A19] 交换两个变量
来源：http://rq.szsharing.cn

Py:   a, b = b, a
来源：http://lu.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ot.asd995.cn

JS:   [a, b] = [b, a];
来源：http://jl.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://eq.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://yw.shxzskj.cn

Go:   a, b = b, a
来源：http://fa.shxzukj.cn

Ruby: a, b = b, a
来源：http://fi.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://pe.gzmigu.cn

[A20] 读取标准输入
来源：http://ng.newstarts.cn

Py:   name = input("请输入：")
来源：http://aj.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fw.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ai.521024.cn

TS:   // Node.js：readline 模块
来源：http://ix.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://mk.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fk.yuexingan06.cn

Ruby: gets.chomp
来源：http://ne.gzmigu.cn

C#:   Console.ReadLine();
来源：http://lt.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://kh.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://pw.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mf.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://ut.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://yx.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://ok.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qk.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://qw.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://oc.gzmigu.cn

[A22] 获取字符串长度
来源：http://mp.asd995.cn

Py:   len(s)
来源：http://vr.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ot.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ax.colortex.cn

TS:   s.length
来源：http://bv.nszjky.cn

Java: s.length()
来源：http://fp.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://on.shxzskj.cn

Ruby: s.length
来源：http://pq.shxzukj.cn

C#:   s.Length
来源：http://zn.hnjuh.cn

[A23] 大小写转换
来源：http://zq.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xt.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kj.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vq.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bh.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pd.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://as.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ne.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dw.huanxung.cn

[A24] 去除首尾空白
来源：http://ar.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bw.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nj.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://el.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tx.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fe.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://he.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fh.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://di.colortex.cn

[A25] 字符串比较
来源：http://de.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://zj.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sk.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ku.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mf.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cq.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lc.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qx.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fs.shxzskj.cn

[A26] 类型转换总览
来源：http://ws.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://al.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kc.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oh.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://an.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xq.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yg.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://is.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yv.nicolike.cn

================================================================================
来源：http://xm.hnjuh.cn

B. 流程控制
来源：http://jk.gzmigu.cn

================================================================================
来源：http://fa.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://xs.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cv.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pr.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nt.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rq.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ed.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sz.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lz.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jx.huanxung.cn

[B02] 多分支 else if / elif
来源：http://ms.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://it.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ok.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wu.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aq.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://si.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ba.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hh.bookmarksfly.cn

[B03] switch / match / case
来源：http://en.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://np.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jd.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ia.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ug.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nt.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iw.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xw.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jk.shxzskj.cn

[B04] for 计数循环
来源：http://hq.asd995.cn

Py:   for i in range(10): print(i)
来源：http://le.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ph.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ir.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wx.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gw.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jo.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://ci.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tw.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://zr.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://lo.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xa.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iw.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sn.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nc.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uw.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://df.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uc.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://fm.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://et.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qp.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ma.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cb.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ag.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ha.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gt.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bx.nszjky.cn

[B07] while 循环
来源：http://nq.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://gs.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sa.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://mh.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://xa.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://cr.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lh.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://zl.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://ag.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://iy.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://yo.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lr.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://tf.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://en.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://pj.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kl.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jq.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://uc.9csxet.cn

[B09] break 与 continue
来源：http://cf.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xk.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hk.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cy.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ea.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fz.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qe.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sz.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xr.szsharing.cn

[B10] 遍历同时拿索引
来源：http://og.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cd.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qy.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ak.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ow.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://py.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ks.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pa.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fu.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://gu.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://yr.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://du.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ak.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zc.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rx.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iv.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://gd.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ns.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://ll.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uv.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pf.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fi.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://me.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yl.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hw.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ra.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hv.9csxet.cn

[B13] 判断是否为数字
来源：http://kp.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://jt.newstarts.cn

PHP:  is_numeric($x)
来源：http://xm.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lm.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://im.shxzskj.cn

Java: x instanceof Number
来源：http://gy.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ot.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://xg.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://dd.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://fb.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ju.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zr.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://fq.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://bi.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://or.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lz.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uv.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qa.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://pc.newstarts.cn

Py:   a and b or not c
来源：http://tm.asd995.cn

PHP:  $a && $b || !$c
来源：http://vc.hnjuh.cn

JS:   a && b || !c
来源：http://sp.huanxung.cn

TS:   a && b || !c
来源：http://ta.newstarts.cn

Java: a && b || !c
来源：http://ou.huixinmuqiang.cn

Go:   a && b || !c
来源：http://ya.bjjhwx.cn

Ruby: a && b || !c
来源：http://tu.huixinmuqiang.cn

C#:   a && b || !c
来源：http://ui.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zw.nicolike.cn

Py:   if not data: return
来源：http://rs.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://na.nszjky.cn

JS:   if (!data) return;
来源：http://it.gzmigu.cn

TS:   if (!data) return;
来源：http://nc.haigaiapp.cn

Java: if (data == null) return;
来源：http://up.newstarts.cn

Go:   if data == nil { return }
来源：http://rx.szsharing.cn

Ruby: return if data.nil?
来源：http://mm.shxzskj.cn

C#:   if (data == null) return;
来源：http://dz.hnjuh.cn

================================================================================
来源：http://ye.yuexingan06.cn

C. 函数与作用域
来源：http://ut.bjjhwx.cn

================================================================================
来源：http://pg.521024.cn

[C01] 定义函数
来源：http://ls.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://tz.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lz.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://sv.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wl.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ja.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wu.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://gt.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kn.gzmigu.cn

[C02] 默认参数
来源：http://jc.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://ah.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nv.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://gn.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ba.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bg.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sa.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://qf.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://as.jianghongdianzi.cn

[C03] 可变参数
来源：http://pc.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://di.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cw.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lh.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kl.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ez.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fc.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rv.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sx.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://ej.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lj.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://om.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nb.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tr.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ry.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://gx.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://qi.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://cu.newstarts.cn

[C05] 返回多个值
来源：http://ls.newstarts.cn

Py:   return a, b
来源：http://gx.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://ua.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nz.shxzskj.cn

TS:   return { a, b };
来源：http://wu.lnxyls.cn


<!-- 参考信息 -->