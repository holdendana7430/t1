代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zd.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ht.szsharing.cn

TS:   if (!x) {}
来源：http://ot.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rf.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gg.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ab.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pw.lnxyls.cn

[A17] 位运算
来源：http://he.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ti.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ls.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oo.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mv.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ar.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ta.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nf.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jc.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://tm.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://wh.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://za.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xb.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vw.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://kr.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bh.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://lg.colortex.cn

C#:   (int)'A'; (char)65
来源：http://gr.haigaiapp.cn

[A19] 交换两个变量
来源：http://tl.nicolike.cn

Py:   a, b = b, a
来源：http://sa.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yo.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://de.colortex.cn

TS:   [a, b] = [b, a];
来源：http://ff.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://is.bjjhwx.cn

Go:   a, b = b, a
来源：http://eu.huanxung.cn

Ruby: a, b = b, a
来源：http://ux.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://iu.asd995.cn

[A20] 读取标准输入
来源：http://bn.huanxung.cn

Py:   name = input("请输入：")
来源：http://gk.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ge.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ae.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://pd.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://xr.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sc.szsharing.cn

Ruby: gets.chomp
来源：http://pr.9csxet.cn

C#:   Console.ReadLine();
来源：http://tp.nszjky.cn

[A21] 保留指定小数位输出
来源：http://ff.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://qg.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fw.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://qr.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://xw.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://sf.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qf.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://ut.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://co.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://ke.bookmarksfly.cn

Py:   len(s)
来源：http://pu.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zb.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://of.szsharing.cn

TS:   s.length
来源：http://xg.chemitech.net.cn

Java: s.length()
来源：http://bs.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jw.hahajie.cn

Ruby: s.length
来源：http://cs.muxihuayi.cn

C#:   s.Length
来源：http://vv.gzmigu.cn

[A23] 大小写转换
来源：http://ra.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bn.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jn.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oj.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ea.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ta.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://go.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sh.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vi.shtwfgs.cn

[A24] 去除首尾空白
来源：http://ro.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dy.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://so.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://du.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sw.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wx.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://mq.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zp.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nm.jianghongdianzi.cn

[A25] 字符串比较
来源：http://fo.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://ck.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xa.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://da.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cn.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://db.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://be.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://be.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jf.szsharing.cn

[A26] 类型转换总览
来源：http://vn.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wi.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uh.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wl.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://wx.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dc.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yo.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xw.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qg.nicolike.cn

================================================================================
来源：http://sj.muxihuayi.cn

B. 流程控制
来源：http://cm.newstarts.cn

================================================================================
来源：http://wz.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://sp.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gf.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://no.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wi.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vd.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rb.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sq.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ek.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gc.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://uq.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ow.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://am.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ib.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wd.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ki.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wh.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uj.muxihuayi.cn

[B03] switch / match / case
来源：http://kh.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vo.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ch.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kq.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mr.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rg.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pj.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wj.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xa.panjiajie.cn

[B04] for 计数循环
来源：http://hj.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://nw.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://la.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yg.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ud.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aa.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dm.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://jp.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gk.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://ef.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://wj.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bt.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hb.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ql.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uq.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nb.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://br.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bw.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://qo.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wz.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mc.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yz.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gs.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aa.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rk.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gx.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wn.bookmarksfly.cn

[B07] while 循环
来源：http://xy.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://at.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ck.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://sj.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://bv.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://lp.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eh.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://ea.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://nr.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://pg.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://iz.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tu.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://de.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://vm.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://vv.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ko.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ii.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://ll.yuntaijiaju.cn

[B09] break 与 continue
来源：http://df.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wz.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tx.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://td.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hf.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mw.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dr.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pq.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zi.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ty.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ga.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mh.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mx.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ou.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://et.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gr.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bl.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mt.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://hr.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://bo.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://sl.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nd.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hn.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oc.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zx.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://hs.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gp.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ws.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kc.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pg.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uu.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vq.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jh.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mn.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ws.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nv.asd995.cn

[B13] 判断是否为数字
来源：http://ad.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://cr.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://cc.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sb.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ft.yuexingan06.cn

Java: x instanceof Number
来源：http://gq.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ml.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://cq.szsharing.cn

C#:   x is int or double or decimal
来源：http://rz.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://bt.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://to.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kt.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://tz.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://vs.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cw.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pn.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oz.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wq.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://in.jianghongdianzi.cn

Py:   a and b or not c
来源：http://jk.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://ve.shxzskj.cn

JS:   a && b || !c
来源：http://vn.gzmigu.cn

TS:   a && b || !c
来源：http://yk.bjjhwx.cn

Java: a && b || !c
来源：http://nd.yuntaijiaju.cn

Go:   a && b || !c
来源：http://gi.panjiajie.cn

Ruby: a && b || !c
来源：http://mu.hnjuh.cn

C#:   a && b || !c
来源：http://tb.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jv.shxzukj.cn

Py:   if not data: return
来源：http://oa.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://gc.chemitech.net.cn

JS:   if (!data) return;
来源：http://ch.huixiangedu.cn

TS:   if (!data) return;
来源：http://hj.521024.cn

Java: if (data == null) return;
来源：http://xk.colortex.cn

Go:   if data == nil { return }
来源：http://cp.shxzukj.cn

Ruby: return if data.nil?
来源：http://zy.asd995.cn

C#:   if (data == null) return;
来源：http://zl.huixiangedu.cn

================================================================================
来源：http://ab.jctech888.com.cn

C. 函数与作用域
来源：http://wo.muxihuayi.cn

================================================================================
来源：http://yd.asd995.cn

[C01] 定义函数
来源：http://gh.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://dw.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ra.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://cv.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dw.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ao.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qf.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://nn.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ng.newstarts.cn

[C02] 默认参数
来源：http://jz.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://bc.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wb.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://cm.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ba.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bt.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xw.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://vp.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://aa.asd995.cn

[C03] 可变参数
来源：http://em.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://ir.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oz.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wc.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yh.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ts.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xm.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sq.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wi.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://aa.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vy.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rl.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sf.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jp.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://as.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://tg.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://rb.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://zi.yuexingan06.cn

[C05] 返回多个值
来源：http://bl.bookmarksfly.cn

Py:   return a, b
来源：http://bk.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://qs.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lr.newstarts.cn

TS:   return { a, b };
来源：http://ay.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xp.bjjhwx.cn

Go:   return a, b
来源：http://yl.shxzukj.cn

Ruby: return a, b
来源：http://yx.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://zn.asd995.cn

[C06] 匿名函数 / lambda
来源：http://by.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://ff.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ik.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://xe.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://wa.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ka.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dv.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://uu.huixinmuqiang.cn


<!-- 参考信息 -->