代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mr.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qh.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zj.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://op.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://af.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://vo.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://mq.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ld.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hy.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://am.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://av.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://jh.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://dt.wgjwhj.cn

[A19] 交换两个变量
来源：http://cl.newstarts.cn

Py:   a, b = b, a
来源：http://hm.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kg.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://zp.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://fc.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://dz.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://ut.521024.cn

Ruby: a, b = b, a
来源：http://uk.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://st.bookmarksfly.cn

[A20] 读取标准输入
来源：http://rn.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://sb.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yi.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ci.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://ut.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://jd.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eo.szsharing.cn

Ruby: gets.chomp
来源：http://cl.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://xe.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://zh.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://hw.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gu.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://do.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://se.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://eu.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qi.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://pa.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://fa.nszjky.cn

[A22] 获取字符串长度
来源：http://ak.shtwfgs.cn

Py:   len(s)
来源：http://xh.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nf.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cz.huixiangedu.cn

TS:   s.length
来源：http://qw.szxytkj.cn

Java: s.length()
来源：http://ll.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dn.bookmarksfly.cn

Ruby: s.length
来源：http://lx.bjjhwx.cn

C#:   s.Length
来源：http://qh.shtwfgs.cn

[A23] 大小写转换
来源：http://ba.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xw.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rx.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wm.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://of.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zg.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ut.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dj.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://db.haigaiapp.cn

[A24] 去除首尾空白
来源：http://mw.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zn.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xg.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cf.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yk.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kx.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://sp.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kl.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jn.chemitech.net.cn

[A25] 字符串比较
来源：http://id.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://dr.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hb.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jj.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cu.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jw.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ew.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fv.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qv.shxzskj.cn

[A26] 类型转换总览
来源：http://pt.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wg.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wm.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uh.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://gr.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gj.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kl.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mn.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mu.jianghongdianzi.cn

================================================================================
来源：http://le.asd995.cn

B. 流程控制
来源：http://zi.521024.cn

================================================================================
来源：http://bt.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://mj.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nn.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wm.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ol.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ah.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ao.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ez.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sx.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://br.asd995.cn

[B02] 多分支 else if / elif
来源：http://iq.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://li.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mo.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vc.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zm.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ql.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cp.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qk.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yb.jctech888.com.cn

[B03] switch / match / case
来源：http://eh.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ea.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uj.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eb.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oh.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kd.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dd.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jc.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gx.jctech888.com.cn

[B04] for 计数循环
来源：http://iu.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://jz.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uc.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qd.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kh.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ni.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bx.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://rr.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qm.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://or.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://ev.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oj.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oi.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rj.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pm.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hf.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://qx.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xs.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://xw.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qg.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nl.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://om.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cs.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vt.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sx.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lw.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cz.hahajie.cn

[B07] while 循环
来源：http://si.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://xp.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wn.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://fc.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://sy.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://tj.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://un.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://hi.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://bm.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://wo.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://dn.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ey.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://cr.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://tm.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://ry.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://om.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vt.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://js.9csxet.cn

[B09] break 与 continue
来源：http://mh.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dp.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mw.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xi.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pp.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ba.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pn.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xi.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://gy.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rj.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ps.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://km.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xw.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hq.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yb.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fj.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://po.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://tq.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://gb.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://sh.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wn.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nx.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://js.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qk.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://qn.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://am.nszjky.cn

[B12] 跳出多层循环
来源：http://ab.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://co.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qg.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tn.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dr.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yj.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://na.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lp.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hx.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://vd.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://er.hahajie.cn

PHP:  is_numeric($x)
来源：http://gk.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://im.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rq.wgjwhj.cn

Java: x instanceof Number
来源：http://lh.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fe.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://oc.shxzukj.cn

C#:   x is int or double or decimal
来源：http://cm.521024.cn

[B14] 判断值是否在集合内
来源：http://dr.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ra.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fu.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://dg.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://vn.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rw.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rv.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zx.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rz.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://cz.huanxung.cn

Py:   a and b or not c
来源：http://tw.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://bm.haigaiapp.cn

JS:   a && b || !c
来源：http://ob.shxzskj.cn

TS:   a && b || !c
来源：http://fd.shxzskj.cn

Java: a && b || !c
来源：http://si.hahajie.cn

Go:   a && b || !c
来源：http://ah.nicolike.cn

Ruby: a && b || !c
来源：http://td.panjiajie.cn

C#:   a && b || !c
来源：http://ic.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sd.muxihuayi.cn

Py:   if not data: return
来源：http://el.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://zs.newstarts.cn

JS:   if (!data) return;
来源：http://md.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://hc.wgjwhj.cn

Java: if (data == null) return;
来源：http://ip.yuexingan06.cn

Go:   if data == nil { return }
来源：http://oo.9csxet.cn

Ruby: return if data.nil?
来源：http://qn.bjjhwx.cn

C#:   if (data == null) return;
来源：http://pp.huixinmuqiang.cn

================================================================================
来源：http://qa.haigaiapp.cn

C. 函数与作用域
来源：http://dv.haigaiapp.cn

================================================================================
来源：http://ka.huixinmuqiang.cn

[C01] 定义函数
来源：http://ez.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://eq.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pz.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://vr.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ms.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mr.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ao.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://po.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sp.wgjwhj.cn

[C02] 默认参数
来源：http://sb.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://dc.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bz.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://fx.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ep.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://it.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iy.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://wu.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://bn.panjiajie.cn

[C03] 可变参数
来源：http://ie.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ck.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bg.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iy.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gb.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bb.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ae.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yh.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fw.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://sw.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qy.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://or.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wl.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pc.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ow.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://ov.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://ti.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://az.szxytkj.cn

[C05] 返回多个值
来源：http://ag.9csxet.cn

Py:   return a, b
来源：http://us.521024.cn

PHP:  return [$a, $b];
来源：http://ut.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yj.bookmarksfly.cn

TS:   return { a, b };
来源：http://mb.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bf.bjjhwx.cn

Go:   return a, b
来源：http://ok.yuntaijiaju.cn

Ruby: return a, b
来源：http://wv.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://en.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://rf.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://sl.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kf.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://md.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://vl.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oz.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qr.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://ec.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://th.521024.cn

[C07] 把函数作为参数传入
来源：http://io.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yo.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lz.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dl.chemitech.net.cn

TS:   arr.map(String)
来源：http://dg.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gf.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pj.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://xa.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ng.yuntaijiaju.cn

[C08] 闭包
来源：http://pb.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ik.521024.cn


<!-- 参考信息 -->