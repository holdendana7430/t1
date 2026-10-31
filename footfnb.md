代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zr.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://rg.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://em.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://oj.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://in.521024.cn

[A19] 交换两个变量
来源：http://zb.huanxung.cn

Py:   a, b = b, a
来源：http://lt.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ms.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://ja.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://ms.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://cb.szxytkj.cn

Go:   a, b = b, a
来源：http://qr.panjiajie.cn

Ruby: a, b = b, a
来源：http://eu.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://sc.lnxyls.cn

[A20] 读取标准输入
来源：http://vi.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://oi.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xo.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ao.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://pi.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://wh.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yy.shtwfgs.cn

Ruby: gets.chomp
来源：http://kb.gzmigu.cn

C#:   Console.ReadLine();
来源：http://uw.nicolike.cn

[A21] 保留指定小数位输出
来源：http://cd.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://qn.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kc.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://pu.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://ub.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://ys.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vn.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://mh.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://ot.haigaiapp.cn

[A22] 获取字符串长度
来源：http://yy.jctech888.com.cn

Py:   len(s)
来源：http://yg.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://la.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sa.hnjuh.cn

TS:   s.length
来源：http://cp.chemitech.net.cn

Java: s.length()
来源：http://wd.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zz.yuexingan06.cn

Ruby: s.length
来源：http://ml.szsharing.cn

C#:   s.Length
来源：http://yo.yuexingan06.cn

[A23] 大小写转换
来源：http://ao.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jn.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hs.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ar.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rf.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hy.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fe.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yl.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ua.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://xw.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://az.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jz.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ry.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kt.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hp.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://sf.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zz.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zv.gzmigu.cn

[A25] 字符串比较
来源：http://ab.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://bc.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oj.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://to.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://up.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sd.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://em.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fc.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ts.newstarts.cn

[A26] 类型转换总览
来源：http://ug.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xu.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cn.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ww.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://nc.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ln.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xg.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hr.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gq.shxzukj.cn

================================================================================
来源：http://tb.nszjky.cn

B. 流程控制
来源：http://aj.yuntaijiaju.cn

================================================================================
来源：http://kc.huanxung.cn

[B01] 条件判断 if / else
来源：http://vi.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wu.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mc.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hj.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dk.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mi.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://so.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://so.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qs.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://kb.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ad.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yf.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dm.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yi.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ra.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ag.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mh.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pz.shtwfgs.cn

[B03] switch / match / case
来源：http://zs.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kg.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lo.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jb.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bw.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uh.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dy.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kp.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rv.hnjuh.cn

[B04] for 计数循环
来源：http://nu.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://ue.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ue.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gn.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hs.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xl.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gk.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://gj.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ao.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://uv.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://zs.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ev.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gx.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tw.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ku.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ao.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://ce.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zt.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://yq.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fg.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xe.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rq.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dt.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hy.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ou.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://da.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jn.yuntaijiaju.cn

[B07] while 循环
来源：http://cd.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://zu.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zm.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://zx.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://sg.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://lq.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xe.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ey.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://sx.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://hf.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://oe.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oa.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://lb.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://vm.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://hb.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wv.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tr.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://sj.bookmarksfly.cn

[B09] break 与 continue
来源：http://no.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tn.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ab.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jy.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jr.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://du.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pl.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kw.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://au.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://ga.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lu.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ph.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ln.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cf.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wc.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yz.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nr.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zv.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://zq.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://rd.colortex.cn

PHP:  range(0, 10, 2);
来源：http://tt.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kz.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://et.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ms.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zw.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://aa.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gb.shtwfgs.cn

[B12] 跳出多层循环
来源：http://xl.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ah.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fu.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ho.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vx.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rr.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tf.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ls.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xj.huanxung.cn

[B13] 判断是否为数字
来源：http://fo.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://ft.panjiajie.cn

PHP:  is_numeric($x)
来源：http://ty.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ri.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gw.yuntaijiaju.cn

Java: x instanceof Number
来源：http://lz.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cb.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://me.shxzskj.cn

C#:   x is int or double or decimal
来源：http://we.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ic.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bx.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eh.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://kt.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://uh.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ol.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://za.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ak.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kg.panjiajie.cn

[B15] 布尔运算与取反
来源：http://dc.nszjky.cn

Py:   a and b or not c
来源：http://pe.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://ak.bjjhwx.cn

JS:   a && b || !c
来源：http://lm.wgjwhj.cn

TS:   a && b || !c
来源：http://qg.shxzukj.cn

Java: a && b || !c
来源：http://yr.hahajie.cn

Go:   a && b || !c
来源：http://qo.szxytkj.cn

Ruby: a && b || !c
来源：http://mk.shtwfgs.cn

C#:   a && b || !c
来源：http://ot.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ri.jctech888.com.cn

Py:   if not data: return
来源：http://it.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://ll.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://yu.hahajie.cn

TS:   if (!data) return;
来源：http://vs.gzmigu.cn

Java: if (data == null) return;
来源：http://va.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://al.bjjhwx.cn

Ruby: return if data.nil?
来源：http://dk.szxytkj.cn

C#:   if (data == null) return;
来源：http://uj.panjiajie.cn

================================================================================
来源：http://tz.hahajie.cn

C. 函数与作用域
来源：http://nx.lnxyls.cn

================================================================================
来源：http://hg.hnjuh.cn

[C01] 定义函数
来源：http://tj.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://pu.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://im.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://rd.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qc.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ea.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bw.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://vx.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ry.521024.cn

[C02] 默认参数
来源：http://qc.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://gi.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oq.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://gx.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iw.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ny.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vh.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://yh.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://kh.hnjuh.cn

[C03] 可变参数
来源：http://yj.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://tk.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xs.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nm.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ci.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rt.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yf.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://el.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qx.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://ef.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lq.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qx.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bl.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pi.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://bd.521024.cn

Go:   // 无：用配置结构体参数
来源：http://in.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://nj.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://wa.huixiangedu.cn

[C05] 返回多个值
来源：http://jd.gzmigu.cn

Py:   return a, b
来源：http://br.szsharing.cn

PHP:  return [$a, $b];
来源：http://ji.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aq.chemitech.net.cn

TS:   return { a, b };
来源：http://dz.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ga.panjiajie.cn

Go:   return a, b
来源：http://qr.jctech888.com.cn

Ruby: return a, b
来源：http://gy.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://ni.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://yj.nszjky.cn

Py:   square = lambda x: x * x
来源：http://tp.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bu.nicolike.cn

JS:   const square = x => x * x;
来源：http://ow.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://lo.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://to.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ma.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://na.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://em.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://iv.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pa.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://li.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qj.yuexingan06.cn

TS:   arr.map(String)
来源：http://uw.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://or.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lt.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://bp.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xi.hnjuh.cn

[C08] 闭包
来源：http://xp.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pl.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tb.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sh.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xe.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mp.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vv.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://el.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bk.yuexingan06.cn

[C09] 递归
来源：http://kr.wgjwhj.cn


<!-- 参考信息 -->