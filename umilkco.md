代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://vd.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://em.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://cx.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lv.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yp.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://wq.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ax.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://fm.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://jw.newstarts.cn

[A19] 交换两个变量
来源：http://mz.nicolike.cn

Py:   a, b = b, a
来源：http://ap.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://es.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://xu.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://zt.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://be.gzmigu.cn

Go:   a, b = b, a
来源：http://db.shtwfgs.cn

Ruby: a, b = b, a
来源：http://rj.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://rx.panjiajie.cn

[A20] 读取标准输入
来源：http://th.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://my.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ao.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cv.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://bw.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://ar.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tq.bjjhwx.cn

Ruby: gets.chomp
来源：http://eu.gzmigu.cn

C#:   Console.ReadLine();
来源：http://hh.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://ty.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://jr.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xm.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://mi.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://hf.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://eq.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pr.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://ux.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://gb.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://ym.newstarts.cn

Py:   len(s)
来源：http://fs.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aq.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tf.bjjhwx.cn

TS:   s.length
来源：http://id.muxihuayi.cn

Java: s.length()
来源：http://et.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lj.nicolike.cn

Ruby: s.length
来源：http://wl.nicolike.cn

C#:   s.Length
来源：http://mr.szsharing.cn

[A23] 大小写转换
来源：http://ik.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zz.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gb.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://so.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jz.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fr.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ps.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zb.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lc.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://zp.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fk.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://od.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pb.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nn.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qq.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://dx.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yh.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lp.jctech888.com.cn

[A25] 字符串比较
来源：http://na.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://it.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hn.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vk.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gl.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ep.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mo.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vl.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hg.521024.cn

[A26] 类型转换总览
来源：http://gv.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gs.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mi.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bc.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://wv.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://md.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://na.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zf.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pi.huanxung.cn

================================================================================
来源：http://ph.asd995.cn

B. 流程控制
来源：http://sy.huixinmuqiang.cn

================================================================================
来源：http://ud.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://us.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hm.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vp.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rp.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ez.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bx.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ax.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bl.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bu.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://ai.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cw.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://un.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://or.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ir.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yl.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rs.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yk.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.bookmarksfly.cn

[B03] switch / match / case
来源：http://oz.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ah.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nk.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://by.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://te.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nc.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xh.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qo.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bp.yuexingan06.cn

[B04] for 计数循环
来源：http://bn.521024.cn

Py:   for i in range(10): print(i)
来源：http://sp.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pq.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ft.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fb.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://db.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vc.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://dw.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hf.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://mx.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://ff.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oc.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dz.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ip.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xs.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yl.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://bm.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ku.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://dk.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mh.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vo.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ht.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nx.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lx.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kd.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qq.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ve.nicolike.cn

[B07] while 循环
来源：http://pg.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://pi.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pb.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://yr.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://lk.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://so.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kf.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ex.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://lo.colortex.cn

[B08] do-while（至少执行一次）
来源：http://qo.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://tw.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xq.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://tq.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://fv.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://sz.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ql.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hu.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://pq.jianghongdianzi.cn

[B09] break 与 continue
来源：http://qv.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rw.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ki.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ll.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wl.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jy.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nb.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ps.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yr.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://lf.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aq.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dg.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ns.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nr.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gj.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vf.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nu.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ue.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://rv.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://gs.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://ud.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dd.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://by.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bu.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ae.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://hl.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lr.asd995.cn

[B12] 跳出多层循环
来源：http://eq.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nb.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wd.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kv.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fe.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wa.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nr.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hq.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://id.panjiajie.cn

[B13] 判断是否为数字
来源：http://gl.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://yg.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://jw.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kv.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hm.muxihuayi.cn

Java: x instanceof Number
来源：http://bc.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ze.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://mc.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://dz.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://np.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aw.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ab.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://ml.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://qe.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fg.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kk.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ek.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hc.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://rl.521024.cn

Py:   a and b or not c
来源：http://sm.hahajie.cn

PHP:  $a && $b || !$c
来源：http://er.colortex.cn

JS:   a && b || !c
来源：http://hz.nicolike.cn

TS:   a && b || !c
来源：http://cj.huanxung.cn

Java: a && b || !c
来源：http://ks.nicolike.cn

Go:   a && b || !c
来源：http://gz.gzmigu.cn

Ruby: a && b || !c
来源：http://au.szsharing.cn

C#:   a && b || !c
来源：http://uh.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hv.shxzukj.cn

Py:   if not data: return
来源：http://mz.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://dx.shxzskj.cn

JS:   if (!data) return;
来源：http://ek.lnxyls.cn

TS:   if (!data) return;
来源：http://sx.asd995.cn

Java: if (data == null) return;
来源：http://ks.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://ih.newstarts.cn

Ruby: return if data.nil?
来源：http://cg.gzmigu.cn

C#:   if (data == null) return;
来源：http://zz.yuexingan06.cn

================================================================================
来源：http://bl.gzmigu.cn

C. 函数与作用域
来源：http://pb.hnjuh.cn

================================================================================
来源：http://op.chemitech.net.cn

[C01] 定义函数
来源：http://jq.521024.cn

Py:   def add(a, b): return a + b
来源：http://jj.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zj.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://gu.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mj.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kb.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jq.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://qr.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zf.9csxet.cn

[C02] 默认参数
来源：http://up.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://wy.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zv.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://tj.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://px.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oz.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ik.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://sq.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://um.wgjwhj.cn

[C03] 可变参数
来源：http://xx.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://xc.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vt.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zr.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pe.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yp.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hi.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uq.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kd.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://wj.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://op.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sh.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ec.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cc.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://mr.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://ls.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://ba.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://ho.lnxyls.cn

[C05] 返回多个值
来源：http://gj.muxihuayi.cn

Py:   return a, b
来源：http://rv.shxzukj.cn

PHP:  return [$a, $b];
来源：http://fj.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yd.jctech888.com.cn

TS:   return { a, b };
来源：http://uc.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yl.asd995.cn

Go:   return a, b
来源：http://nk.9csxet.cn

Ruby: return a, b
来源：http://cg.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://nc.colortex.cn

[C06] 匿名函数 / lambda
来源：http://sb.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://qd.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tz.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://di.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://df.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lt.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bp.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://gp.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ip.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://gq.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ft.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rs.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bt.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://cm.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gl.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nd.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://qi.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gi.panjiajie.cn

[C08] 闭包
来源：http://ka.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dn.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sj.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sz.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cc.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zu.bjjhwx.cn


<!-- 参考信息 -->