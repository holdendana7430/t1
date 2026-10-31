代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ra.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pq.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nb.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ai.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://pa.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://ov.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://yd.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wd.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pt.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://sa.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pw.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://mj.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://xz.lnxyls.cn

[A19] 交换两个变量
来源：http://yq.huixiangedu.cn

Py:   a, b = b, a
来源：http://zj.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zz.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://xw.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://xg.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://ck.bjjhwx.cn

Go:   a, b = b, a
来源：http://zf.colortex.cn

Ruby: a, b = b, a
来源：http://by.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://ah.521024.cn

[A20] 读取标准输入
来源：http://kl.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://fw.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rh.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jj.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://bf.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://jn.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rw.lnxyls.cn

Ruby: gets.chomp
来源：http://hg.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://uh.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://dn.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://mv.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://di.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://bd.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://lq.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://ms.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vy.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://sm.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://rh.521024.cn

[A22] 获取字符串长度
来源：http://bf.gzmigu.cn

Py:   len(s)
来源：http://ha.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fz.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ej.szxytkj.cn

TS:   s.length
来源：http://fd.huixinmuqiang.cn

Java: s.length()
来源：http://oe.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dw.wgjwhj.cn

Ruby: s.length
来源：http://no.haigaiapp.cn

C#:   s.Length
来源：http://tp.nszjky.cn

[A23] 大小写转换
来源：http://nl.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://et.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ph.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xl.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pg.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rg.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jj.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ux.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nt.nicolike.cn

[A24] 去除首尾空白
来源：http://yq.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fe.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ym.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vg.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ce.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ja.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://si.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gp.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jm.nszjky.cn

[A25] 字符串比较
来源：http://ai.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://te.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fj.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jq.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gw.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rr.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cd.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uf.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ft.panjiajie.cn

[A26] 类型转换总览
来源：http://pf.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pi.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sq.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ol.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://bi.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://so.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bt.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://id.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qr.muxihuayi.cn

================================================================================
来源：http://ur.chemitech.net.cn

B. 流程控制
来源：http://lz.lnxyls.cn

================================================================================
来源：http://is.szsharing.cn

[B01] 条件判断 if / else
来源：http://tx.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dy.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uu.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://un.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wh.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wa.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ph.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dq.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eh.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://ul.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nt.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fw.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nz.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wm.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jj.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zt.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://af.jianghongdianzi.cn

[B03] switch / match / case
来源：http://fk.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xb.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cf.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lc.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sx.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mx.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bw.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ia.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jl.gzmigu.cn

[B04] for 计数循环
来源：http://xf.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://rh.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pr.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wm.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://az.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sy.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://am.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://aj.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zf.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://md.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://kh.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ha.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cn.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fw.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pw.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pt.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://gj.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bq.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://yb.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ni.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://as.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pk.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ov.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jo.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zm.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ib.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gx.yuntaijiaju.cn

[B07] while 循环
来源：http://ra.521024.cn

Py:   while i < 10: i += 1
来源：http://es.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fb.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://to.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://yj.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://th.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ho.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://jc.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://en.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://vt.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://os.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://km.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://ka.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://ip.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://wz.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bs.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rg.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://ma.szxytkj.cn

[B09] break 与 continue
来源：http://se.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nk.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sp.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://go.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hf.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wo.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ve.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ry.newstarts.cn

[B10] 遍历同时拿索引
来源：http://fk.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jl.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fr.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://as.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zm.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bp.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qo.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ke.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cs.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://la.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://xm.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://us.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kk.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ua.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xk.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cm.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://yr.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kg.newstarts.cn

[B12] 跳出多层循环
来源：http://pi.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://he.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ix.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xc.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cg.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bx.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tm.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ck.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zh.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://io.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://cw.panjiajie.cn

PHP:  is_numeric($x)
来源：http://lw.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xm.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://su.newstarts.cn

Java: x instanceof Number
来源：http://oq.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://il.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://at.nszjky.cn

C#:   x is int or double or decimal
来源：http://ct.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://lb.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zj.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iw.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ns.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://sr.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qn.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jm.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cc.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jz.521024.cn

[B15] 布尔运算与取反
来源：http://uf.nszjky.cn

Py:   a and b or not c
来源：http://oo.newstarts.cn

PHP:  $a && $b || !$c
来源：http://tm.nicolike.cn

JS:   a && b || !c
来源：http://mp.chemitech.net.cn

TS:   a && b || !c
来源：http://gr.9csxet.cn

Java: a && b || !c
来源：http://ab.shxzukj.cn

Go:   a && b || !c
来源：http://si.colortex.cn

Ruby: a && b || !c
来源：http://zy.hahajie.cn

C#:   a && b || !c
来源：http://yo.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wv.hnjuh.cn

Py:   if not data: return
来源：http://lp.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://ey.nicolike.cn

JS:   if (!data) return;
来源：http://zs.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://vd.hnjuh.cn

Java: if (data == null) return;
来源：http://vl.haigaiapp.cn

Go:   if data == nil { return }
来源：http://ri.colortex.cn

Ruby: return if data.nil?
来源：http://kz.hnjuh.cn

C#:   if (data == null) return;
来源：http://no.huanxung.cn

================================================================================
来源：http://lv.521024.cn

C. 函数与作用域
来源：http://sc.521024.cn

================================================================================
来源：http://uh.9csxet.cn

[C01] 定义函数
来源：http://lj.asd995.cn

Py:   def add(a, b): return a + b
来源：http://zt.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jh.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://dk.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wc.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yn.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wc.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://lx.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ht.muxihuayi.cn

[C02] 默认参数
来源：http://nx.521024.cn

Py:   def greet(name="World"): return name
来源：http://cc.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iu.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://oe.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ra.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pa.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ga.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://ni.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://xp.jctech888.com.cn

[C03] 可变参数
来源：http://zj.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://nf.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tm.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dy.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fa.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hb.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lx.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pj.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zd.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://am.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://st.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vv.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ah.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wj.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://sv.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://if.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://ec.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://vp.szxytkj.cn

[C05] 返回多个值
来源：http://qj.chemitech.net.cn

Py:   return a, b
来源：http://pf.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://dc.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vb.shxzskj.cn

TS:   return { a, b };
来源：http://qp.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wt.huixinmuqiang.cn

Go:   return a, b
来源：http://gu.shtwfgs.cn

Ruby: return a, b
来源：http://ik.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://um.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://ok.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://ck.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ga.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://io.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://kk.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bl.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dn.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://lv.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sx.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://ed.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bp.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vx.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ek.panjiajie.cn

TS:   arr.map(String)
来源：http://jl.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kt.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yy.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://zs.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vo.521024.cn

[C08] 闭包
来源：http://fb.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fn.szxytkj.cn


<!-- 参考信息 -->