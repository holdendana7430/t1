代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rd.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ng.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jm.asd995.cn

[A17] 位运算
来源：http://uv.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pm.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ke.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rv.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qg.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ta.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bd.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://va.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ku.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://kp.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://cz.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://ag.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gu.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uk.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://uj.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://me.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://gg.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://yj.gzmigu.cn

[A19] 交换两个变量
来源：http://ey.shxzskj.cn

Py:   a, b = b, a
来源：http://zj.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zh.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://ab.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://dq.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://gn.huixiangedu.cn

Go:   a, b = b, a
来源：http://wb.chemitech.net.cn

Ruby: a, b = b, a
来源：http://vz.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://ek.shtwfgs.cn

[A20] 读取标准输入
来源：http://fy.hnjuh.cn

Py:   name = input("请输入：")
来源：http://eq.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jq.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aw.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://ms.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://qi.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://om.chemitech.net.cn

Ruby: gets.chomp
来源：http://pi.521024.cn

C#:   Console.ReadLine();
来源：http://hc.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://ka.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://ra.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pj.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://hs.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://ht.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://dn.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qt.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://ee.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://zf.haigaiapp.cn

[A22] 获取字符串长度
来源：http://hc.yuexingan06.cn

Py:   len(s)
来源：http://nh.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bg.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jt.hnjuh.cn

TS:   s.length
来源：http://ys.hahajie.cn

Java: s.length()
来源：http://ix.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://km.newstarts.cn

Ruby: s.length
来源：http://lr.nszjky.cn

C#:   s.Length
来源：http://bs.9csxet.cn

[A23] 大小写转换
来源：http://qk.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vl.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mt.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://az.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lt.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xp.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yr.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ve.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lh.szsharing.cn

[A24] 去除首尾空白
来源：http://co.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eq.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nf.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zb.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tq.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vh.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://gb.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ub.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lx.szsharing.cn

[A25] 字符串比较
来源：http://oh.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://kb.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qd.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pm.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ev.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jo.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jd.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jy.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://um.wgjwhj.cn

[A26] 类型转换总览
来源：http://ln.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://le.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ir.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://af.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://vb.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hf.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pm.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dw.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nb.huanxung.cn

================================================================================
来源：http://af.gzmigu.cn

B. 流程控制
来源：http://gc.wgjwhj.cn

================================================================================
来源：http://wn.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://pq.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cm.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pa.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yb.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://se.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xg.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tx.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uu.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ug.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://ds.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gn.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wd.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ik.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wv.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uc.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ac.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zs.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ts.shtwfgs.cn

[B03] switch / match / case
来源：http://bq.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oh.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ef.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://te.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://be.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uf.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://km.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lx.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vz.9csxet.cn

[B04] for 计数循环
来源：http://jq.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://jt.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iz.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cp.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ww.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fs.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ec.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://bq.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jg.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://ku.szsharing.cn

Py:   for item in arr: print(item)
来源：http://bl.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://il.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dz.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vx.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ih.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oq.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://lx.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://he.asd995.cn

[B06] 遍历字典 / 对象
来源：http://sg.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gr.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fd.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sz.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://si.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zl.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lq.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://an.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pk.asd995.cn

[B07] while 循环
来源：http://dh.asd995.cn

Py:   while i < 10: i += 1
来源：http://km.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://so.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://po.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://lz.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://dz.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gk.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://er.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://cq.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://ey.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://ap.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ib.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://co.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://aa.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://ym.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rc.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ms.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://kg.yuntaijiaju.cn

[B09] break 与 continue
来源：http://xs.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oh.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cm.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sb.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sv.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mr.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dx.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kt.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lj.nicolike.cn

[B10] 遍历同时拿索引
来源：http://op.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pz.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nf.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zs.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://th.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sx.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gk.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ha.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qc.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://zl.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://li.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://rj.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vo.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qw.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fm.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bw.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://yz.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sv.bjjhwx.cn

[B12] 跳出多层循环
来源：http://cx.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://il.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://he.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jh.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iz.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vb.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://av.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ma.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aj.wgjwhj.cn

[B13] 判断是否为数字
来源：http://hv.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://wa.huanxung.cn

PHP:  is_numeric($x)
来源：http://mt.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cd.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mh.hnjuh.cn

Java: x instanceof Number
来源：http://qa.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sf.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://to.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://xf.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://ua.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yl.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yv.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://sp.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://kh.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ka.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kh.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kv.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gn.asd995.cn

[B15] 布尔运算与取反
来源：http://ro.hahajie.cn

Py:   a and b or not c
来源：http://jt.newstarts.cn

PHP:  $a && $b || !$c
来源：http://ci.muxihuayi.cn

JS:   a && b || !c
来源：http://hl.panjiajie.cn

TS:   a && b || !c
来源：http://vz.muxihuayi.cn

Java: a && b || !c
来源：http://bm.shtwfgs.cn

Go:   a && b || !c
来源：http://bk.wgjwhj.cn

Ruby: a && b || !c
来源：http://im.gzmigu.cn

C#:   a && b || !c
来源：http://uk.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://es.jianghongdianzi.cn

Py:   if not data: return
来源：http://jx.colortex.cn

PHP:  if (!$data) { return; }
来源：http://om.chemitech.net.cn

JS:   if (!data) return;
来源：http://lt.nszjky.cn

TS:   if (!data) return;
来源：http://be.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://ks.huanxung.cn

Go:   if data == nil { return }
来源：http://wx.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://rr.newstarts.cn

C#:   if (data == null) return;
来源：http://xa.asd995.cn

================================================================================
来源：http://qm.szsharing.cn

C. 函数与作用域
来源：http://sc.nszjky.cn

================================================================================
来源：http://ni.colortex.cn

[C01] 定义函数
来源：http://ol.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://nd.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cx.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://ze.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bx.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cz.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pk.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://gx.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wl.chemitech.net.cn

[C02] 默认参数
来源：http://cd.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://st.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ko.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://by.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ve.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ph.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ni.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://dm.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://hw.nszjky.cn

[C03] 可变参数
来源：http://ug.521024.cn

Py:   def total(*args): return sum(args)
来源：http://kx.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lw.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ta.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nl.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zc.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://re.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gf.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yg.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://jg.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aq.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sz.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yn.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vc.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://zy.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://wq.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://np.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://aw.521024.cn

[C05] 返回多个值
来源：http://pc.jianghongdianzi.cn

Py:   return a, b
来源：http://rc.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://ws.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xu.haigaiapp.cn

TS:   return { a, b };
来源：http://tz.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ff.shxzskj.cn

Go:   return a, b
来源：http://ja.huanxung.cn

Ruby: return a, b
来源：http://rj.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://be.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://ul.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://uh.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qx.hnjuh.cn

JS:   const square = x => x * x;
来源：http://nx.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://gc.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yv.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ox.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://ii.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cg.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://kz.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ii.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cv.yuntaijiaju.cn


<!-- 参考信息 -->