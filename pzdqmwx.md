代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tz.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ws.hahajie.cn

TS:   if (!x) {}
来源：http://dv.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://et.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jx.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pw.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ss.panjiajie.cn

[A17] 位运算
来源：http://xq.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://np.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://at.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yz.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ko.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pq.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nu.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bd.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://av.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://hs.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://nf.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://hp.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eh.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://do.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://oi.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qj.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://jk.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://zk.haigaiapp.cn

[A19] 交换两个变量
来源：http://su.bjjhwx.cn

Py:   a, b = b, a
来源：http://fn.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://un.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://zn.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://tr.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://zz.szxytkj.cn

Go:   a, b = b, a
来源：http://wz.asd995.cn

Ruby: a, b = b, a
来源：http://gh.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://dy.szxytkj.cn

[A20] 读取标准输入
来源：http://os.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://kk.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ff.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ke.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://tx.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://dx.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ch.hnjuh.cn

Ruby: gets.chomp
来源：http://fw.newstarts.cn

C#:   Console.ReadLine();
来源：http://yy.asd995.cn

[A21] 保留指定小数位输出
来源：http://wd.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://dt.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://za.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://on.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://hu.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://iz.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xa.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://la.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://ys.bjjhwx.cn

[A22] 获取字符串长度
来源：http://em.asd995.cn

Py:   len(s)
来源：http://in.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gu.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ly.shtwfgs.cn

TS:   s.length
来源：http://cv.nszjky.cn

Java: s.length()
来源：http://pl.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wn.huanxung.cn

Ruby: s.length
来源：http://ca.nszjky.cn

C#:   s.Length
来源：http://hh.hnjuh.cn

[A23] 大小写转换
来源：http://cw.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ns.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zl.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ln.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lq.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dn.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fl.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://to.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nj.szsharing.cn

[A24] 去除首尾空白
来源：http://rf.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vy.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rl.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bz.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rg.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bg.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://zm.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ho.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dc.wgjwhj.cn

[A25] 字符串比较
来源：http://ix.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://xw.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ue.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vk.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jq.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nb.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yf.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hy.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lp.szsharing.cn

[A26] 类型转换总览
来源：http://nc.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wm.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ud.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bs.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://lu.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ca.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gk.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mi.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ir.bookmarksfly.cn

================================================================================
来源：http://px.nicolike.cn

B. 流程控制
来源：http://dh.huixiangedu.cn

================================================================================
来源：http://vp.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://bd.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yh.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qx.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fw.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wg.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://md.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qb.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://md.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ze.9csxet.cn

[B02] 多分支 else if / elif
来源：http://qi.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lz.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xo.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sr.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jr.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hh.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dj.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rr.jianghongdianzi.cn

[B03] switch / match / case
来源：http://iu.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lr.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yg.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cx.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bk.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vi.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lo.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kh.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ac.szsharing.cn

[B04] for 计数循环
来源：http://qw.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://mb.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tb.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dy.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rs.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ro.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tm.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://gw.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://of.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://rg.szsharing.cn

Py:   for item in arr: print(item)
来源：http://hm.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pb.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nq.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wy.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nt.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ey.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://ux.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pm.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://gt.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pl.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ex.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sc.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lm.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yq.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pn.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bv.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://na.huixiangedu.cn

[B07] while 循环
来源：http://li.newstarts.cn

Py:   while i < 10: i += 1
来源：http://wt.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cv.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://mf.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://nz.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://fl.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lt.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://bq.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://ab.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://ng.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://gw.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pg.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://db.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://sg.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://xi.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iv.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ga.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://rf.huixinmuqiang.cn

[B09] break 与 continue
来源：http://np.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://op.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kr.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wx.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zk.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hy.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ja.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zi.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gq.colortex.cn

[B10] 遍历同时拿索引
来源：http://mm.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vm.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sp.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://td.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uz.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nx.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://af.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uo.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mw.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://rq.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://kq.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://bl.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lb.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jt.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mr.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ls.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://rw.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wy.bjjhwx.cn

[B12] 跳出多层循环
来源：http://be.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ok.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://om.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wn.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mm.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ph.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ir.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qb.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ul.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://jr.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://bq.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://oc.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jx.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mx.chemitech.net.cn

Java: x instanceof Number
来源：http://pr.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sm.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://af.colortex.cn

C#:   x is int or double or decimal
来源：http://gb.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://ez.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pv.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cm.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://hv.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://qj.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xv.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fw.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cc.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cy.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://fc.jianghongdianzi.cn

Py:   a and b or not c
来源：http://ef.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://ms.huixinmuqiang.cn

JS:   a && b || !c
来源：http://wx.szxytkj.cn

TS:   a && b || !c
来源：http://tb.gzmigu.cn

Java: a && b || !c
来源：http://bh.jianghongdianzi.cn

Go:   a && b || !c
来源：http://kj.chemitech.net.cn

Ruby: a && b || !c
来源：http://uh.wgjwhj.cn

C#:   a && b || !c
来源：http://cb.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://le.jctech888.com.cn

Py:   if not data: return
来源：http://or.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://dc.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://ee.hnjuh.cn

TS:   if (!data) return;
来源：http://fy.bjjhwx.cn

Java: if (data == null) return;
来源：http://pi.nszjky.cn

Go:   if data == nil { return }
来源：http://if.jctech888.com.cn

Ruby: return if data.nil?
来源：http://cq.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://bd.shtwfgs.cn

================================================================================
来源：http://te.hnjuh.cn

C. 函数与作用域
来源：http://ag.colortex.cn

================================================================================
来源：http://gx.haigaiapp.cn

[C01] 定义函数
来源：http://cj.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://me.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rs.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://as.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cy.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fl.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yw.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://hd.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nv.asd995.cn

[C02] 默认参数
来源：http://aa.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://mt.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bo.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://hb.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://if.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fx.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bc.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://od.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://vw.szsharing.cn

[C03] 可变参数
来源：http://kb.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://zt.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pr.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pj.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rt.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pv.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vm.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zv.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ck.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://nn.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ay.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bx.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uw.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ux.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://iq.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://hi.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://cr.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://fh.bookmarksfly.cn

[C05] 返回多个值
来源：http://xf.nicolike.cn

Py:   return a, b
来源：http://uj.huanxung.cn

PHP:  return [$a, $b];
来源：http://cy.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oy.muxihuayi.cn

TS:   return { a, b };
来源：http://yn.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yr.lnxyls.cn

Go:   return a, b
来源：http://pv.shxzskj.cn

Ruby: return a, b
来源：http://ak.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://qr.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://hz.nszjky.cn

Py:   square = lambda x: x * x
来源：http://dp.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gp.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://qt.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://xa.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kg.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eh.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://iv.521024.cn


<!-- 参考信息 -->