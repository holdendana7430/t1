代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qw.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gs.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wm.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xy.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://io.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ch.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sf.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ug.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://ez.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://hm.521024.cn

PHP:  ord("A"); chr(65)
来源：http://to.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ov.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://be.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://de.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wl.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://ld.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://bp.chemitech.net.cn

[A19] 交换两个变量
来源：http://kv.hnjuh.cn

Py:   a, b = b, a
来源：http://in.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gl.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://nf.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://bs.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://ia.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://tb.nicolike.cn

Ruby: a, b = b, a
来源：http://jj.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://hl.wgjwhj.cn

[A20] 读取标准输入
来源：http://gw.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://he.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uw.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qg.colortex.cn

TS:   // Node.js：readline 模块
来源：http://cv.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://cj.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wg.shtwfgs.cn

Ruby: gets.chomp
来源：http://br.huanxung.cn

C#:   Console.ReadLine();
来源：http://yf.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://rl.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://mb.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://up.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://xm.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://up.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://vm.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xw.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://dy.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://wh.hnjuh.cn

[A22] 获取字符串长度
来源：http://av.nszjky.cn

Py:   len(s)
来源：http://jy.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ze.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iw.szsharing.cn

TS:   s.length
来源：http://mp.shxzskj.cn

Java: s.length()
来源：http://aj.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pw.asd995.cn

Ruby: s.length
来源：http://ja.huanxung.cn

C#:   s.Length
来源：http://sl.haigaiapp.cn

[A23] 大小写转换
来源：http://gk.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://iu.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jv.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wz.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ma.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ff.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wc.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://td.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vy.chemitech.net.cn

[A24] 去除首尾空白
来源：http://nw.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zg.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cy.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tq.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zk.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sj.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://kk.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zr.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bi.newstarts.cn

[A25] 字符串比较
来源：http://lu.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://ta.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bq.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lh.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yi.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jv.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zx.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zc.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nn.haigaiapp.cn

[A26] 类型转换总览
来源：http://kc.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mp.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fd.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hq.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://th.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wn.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bk.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zn.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nz.huixinmuqiang.cn

================================================================================
来源：http://wi.yuexingan06.cn

B. 流程控制
来源：http://tk.chemitech.net.cn

================================================================================
来源：http://fu.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://mr.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yk.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gu.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hp.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kw.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qq.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rg.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qc.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dl.9csxet.cn

[B02] 多分支 else if / elif
来源：http://qk.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vi.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lr.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ea.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://do.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lq.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://po.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cs.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.gzmigu.cn

[B03] switch / match / case
来源：http://ew.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://be.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ci.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bu.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tf.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xy.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pz.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ur.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qm.521024.cn

[B04] for 计数循环
来源：http://rp.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://by.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qb.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://en.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bp.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ey.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eq.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://ly.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dy.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://ac.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://ht.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gm.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ae.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vu.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qt.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wf.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://hj.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://du.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://cn.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://if.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ss.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xy.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ut.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nm.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hd.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ll.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ln.nszjky.cn

[B07] while 循环
来源：http://ua.huanxung.cn

Py:   while i < 10: i += 1
来源：http://ij.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://og.521024.cn

JS:   while (i < 10) { i++; }
来源：http://zi.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://tf.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://bd.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vl.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://hi.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://le.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://ti.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://ob.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fp.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://kt.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://ip.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://ld.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cu.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://of.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://cu.wgjwhj.cn

[B09] break 与 continue
来源：http://qe.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vw.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xx.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bm.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tv.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lt.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ly.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ra.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fs.9csxet.cn

[B10] 遍历同时拿索引
来源：http://xs.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gq.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ip.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zj.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jn.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ag.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fb.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://na.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ca.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://uy.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://gw.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://uu.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jl.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rr.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gt.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ut.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://ch.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hj.asd995.cn

[B12] 跳出多层循环
来源：http://mc.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zv.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ez.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gx.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ki.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zm.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dw.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yp.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://du.szxytkj.cn

[B13] 判断是否为数字
来源：http://qf.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://be.nicolike.cn

PHP:  is_numeric($x)
来源：http://pu.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ed.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jk.shxzukj.cn

Java: x instanceof Number
来源：http://rw.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yp.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://yg.9csxet.cn

C#:   x is int or double or decimal
来源：http://ac.9csxet.cn

[B14] 判断值是否在集合内
来源：http://bm.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://si.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fm.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://ss.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://kg.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uc.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hf.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qv.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oy.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://vn.shxzukj.cn

Py:   a and b or not c
来源：http://ad.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://np.panjiajie.cn

JS:   a && b || !c
来源：http://qt.wgjwhj.cn

TS:   a && b || !c
来源：http://pr.asd995.cn

Java: a && b || !c
来源：http://ww.haigaiapp.cn

Go:   a && b || !c
来源：http://py.gzmigu.cn

Ruby: a && b || !c
来源：http://lt.asd995.cn

C#:   a && b || !c
来源：http://cn.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zd.huixinmuqiang.cn

Py:   if not data: return
来源：http://hk.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://ey.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://fx.szxytkj.cn

TS:   if (!data) return;
来源：http://tf.521024.cn

Java: if (data == null) return;
来源：http://ca.shxzukj.cn

Go:   if data == nil { return }
来源：http://ed.wgjwhj.cn

Ruby: return if data.nil?
来源：http://gm.nicolike.cn

C#:   if (data == null) return;
来源：http://dx.bookmarksfly.cn

================================================================================
来源：http://fl.yuntaijiaju.cn

C. 函数与作用域
来源：http://nz.lnxyls.cn

================================================================================
来源：http://ea.wgjwhj.cn

[C01] 定义函数
来源：http://xf.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://sx.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qn.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://og.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://us.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nc.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vf.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://sq.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ku.bookmarksfly.cn

[C02] 默认参数
来源：http://kf.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://ew.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xk.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://ma.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wd.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tv.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fd.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://qc.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://gf.colortex.cn

[C03] 可变参数
来源：http://vy.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://wk.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://id.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dd.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ro.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ow.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oz.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rr.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yj.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://pw.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pt.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fk.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lt.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wd.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://hd.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://od.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://jh.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://rh.gzmigu.cn

[C05] 返回多个值
来源：http://zk.bookmarksfly.cn

Py:   return a, b
来源：http://uf.newstarts.cn

PHP:  return [$a, $b];
来源：http://pw.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kp.shtwfgs.cn

TS:   return { a, b };
来源：http://xi.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yq.jianghongdianzi.cn

Go:   return a, b
来源：http://eh.hnjuh.cn

Ruby: return a, b
来源：http://ok.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://ee.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://fs.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://pd.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aj.shxzukj.cn

JS:   const square = x => x * x;
来源：http://qo.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://zx.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gy.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ti.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://ul.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ti.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://sl.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bj.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hu.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sr.bookmarksfly.cn

TS:   arr.map(String)
来源：http://jt.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://on.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mp.chemitech.net.cn


<!-- 参考信息 -->