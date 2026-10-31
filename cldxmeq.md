代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dq.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qv.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tz.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://om.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rs.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zv.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ox.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wb.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://lk.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://bn.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://bw.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ny.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oz.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://gb.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lk.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://wj.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://sb.521024.cn

[A19] 交换两个变量
来源：http://so.bjjhwx.cn

Py:   a, b = b, a
来源：http://uv.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wn.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://ri.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://xk.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://kn.lnxyls.cn

Go:   a, b = b, a
来源：http://dk.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://tm.521024.cn

C#:   (a, b) = (b, a);
来源：http://hq.huixiangedu.cn

[A20] 读取标准输入
来源：http://nd.shxzskj.cn

Py:   name = input("请输入：")
来源：http://pf.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ww.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aq.asd995.cn

TS:   // Node.js：readline 模块
来源：http://mg.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://od.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zw.panjiajie.cn

Ruby: gets.chomp
来源：http://br.hahajie.cn

C#:   Console.ReadLine();
来源：http://yt.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://tx.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://io.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pt.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://px.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://ur.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://oh.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fh.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://tu.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://cj.9csxet.cn

[A22] 获取字符串长度
来源：http://kl.shtwfgs.cn

Py:   len(s)
来源：http://iz.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nz.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iq.9csxet.cn

TS:   s.length
来源：http://fx.asd995.cn

Java: s.length()
来源：http://ox.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ba.colortex.cn

Ruby: s.length
来源：http://qe.wgjwhj.cn

C#:   s.Length
来源：http://gp.shxzskj.cn

[A23] 大小写转换
来源：http://jr.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pv.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cw.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iy.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cz.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jl.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://md.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fr.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zt.shxzukj.cn

[A24] 去除首尾空白
来源：http://ui.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ql.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://il.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gz.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ea.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fq.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://me.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rn.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xh.lnxyls.cn

[A25] 字符串比较
来源：http://bo.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://ny.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ko.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xb.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://od.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://da.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://np.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rf.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wg.newstarts.cn

[A26] 类型转换总览
来源：http://he.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bc.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yf.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zz.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://pg.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iv.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xd.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mz.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dq.panjiajie.cn

================================================================================
来源：http://gk.newstarts.cn

B. 流程控制
来源：http://tm.shxzskj.cn

================================================================================
来源：http://gw.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://rw.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://el.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://js.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jc.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iv.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rd.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uv.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gb.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jx.nszjky.cn

[B02] 多分支 else if / elif
来源：http://tm.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://er.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fi.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qr.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ug.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lk.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://da.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ze.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jq.lnxyls.cn

[B03] switch / match / case
来源：http://bb.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uq.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vg.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gw.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ey.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ho.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ch.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://io.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ap.9csxet.cn

[B04] for 计数循环
来源：http://vn.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://aw.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cy.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bp.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ct.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oy.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tk.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://cg.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hr.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://lj.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://yk.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dg.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kn.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nw.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://co.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uo.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://fe.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jk.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://jc.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ko.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pl.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wj.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zz.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dw.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uc.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://su.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vn.wgjwhj.cn

[B07] while 循环
来源：http://ds.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://lk.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wf.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://xi.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://mr.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://os.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://my.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://tc.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://jt.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://qa.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://qp.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sf.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://yv.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://ci.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://kp.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bf.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jz.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://dl.jianghongdianzi.cn

[B09] break 与 continue
来源：http://ta.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xq.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sw.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yk.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fd.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ca.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hj.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ay.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ny.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://jf.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://io.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nk.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kv.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tb.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://di.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cz.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gu.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://su.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://da.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://vy.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://th.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iw.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://td.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sg.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cx.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://db.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://un.huixiangedu.cn

[B12] 跳出多层循环
来源：http://ly.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oy.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dm.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mp.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tw.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://up.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mw.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ld.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://om.nicolike.cn

[B13] 判断是否为数字
来源：http://zb.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://ey.asd995.cn

PHP:  is_numeric($x)
来源：http://hn.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kb.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qk.hahajie.cn

Java: x instanceof Number
来源：http://ap.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://de.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://hu.shxzukj.cn

C#:   x is int or double or decimal
来源：http://sy.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://cc.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ab.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ok.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://iw.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://to.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qi.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vq.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rv.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ta.asd995.cn

[B15] 布尔运算与取反
来源：http://co.hnjuh.cn

Py:   a and b or not c
来源：http://id.asd995.cn

PHP:  $a && $b || !$c
来源：http://sx.szsharing.cn

JS:   a && b || !c
来源：http://qy.huixiangedu.cn

TS:   a && b || !c
来源：http://oq.jctech888.com.cn

Java: a && b || !c
来源：http://ph.jianghongdianzi.cn

Go:   a && b || !c
来源：http://le.chemitech.net.cn

Ruby: a && b || !c
来源：http://ex.yuntaijiaju.cn

C#:   a && b || !c
来源：http://cx.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ze.huixiangedu.cn

Py:   if not data: return
来源：http://wq.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://sd.nszjky.cn

JS:   if (!data) return;
来源：http://es.nicolike.cn

TS:   if (!data) return;
来源：http://wn.szsharing.cn

Java: if (data == null) return;
来源：http://rw.newstarts.cn

Go:   if data == nil { return }
来源：http://mu.colortex.cn

Ruby: return if data.nil?
来源：http://aa.shtwfgs.cn

C#:   if (data == null) return;
来源：http://af.hnjuh.cn

================================================================================
来源：http://ug.szxytkj.cn

C. 函数与作用域
来源：http://la.huixinmuqiang.cn

================================================================================
来源：http://mb.9csxet.cn

[C01] 定义函数
来源：http://va.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://cb.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zp.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://rj.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hx.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gn.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ep.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://rx.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ar.bookmarksfly.cn

[C02] 默认参数
来源：http://bq.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://zi.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dm.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://ck.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://me.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hx.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ng.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://lf.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://vh.asd995.cn

[C03] 可变参数
来源：http://sp.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://mk.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dg.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jb.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://je.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kx.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ra.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sw.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ca.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://je.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tu.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jw.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gu.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dy.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://yh.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://rq.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://ig.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://ik.bjjhwx.cn

[C05] 返回多个值
来源：http://ra.lnxyls.cn

Py:   return a, b
来源：http://cm.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://qe.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sk.shtwfgs.cn

TS:   return { a, b };
来源：http://vp.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://em.szsharing.cn

Go:   return a, b
来源：http://bt.jctech888.com.cn

Ruby: return a, b
来源：http://ll.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://pt.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://dm.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://hf.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ef.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://uu.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://ln.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kk.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dk.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://ms.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ra.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://pq.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yi.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nq.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ov.nicolike.cn

TS:   arr.map(String)
来源：http://ce.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sk.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gy.panjiajie.cn


<!-- 参考信息 -->