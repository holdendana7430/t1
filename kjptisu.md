代发 wailian999

C#:   (int)'A'; (char)65
来源：http://dr.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://al.shxzukj.cn

Py:   a, b = b, a
来源：http://rb.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uh.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://yy.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://gv.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://tk.shxzskj.cn

Go:   a, b = b, a
来源：http://gz.haigaiapp.cn

Ruby: a, b = b, a
来源：http://sn.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://ji.bjjhwx.cn

[A20] 读取标准输入
来源：http://js.gzmigu.cn

Py:   name = input("请输入：")
来源：http://yd.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://no.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tv.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://kk.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://sa.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uw.colortex.cn

Ruby: gets.chomp
来源：http://ik.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://ez.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://fk.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://ii.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wk.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://wv.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://sr.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://by.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bq.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://xz.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://vp.9csxet.cn

[A22] 获取字符串长度
来源：http://dw.huixiangedu.cn

Py:   len(s)
来源：http://dz.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rf.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uq.shxzskj.cn

TS:   s.length
来源：http://zu.shxzskj.cn

Java: s.length()
来源：http://qz.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://em.szxytkj.cn

Ruby: s.length
来源：http://nd.yuexingan06.cn

C#:   s.Length
来源：http://bf.szsharing.cn

[A23] 大小写转换
来源：http://hw.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sk.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nn.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tp.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://te.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hf.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gr.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zh.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dz.jctech888.com.cn

[A24] 去除首尾空白
来源：http://xw.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wt.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fb.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xe.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jn.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ai.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://cn.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ni.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qk.huixiangedu.cn

[A25] 字符串比较
来源：http://hf.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://cw.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kq.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://el.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wr.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ch.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mj.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qp.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tp.szsharing.cn

[A26] 类型转换总览
来源：http://gf.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nx.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zt.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uj.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://wk.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hs.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fs.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wf.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hd.newstarts.cn

================================================================================
来源：http://qa.shtwfgs.cn

B. 流程控制
来源：http://el.lnxyls.cn

================================================================================
来源：http://iy.hahajie.cn

[B01] 条件判断 if / else
来源：http://yf.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lx.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zi.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fe.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xw.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ba.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wy.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dc.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hb.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://yr.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iq.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xv.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uw.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wx.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sw.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ib.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fj.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yh.colortex.cn

[B03] switch / match / case
来源：http://ci.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ws.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kv.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dz.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vi.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lg.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ti.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tq.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ar.lnxyls.cn

[B04] for 计数循环
来源：http://kk.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://wb.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yh.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ro.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pd.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mo.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kb.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://ku.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ch.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://it.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://uc.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mr.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oz.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iw.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ye.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ep.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://zy.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mx.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://dl.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sm.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ow.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xw.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hv.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pf.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://of.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zz.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sm.nszjky.cn

[B07] while 循环
来源：http://jf.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://zz.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vq.521024.cn

JS:   while (i < 10) { i++; }
来源：http://gf.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://qb.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://ix.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ju.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ig.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://kk.521024.cn

[B08] do-while（至少执行一次）
来源：http://hw.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://bg.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vj.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://za.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://es.521024.cn

Java: do { i++; } while (i < 10);
来源：http://fv.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sk.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gr.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://ik.bjjhwx.cn

[B09] break 与 continue
来源：http://xd.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rc.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kh.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://we.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://op.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oc.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xq.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zf.szsharing.cn

[B10] 遍历同时拿索引
来源：http://aw.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uc.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wo.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yv.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zt.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rn.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ga.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pd.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wy.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://al.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://cy.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://lc.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kn.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vy.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://su.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pm.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://mk.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hb.szxytkj.cn

[B12] 跳出多层循环
来源：http://rv.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zf.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qk.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yz.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nj.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://su.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hf.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vd.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lp.wgjwhj.cn

[B13] 判断是否为数字
来源：http://nf.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://ld.lnxyls.cn

PHP:  is_numeric($x)
来源：http://fr.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cb.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fo.jianghongdianzi.cn

Java: x instanceof Number
来源：http://bc.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fg.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://ft.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://jt.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://qk.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hu.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ep.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://oj.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://wq.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oc.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://af.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ek.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fl.szxytkj.cn

[B15] 布尔运算与取反
来源：http://hu.yuexingan06.cn

Py:   a and b or not c
来源：http://va.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://hd.panjiajie.cn

JS:   a && b || !c
来源：http://yr.huanxung.cn

TS:   a && b || !c
来源：http://di.bookmarksfly.cn

Java: a && b || !c
来源：http://fn.chemitech.net.cn

Go:   a && b || !c
来源：http://ck.gzmigu.cn

Ruby: a && b || !c
来源：http://su.nszjky.cn

C#:   a && b || !c
来源：http://ut.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uk.wgjwhj.cn

Py:   if not data: return
来源：http://wx.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://ye.shxzukj.cn

JS:   if (!data) return;
来源：http://ia.shtwfgs.cn

TS:   if (!data) return;
来源：http://wq.chemitech.net.cn

Java: if (data == null) return;
来源：http://jk.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://ze.newstarts.cn

Ruby: return if data.nil?
来源：http://xl.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://yi.yuexingan06.cn

================================================================================
来源：http://yx.hnjuh.cn

C. 函数与作用域
来源：http://qp.shxzskj.cn

================================================================================
来源：http://ck.nicolike.cn

[C01] 定义函数
来源：http://eu.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://vf.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ya.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://wt.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tx.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lw.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zg.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://uz.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nu.521024.cn

[C02] 默认参数
来源：http://wo.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://nv.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cz.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://ng.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uh.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tu.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qi.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ln.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://vr.haigaiapp.cn

[C03] 可变参数
来源：http://yy.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://kd.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://in.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qw.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://si.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vz.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fg.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yh.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ml.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://ld.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://li.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bx.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://so.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aq.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://nr.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://eh.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://sg.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://pm.asd995.cn

[C05] 返回多个值
来源：http://hg.yuntaijiaju.cn

Py:   return a, b
来源：http://nr.colortex.cn

PHP:  return [$a, $b];
来源：http://gz.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ne.shtwfgs.cn

TS:   return { a, b };
来源：http://im.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bp.bookmarksfly.cn

Go:   return a, b
来源：http://tp.nicolike.cn

Ruby: return a, b
来源：http://ih.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://yj.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://wt.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://vt.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://in.newstarts.cn

JS:   const square = x => x * x;
来源：http://fx.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://oh.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rq.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gz.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://py.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ss.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://ub.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tp.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sg.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bo.szxytkj.cn

TS:   arr.map(String)
来源：http://ry.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://je.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wn.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://zx.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wo.wgjwhj.cn

[C08] 闭包
来源：http://tk.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lz.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cg.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rs.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qm.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ek.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vc.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ye.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vb.jianghongdianzi.cn

[C09] 递归
来源：http://ho.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ex.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aq.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vv.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yo.nicolike.cn


<!-- 参考信息 -->