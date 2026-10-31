代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ka.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nv.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pp.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hv.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://xj.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://hc.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://dd.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yi.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ic.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://vo.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jk.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://dt.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://fs.9csxet.cn

[A19] 交换两个变量
来源：http://yi.hnjuh.cn

Py:   a, b = b, a
来源：http://yc.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qo.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://ii.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://gn.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://ts.shxzukj.cn

Go:   a, b = b, a
来源：http://cy.hahajie.cn

Ruby: a, b = b, a
来源：http://vz.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://mp.nszjky.cn

[A20] 读取标准输入
来源：http://yy.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://vo.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uo.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lt.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://xc.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://fi.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pc.nszjky.cn

Ruby: gets.chomp
来源：http://kz.hnjuh.cn

C#:   Console.ReadLine();
来源：http://jb.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://ov.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://wk.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qt.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://vn.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://ih.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://tg.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cq.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ci.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://cn.chemitech.net.cn

[A22] 获取字符串长度
来源：http://sh.muxihuayi.cn

Py:   len(s)
来源：http://zk.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rb.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gu.shxzukj.cn

TS:   s.length
来源：http://ca.jianghongdianzi.cn

Java: s.length()
来源：http://ng.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zj.huixiangedu.cn

Ruby: s.length
来源：http://eg.newstarts.cn

C#:   s.Length
来源：http://pq.muxihuayi.cn

[A23] 大小写转换
来源：http://tq.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qs.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nk.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hy.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bo.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wp.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hd.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://az.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lm.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://dk.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jy.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ey.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fd.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ym.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vt.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://ix.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bh.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gv.lnxyls.cn

[A25] 字符串比较
来源：http://oh.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://ns.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yq.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rh.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kx.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eu.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gg.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://os.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wk.521024.cn

[A26] 类型转换总览
来源：http://oj.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zb.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vg.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jg.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://zz.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uc.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pd.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bc.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lb.chemitech.net.cn

================================================================================
来源：http://se.huixiangedu.cn

B. 流程控制
来源：http://vj.yuexingan06.cn

================================================================================
来源：http://uc.shxzskj.cn

[B01] 条件判断 if / else
来源：http://wy.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gx.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cn.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nr.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vo.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dp.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://up.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mp.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nz.nszjky.cn

[B02] 多分支 else if / elif
来源：http://mg.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yt.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ce.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zb.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://di.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ym.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://se.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cm.nszjky.cn

[B03] switch / match / case
来源：http://fe.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zl.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://es.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fx.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gz.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ma.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hp.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kt.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bu.szsharing.cn

[B04] for 计数循环
来源：http://hg.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://qz.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vj.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://za.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qg.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ae.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lg.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://nv.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wr.colortex.cn

[B05] 遍历数组 / 列表
来源：http://tw.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://ku.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qa.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://di.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rh.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qj.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wd.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://fm.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xv.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://ej.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gm.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://li.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rz.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://un.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ph.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jt.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ho.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wb.jctech888.com.cn

[B07] while 循环
来源：http://xu.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://eb.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qr.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://qc.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://qa.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://ze.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yv.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://xp.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://kx.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://nq.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ef.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cy.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://vv.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://nt.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://ob.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dr.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ht.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://uj.szsharing.cn

[B09] break 与 continue
来源：http://ma.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nd.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gj.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ek.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sa.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tx.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jb.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://ih.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fl.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rh.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cx.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iu.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ik.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xt.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ht.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yf.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://qs.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://rf.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://bn.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kp.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fr.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xv.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eo.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://sr.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zk.asd995.cn

[B12] 跳出多层循环
来源：http://jw.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nv.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nu.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zv.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gh.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vl.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bh.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://up.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zf.chemitech.net.cn

[B13] 判断是否为数字
来源：http://jc.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://jl.nicolike.cn

PHP:  is_numeric($x)
来源：http://an.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://al.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ay.wgjwhj.cn

Java: x instanceof Number
来源：http://vk.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bq.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://tq.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ek.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://bu.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ts.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vd.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://kc.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://md.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fg.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tv.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wm.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://li.lnxyls.cn

[B15] 布尔运算与取反
来源：http://jj.hahajie.cn

Py:   a and b or not c
来源：http://qt.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://oq.panjiajie.cn

JS:   a && b || !c
来源：http://pd.shxzukj.cn

TS:   a && b || !c
来源：http://fu.chemitech.net.cn

Java: a && b || !c
来源：http://al.jctech888.com.cn

Go:   a && b || !c
来源：http://ko.nicolike.cn

Ruby: a && b || !c
来源：http://cm.bjjhwx.cn

C#:   a && b || !c
来源：http://vt.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yx.9csxet.cn

Py:   if not data: return
来源：http://bk.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://aj.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://rk.yuexingan06.cn

TS:   if (!data) return;
来源：http://mm.newstarts.cn

Java: if (data == null) return;
来源：http://se.hahajie.cn

Go:   if data == nil { return }
来源：http://ul.hnjuh.cn

Ruby: return if data.nil?
来源：http://nk.jctech888.com.cn

C#:   if (data == null) return;
来源：http://ii.yuntaijiaju.cn

================================================================================
来源：http://as.huixinmuqiang.cn

C. 函数与作用域
来源：http://hx.szsharing.cn

================================================================================
来源：http://eo.lnxyls.cn

[C01] 定义函数
来源：http://xm.asd995.cn

Py:   def add(a, b): return a + b
来源：http://it.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://su.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://bq.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gi.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jk.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iv.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://lt.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ow.hahajie.cn

[C02] 默认参数
来源：http://pl.521024.cn

Py:   def greet(name="World"): return name
来源：http://xl.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dw.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://zn.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://po.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vw.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://us.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://tb.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://gt.panjiajie.cn

[C03] 可变参数
来源：http://uu.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://mb.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uq.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bn.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ty.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hk.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fa.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vx.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://az.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://xx.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wn.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ph.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zl.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ic.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://js.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://yx.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://qy.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://zh.shxzukj.cn

[C05] 返回多个值
来源：http://xd.szsharing.cn

Py:   return a, b
来源：http://ok.szxytkj.cn

PHP:  return [$a, $b];
来源：http://eo.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pu.szsharing.cn

TS:   return { a, b };
来源：http://yc.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://os.shxzskj.cn

Go:   return a, b
来源：http://sq.asd995.cn

Ruby: return a, b
来源：http://tx.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://pv.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://at.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://xr.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wi.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://aw.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://fb.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jb.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yw.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://dq.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ur.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://wr.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yz.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nt.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lw.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://qv.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pn.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wr.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://xh.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dw.bjjhwx.cn

[C08] 闭包
来源：http://au.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oz.yuexingan06.cn


<!-- 参考信息 -->