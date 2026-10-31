代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zc.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cr.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hg.haigaiapp.cn

[A17] 位运算
来源：http://ka.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hn.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fi.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qx.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kd.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tc.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dx.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dj.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ui.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://lp.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://aj.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://mk.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wu.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ij.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://st.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ul.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://to.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://cm.panjiajie.cn

[A19] 交换两个变量
来源：http://ez.nicolike.cn

Py:   a, b = b, a
来源：http://nc.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gv.asd995.cn

JS:   [a, b] = [b, a];
来源：http://mm.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://cs.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://xm.shxzskj.cn

Go:   a, b = b, a
来源：http://rm.panjiajie.cn

Ruby: a, b = b, a
来源：http://fr.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://tx.shtwfgs.cn

[A20] 读取标准输入
来源：http://zt.nicolike.cn

Py:   name = input("请输入：")
来源：http://qb.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://di.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nx.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://dv.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://hh.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wb.panjiajie.cn

Ruby: gets.chomp
来源：http://zz.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://fz.hahajie.cn

[A21] 保留指定小数位输出
来源：http://nv.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://km.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ot.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://wx.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://oc.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://sa.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ye.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://qa.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://os.colortex.cn

[A22] 获取字符串长度
来源：http://ju.szxytkj.cn

Py:   len(s)
来源：http://xg.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ag.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dh.muxihuayi.cn

TS:   s.length
来源：http://ib.shtwfgs.cn

Java: s.length()
来源：http://yr.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oc.gzmigu.cn

Ruby: s.length
来源：http://vp.lnxyls.cn

C#:   s.Length
来源：http://au.yuexingan06.cn

[A23] 大小写转换
来源：http://cz.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hj.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pi.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ct.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ei.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uv.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cr.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xk.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pw.shxzukj.cn

[A24] 去除首尾空白
来源：http://jo.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jv.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wu.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ah.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nu.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cu.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://wn.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zn.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ap.lnxyls.cn

[A25] 字符串比较
来源：http://at.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://wd.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ac.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lv.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vf.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tj.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://df.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ek.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cl.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://yg.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ak.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fs.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jo.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://vf.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qd.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uh.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nw.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bq.newstarts.cn

================================================================================
来源：http://bs.chemitech.net.cn

B. 流程控制
来源：http://mv.gzmigu.cn

================================================================================
来源：http://dc.gzmigu.cn

[B01] 条件判断 if / else
来源：http://nd.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://py.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ae.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jg.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yh.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sw.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hs.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ho.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cy.nszjky.cn

[B02] 多分支 else if / elif
来源：http://si.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ra.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fx.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ka.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eu.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jj.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pw.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tg.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yp.asd995.cn

[B03] switch / match / case
来源：http://cc.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ub.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wy.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hh.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fn.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tk.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ix.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nx.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zv.9csxet.cn

[B04] for 计数循环
来源：http://ui.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://tl.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tn.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sn.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yn.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lu.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fj.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://fe.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://im.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://ov.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://hn.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ac.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zj.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://je.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ds.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qp.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://wj.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ru.colortex.cn

[B06] 遍历字典 / 对象
来源：http://ku.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gu.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lu.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tw.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fr.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dr.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ho.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ib.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wp.shxzskj.cn

[B07] while 循环
来源：http://jr.colortex.cn

Py:   while i < 10: i += 1
来源：http://zg.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rc.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://kd.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://wr.521024.cn

Java: while (i < 10) { i++; }
来源：http://it.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://me.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://ja.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://yw.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://gh.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://bi.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yk.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://ep.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://qx.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://nb.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jw.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zt.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://do.huanxung.cn

[B09] break 与 continue
来源：http://zc.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bb.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ea.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vm.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://li.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nm.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://at.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wr.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ju.colortex.cn

[B10] 遍历同时拿索引
来源：http://fs.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sg.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kz.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fg.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dx.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bq.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fy.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yt.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nj.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://gv.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://mx.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://ou.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://md.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xg.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ns.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rn.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://wl.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mb.szsharing.cn

[B12] 跳出多层循环
来源：http://zp.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mr.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://el.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aa.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xy.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jg.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xf.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lt.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dy.newstarts.cn

[B13] 判断是否为数字
来源：http://qp.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://xd.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://ol.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dz.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pa.shxzukj.cn

Java: x instanceof Number
来源：http://of.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vm.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://rj.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://th.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://sz.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fa.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bw.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://xy.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://ly.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yv.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xb.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nr.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://km.hnjuh.cn

[B15] 布尔运算与取反
来源：http://js.chemitech.net.cn

Py:   a and b or not c
来源：http://vu.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://qn.9csxet.cn

JS:   a && b || !c
来源：http://lf.shtwfgs.cn

TS:   a && b || !c
来源：http://vn.gzmigu.cn

Java: a && b || !c
来源：http://jk.shxzukj.cn

Go:   a && b || !c
来源：http://se.lnxyls.cn

Ruby: a && b || !c
来源：http://nm.shxzskj.cn

C#:   a && b || !c
来源：http://am.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zq.lnxyls.cn

Py:   if not data: return
来源：http://uk.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://lx.huixiangedu.cn

JS:   if (!data) return;
来源：http://rg.shxzukj.cn

TS:   if (!data) return;
来源：http://qc.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://ql.9csxet.cn

Go:   if data == nil { return }
来源：http://vn.lnxyls.cn

Ruby: return if data.nil?
来源：http://ky.panjiajie.cn

C#:   if (data == null) return;
来源：http://zp.muxihuayi.cn

================================================================================
来源：http://pr.huixiangedu.cn

C. 函数与作用域
来源：http://sy.szsharing.cn

================================================================================
来源：http://is.huanxung.cn

[C01] 定义函数
来源：http://qn.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://hz.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dy.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://sp.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://af.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ut.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://di.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://ad.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://os.newstarts.cn

[C02] 默认参数
来源：http://tj.asd995.cn

Py:   def greet(name="World"): return name
来源：http://ag.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xj.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://ky.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lq.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pf.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ie.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://jt.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://gw.colortex.cn

[C03] 可变参数
来源：http://jy.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://hb.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ji.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://td.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tn.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gm.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ic.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gg.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vk.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://sj.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pe.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nr.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nj.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pp.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://ip.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://kp.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://yf.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://mj.jianghongdianzi.cn

[C05] 返回多个值
来源：http://po.wgjwhj.cn

Py:   return a, b
来源：http://kv.hahajie.cn

PHP:  return [$a, $b];
来源：http://qh.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ft.haigaiapp.cn

TS:   return { a, b };
来源：http://mm.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ir.gzmigu.cn

Go:   return a, b
来源：http://mf.lnxyls.cn

Ruby: return a, b
来源：http://we.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://nd.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://wp.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://ez.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cb.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://mt.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ov.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hm.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tk.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://mz.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ww.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://ay.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vy.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://en.yuexingan06.cn


<!-- 参考信息 -->