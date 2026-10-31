代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oq.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kn.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fu.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gp.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mq.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sg.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://en.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ej.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://ia.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://lm.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://zx.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xu.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://or.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://nt.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jp.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://go.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://ff.asd995.cn

[A19] 交换两个变量
来源：http://fc.9csxet.cn

Py:   a, b = b, a
来源：http://oq.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://py.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://nt.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://yh.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://iv.nicolike.cn

Go:   a, b = b, a
来源：http://fr.hahajie.cn

Ruby: a, b = b, a
来源：http://id.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://kv.wgjwhj.cn

[A20] 读取标准输入
来源：http://sx.asd995.cn

Py:   name = input("请输入：")
来源：http://bv.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lf.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cc.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://kd.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://ii.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zw.9csxet.cn

Ruby: gets.chomp
来源：http://vs.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://es.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://bc.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://nr.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vg.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://wk.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://wd.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://vt.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lj.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://xu.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://ol.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://px.shtwfgs.cn

Py:   len(s)
来源：http://pa.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uw.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ml.shxzukj.cn

TS:   s.length
来源：http://ek.yuexingan06.cn

Java: s.length()
来源：http://ns.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kc.huanxung.cn

Ruby: s.length
来源：http://nu.yuntaijiaju.cn

C#:   s.Length
来源：http://wn.nszjky.cn

[A23] 大小写转换
来源：http://mt.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://at.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ct.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ky.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ql.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qi.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rp.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ei.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mo.shtwfgs.cn

[A24] 去除首尾空白
来源：http://ra.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://na.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oj.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yn.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kd.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cu.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://if.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ci.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sk.gzmigu.cn

[A25] 字符串比较
来源：http://kh.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://pk.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://em.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pf.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dm.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kx.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kv.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yr.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gv.lnxyls.cn

[A26] 类型转换总览
来源：http://ju.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cm.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ja.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jy.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://na.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rj.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ty.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yj.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wy.muxihuayi.cn

================================================================================
来源：http://me.shxzukj.cn

B. 流程控制
来源：http://nf.huixinmuqiang.cn

================================================================================
来源：http://rq.nicolike.cn

[B01] 条件判断 if / else
来源：http://kz.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gc.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://on.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hq.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bd.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pn.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wc.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ih.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zf.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://lm.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wm.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pk.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ib.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fy.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cw.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qs.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fy.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qt.gzmigu.cn

[B03] switch / match / case
来源：http://yf.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hl.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xm.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ub.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://el.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fp.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pt.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://go.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qj.yuexingan06.cn

[B04] for 计数循环
来源：http://nh.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://jt.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bg.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rv.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bz.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hw.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ik.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://fh.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ak.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://ko.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://sg.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qt.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://er.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://br.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://em.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sq.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://ya.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fr.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://zc.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pp.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ao.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://je.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wj.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cc.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yc.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fv.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xd.shtwfgs.cn

[B07] while 循环
来源：http://lg.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://gx.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mp.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://kt.521024.cn

TS:   while (i < 10) { i++; }
来源：http://xb.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://fl.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fn.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://su.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://vf.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://vr.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://qq.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xb.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://sp.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://nf.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://rg.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ga.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qa.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://yn.shtwfgs.cn

[B09] break 与 continue
来源：http://mk.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nf.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hd.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ir.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oq.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://io.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://en.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ka.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qq.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://xv.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gh.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yt.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fx.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iz.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xs.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xu.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sm.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hc.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://jq.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://ed.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://kj.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bf.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xo.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yw.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yl.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://os.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://md.lnxyls.cn

[B12] 跳出多层循环
来源：http://xf.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ea.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wu.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xl.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cy.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uz.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oc.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ub.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yw.muxihuayi.cn

[B13] 判断是否为数字
来源：http://zy.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://am.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://km.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ld.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qf.colortex.cn

Java: x instanceof Number
来源：http://lv.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pq.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://rz.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://ad.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://wf.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://su.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xf.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://av.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://yc.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kk.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qx.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ig.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hr.shxzskj.cn

[B15] 布尔运算与取反
来源：http://up.521024.cn

Py:   a and b or not c
来源：http://bx.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://bm.jctech888.com.cn

JS:   a && b || !c
来源：http://zd.hahajie.cn

TS:   a && b || !c
来源：http://qo.nicolike.cn

Java: a && b || !c
来源：http://qz.jianghongdianzi.cn

Go:   a && b || !c
来源：http://uj.nszjky.cn

Ruby: a && b || !c
来源：http://ao.yuntaijiaju.cn

C#:   a && b || !c
来源：http://ag.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zo.szsharing.cn

Py:   if not data: return
来源：http://tl.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://bv.hnjuh.cn

JS:   if (!data) return;
来源：http://ck.wgjwhj.cn

TS:   if (!data) return;
来源：http://aj.yuexingan06.cn

Java: if (data == null) return;
来源：http://kr.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://ra.lnxyls.cn

Ruby: return if data.nil?
来源：http://nc.shxzukj.cn

C#:   if (data == null) return;
来源：http://gb.nicolike.cn

================================================================================
来源：http://yb.jianghongdianzi.cn

C. 函数与作用域
来源：http://iv.nicolike.cn

================================================================================
来源：http://fj.newstarts.cn

[C01] 定义函数
来源：http://mh.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://ou.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hq.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://xp.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nb.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eo.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dh.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://mt.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ro.shxzskj.cn

[C02] 默认参数
来源：http://pu.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://dl.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lm.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://ez.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wp.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fi.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qm.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://kf.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://qj.9csxet.cn

[C03] 可变参数
来源：http://ju.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://uk.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hq.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gt.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hj.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wn.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yd.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jw.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qe.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://to.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ve.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rb.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kp.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ex.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://qj.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://wu.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://mo.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://gi.hahajie.cn

[C05] 返回多个值
来源：http://ut.huixinmuqiang.cn

Py:   return a, b
来源：http://ma.colortex.cn

PHP:  return [$a, $b];
来源：http://fq.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mi.panjiajie.cn

TS:   return { a, b };
来源：http://ly.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ay.haigaiapp.cn

Go:   return a, b
来源：http://pt.lnxyls.cn

Ruby: return a, b
来源：http://zd.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://tb.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://yh.9csxet.cn

Py:   square = lambda x: x * x
来源：http://oz.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ej.lnxyls.cn

JS:   const square = x => x * x;
来源：http://lp.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://oc.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eh.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sv.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://la.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bo.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://pn.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wd.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pk.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xq.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://oe.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ki.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ep.huixiangedu.cn


<!-- 参考信息 -->