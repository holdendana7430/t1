代发 wailian999

C#:   (int)'A'; (char)65
来源：http://yv.9csxet.cn

[A19] 交换两个变量
来源：http://el.shxzukj.cn

Py:   a, b = b, a
来源：http://ys.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tn.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://wg.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://ug.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://uw.nicolike.cn

Go:   a, b = b, a
来源：http://sc.shxzukj.cn

Ruby: a, b = b, a
来源：http://di.asd995.cn

C#:   (a, b) = (b, a);
来源：http://vk.asd995.cn

[A20] 读取标准输入
来源：http://gw.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://yq.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zg.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ov.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://ct.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://dr.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vd.haigaiapp.cn

Ruby: gets.chomp
来源：http://gm.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://qc.521024.cn

[A21] 保留指定小数位输出
来源：http://bh.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://ne.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jk.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://lz.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://jr.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://fp.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ct.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://sn.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://qi.nszjky.cn

[A22] 获取字符串长度
来源：http://la.chemitech.net.cn

Py:   len(s)
来源：http://al.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eh.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hr.shxzskj.cn

TS:   s.length
来源：http://jj.wgjwhj.cn

Java: s.length()
来源：http://as.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hn.haigaiapp.cn

Ruby: s.length
来源：http://ef.hahajie.cn

C#:   s.Length
来源：http://gc.hahajie.cn

[A23] 大小写转换
来源：http://po.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://te.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yj.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xn.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lc.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gq.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bq.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cv.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cq.hnjuh.cn

[A24] 去除首尾空白
来源：http://de.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fw.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://io.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://em.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qm.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xu.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://op.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eq.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://en.bookmarksfly.cn

[A25] 字符串比较
来源：http://bl.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://gq.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vh.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://do.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ns.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wu.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://op.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pj.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hq.9csxet.cn

[A26] 类型转换总览
来源：http://bp.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yi.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hg.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cj.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://kj.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lx.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zh.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rr.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nm.bjjhwx.cn

================================================================================
来源：http://nd.jctech888.com.cn

B. 流程控制
来源：http://rr.asd995.cn

================================================================================
来源：http://ns.9csxet.cn

[B01] 条件判断 if / else
来源：http://hm.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hf.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ic.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ur.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ou.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qo.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gh.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gm.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aj.hahajie.cn

[B02] 多分支 else if / elif
来源：http://ex.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nq.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lf.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://la.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pm.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oq.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jv.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ru.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.huixinmuqiang.cn

[B03] switch / match / case
来源：http://ur.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lv.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ad.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ia.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ya.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lv.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://di.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lt.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ow.panjiajie.cn

[B04] for 计数循环
来源：http://bz.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://io.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kw.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yl.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ul.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fn.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yn.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://mq.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ex.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://gc.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://tr.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wy.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zh.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gh.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hp.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kd.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://bh.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ts.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://wm.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fj.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xw.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://od.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nm.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ki.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://av.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ll.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ex.newstarts.cn

[B07] while 循环
来源：http://yn.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://sj.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wo.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://dd.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://lp.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://fr.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jn.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://gw.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://rz.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://je.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://rc.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gn.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://sa.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://xr.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://zf.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tj.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wg.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://oq.newstarts.cn

[B09] break 与 continue
来源：http://ra.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vx.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jq.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hk.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://un.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zg.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xq.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bs.9csxet.cn

[B10] 遍历同时拿索引
来源：http://tn.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nd.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wc.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fk.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tv.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://go.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://la.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wd.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rf.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://tx.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://tg.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://op.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ka.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://py.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kb.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mi.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://gt.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qs.nszjky.cn

[B12] 跳出多层循环
来源：http://oc.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vg.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pt.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vg.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rw.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cm.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dj.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qz.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kt.shtwfgs.cn

[B13] 判断是否为数字
来源：http://zn.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://rf.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://ev.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dx.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hi.9csxet.cn

Java: x instanceof Number
来源：http://od.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fp.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://wd.szxytkj.cn

C#:   x is int or double or decimal
来源：http://ez.hahajie.cn

[B14] 判断值是否在集合内
来源：http://dh.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tq.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ll.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://oz.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://sz.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qd.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cp.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cc.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nk.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://ww.haigaiapp.cn

Py:   a and b or not c
来源：http://vs.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://ue.haigaiapp.cn

JS:   a && b || !c
来源：http://wn.shxzukj.cn

TS:   a && b || !c
来源：http://tp.szxytkj.cn

Java: a && b || !c
来源：http://sc.nszjky.cn

Go:   a && b || !c
来源：http://kf.bjjhwx.cn

Ruby: a && b || !c
来源：http://ma.9csxet.cn

C#:   a && b || !c
来源：http://xc.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oq.szxytkj.cn

Py:   if not data: return
来源：http://vf.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://bn.colortex.cn

JS:   if (!data) return;
来源：http://wg.haigaiapp.cn

TS:   if (!data) return;
来源：http://ba.haigaiapp.cn

Java: if (data == null) return;
来源：http://uy.9csxet.cn

Go:   if data == nil { return }
来源：http://yf.szsharing.cn

Ruby: return if data.nil?
来源：http://ek.gzmigu.cn

C#:   if (data == null) return;
来源：http://an.nszjky.cn

================================================================================
来源：http://oy.muxihuayi.cn

C. 函数与作用域
来源：http://fy.jianghongdianzi.cn

================================================================================
来源：http://dc.shxzukj.cn

[C01] 定义函数
来源：http://rp.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://dq.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wq.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://to.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fr.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cj.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mj.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://xv.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uq.9csxet.cn

[C02] 默认参数
来源：http://fc.521024.cn

Py:   def greet(name="World"): return name
来源：http://iy.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hu.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://in.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yw.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kk.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ee.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://zi.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://qc.jianghongdianzi.cn

[C03] 可变参数
来源：http://du.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://dd.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hy.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ha.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nx.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vc.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bc.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tb.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xz.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://nf.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bb.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vi.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xd.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bf.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://lv.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://tb.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://ze.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://je.shtwfgs.cn

[C05] 返回多个值
来源：http://zd.wgjwhj.cn

Py:   return a, b
来源：http://uo.colortex.cn

PHP:  return [$a, $b];
来源：http://ur.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xj.lnxyls.cn

TS:   return { a, b };
来源：http://uc.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xt.huixinmuqiang.cn

Go:   return a, b
来源：http://ja.bjjhwx.cn

Ruby: return a, b
来源：http://zr.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://ld.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://wy.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://th.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://al.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://no.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://kf.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xb.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wh.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://ul.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xx.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://ge.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oc.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://be.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rf.shxzukj.cn

TS:   arr.map(String)
来源：http://df.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ma.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qv.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://rk.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rx.nszjky.cn

[C08] 闭包
来源：http://uc.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nn.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://um.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://es.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oo.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dy.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ho.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kq.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wz.521024.cn

[C09] 递归
来源：http://ux.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dq.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fu.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hj.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wt.hnjuh.cn


<!-- 参考信息 -->