代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://mz.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://fv.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://ud.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zy.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ai.521024.cn

Java: (int) 'A'; (char) 65
来源：http://tr.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qc.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://uo.521024.cn

C#:   (int)'A'; (char)65
来源：http://bj.huixiangedu.cn

[A19] 交换两个变量
来源：http://tf.panjiajie.cn

Py:   a, b = b, a
来源：http://ry.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vr.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://bo.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://ed.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://zu.huanxung.cn

Go:   a, b = b, a
来源：http://oj.nicolike.cn

Ruby: a, b = b, a
来源：http://fn.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://py.colortex.cn

[A20] 读取标准输入
来源：http://fs.gzmigu.cn

Py:   name = input("请输入：")
来源：http://oz.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gk.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ki.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://pv.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://db.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tn.gzmigu.cn

Ruby: gets.chomp
来源：http://qa.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://ev.huanxung.cn

[A21] 保留指定小数位输出
来源：http://no.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://jl.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wv.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://qe.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://kj.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://lb.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jj.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://nz.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://ji.shxzukj.cn

[A22] 获取字符串长度
来源：http://og.jctech888.com.cn

Py:   len(s)
来源：http://fj.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qm.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zx.colortex.cn

TS:   s.length
来源：http://ba.shtwfgs.cn

Java: s.length()
来源：http://zy.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xd.bjjhwx.cn

Ruby: s.length
来源：http://qq.wgjwhj.cn

C#:   s.Length
来源：http://yy.muxihuayi.cn

[A23] 大小写转换
来源：http://cq.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eu.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hy.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ku.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ln.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ab.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gm.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iz.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bq.521024.cn

[A24] 去除首尾空白
来源：http://bp.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zo.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://by.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kp.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hc.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://se.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://kl.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vo.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rr.chemitech.net.cn

[A25] 字符串比较
来源：http://ua.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://bx.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fh.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ss.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bg.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wc.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lg.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yz.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ah.asd995.cn

[A26] 类型转换总览
来源：http://ja.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pb.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ne.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xk.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://bx.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vq.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ke.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fv.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nn.colortex.cn

================================================================================
来源：http://st.nszjky.cn

B. 流程控制
来源：http://fk.panjiajie.cn

================================================================================
来源：http://kr.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://hn.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oz.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ul.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ct.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fj.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tg.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vo.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ik.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yi.newstarts.cn

[B02] 多分支 else if / elif
来源：http://zw.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yh.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://am.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dh.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bx.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lr.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sj.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ki.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.haigaiapp.cn

[B03] switch / match / case
来源：http://ly.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://by.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ar.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yi.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gv.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ai.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pt.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://on.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uh.szxytkj.cn

[B04] for 计数循环
来源：http://ur.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://fc.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cc.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gm.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://da.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ae.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iu.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://oq.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://it.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://nb.colortex.cn

Py:   for item in arr: print(item)
来源：http://jn.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dr.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sp.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xx.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fc.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jh.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://sy.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oj.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://jp.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jo.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pq.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yt.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://py.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jy.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sr.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cy.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ix.panjiajie.cn

[B07] while 循环
来源：http://jd.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://xz.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oy.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://zo.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://tt.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://ah.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mb.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://hf.521024.cn

C#:   while (i < 10) { i++; }
来源：http://oj.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://pt.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://ui.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sd.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://pf.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://er.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://bi.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://og.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ax.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://yu.hahajie.cn

[B09] break 与 continue
来源：http://gp.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bl.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hn.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qd.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://es.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qd.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://on.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uu.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://on.asd995.cn

[B10] 遍历同时拿索引
来源：http://py.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zn.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dc.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bf.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dz.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ll.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://he.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dr.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hd.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://hg.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://ol.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://oc.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dg.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://va.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://of.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zo.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://et.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://np.hnjuh.cn

[B12] 跳出多层循环
来源：http://pu.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dx.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zl.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ap.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jk.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aj.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sf.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rr.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gs.huixiangedu.cn

[B13] 判断是否为数字
来源：http://rf.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://au.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://ms.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eo.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gz.newstarts.cn

Java: x instanceof Number
来源：http://do.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gx.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://cq.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://gc.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://kz.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cj.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://on.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://gs.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://gv.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xq.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ai.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qf.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iz.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://ve.shxzukj.cn

Py:   a and b or not c
来源：http://kt.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://az.jctech888.com.cn

JS:   a && b || !c
来源：http://mm.huixinmuqiang.cn

TS:   a && b || !c
来源：http://sm.yuntaijiaju.cn

Java: a && b || !c
来源：http://im.wgjwhj.cn

Go:   a && b || !c
来源：http://lb.nicolike.cn

Ruby: a && b || !c
来源：http://bb.nszjky.cn

C#:   a && b || !c
来源：http://lb.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rc.haigaiapp.cn

Py:   if not data: return
来源：http://rr.521024.cn

PHP:  if (!$data) { return; }
来源：http://ea.huanxung.cn

JS:   if (!data) return;
来源：http://qc.521024.cn

TS:   if (!data) return;
来源：http://rx.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://fw.hnjuh.cn

Go:   if data == nil { return }
来源：http://up.panjiajie.cn

Ruby: return if data.nil?
来源：http://la.bjjhwx.cn

C#:   if (data == null) return;
来源：http://mw.huanxung.cn

================================================================================
来源：http://wu.9csxet.cn

C. 函数与作用域
来源：http://tx.chemitech.net.cn

================================================================================
来源：http://un.gzmigu.cn

[C01] 定义函数
来源：http://kc.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://mu.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tp.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://lc.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vd.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kg.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://at.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://zz.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://on.521024.cn

[C02] 默认参数
来源：http://lw.asd995.cn

Py:   def greet(name="World"): return name
来源：http://tr.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sb.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://fu.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qt.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pq.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fi.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://qx.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://ck.yuexingan06.cn

[C03] 可变参数
来源：http://pq.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://gd.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wo.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cv.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ud.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bd.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mt.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ji.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hi.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://be.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aj.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ux.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qi.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ok.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://my.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://rw.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://cy.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://wk.hahajie.cn

[C05] 返回多个值
来源：http://bk.huixiangedu.cn

Py:   return a, b
来源：http://qi.newstarts.cn

PHP:  return [$a, $b];
来源：http://rs.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ry.yuntaijiaju.cn

TS:   return { a, b };
来源：http://ah.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yj.9csxet.cn

Go:   return a, b
来源：http://qp.bookmarksfly.cn

Ruby: return a, b
来源：http://gn.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://ab.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://ll.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://cv.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mo.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://uf.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ix.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ue.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qc.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://am.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xp.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://ia.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xj.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vp.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ns.haigaiapp.cn

TS:   arr.map(String)
来源：http://de.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hu.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mp.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://se.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jb.asd995.cn

[C08] 闭包
来源：http://hl.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ie.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bw.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wm.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wf.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uy.jianghongdianzi.cn


<!-- 参考信息 -->