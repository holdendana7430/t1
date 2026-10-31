代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uk.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cs.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sr.huixinmuqiang.cn

[A17] 位运算
来源：http://dr.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gi.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://aq.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qd.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dl.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vm.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lm.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ax.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zu.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://jg.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://bz.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://gw.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xz.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uo.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://qk.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://an.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://xl.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://bg.521024.cn

[A19] 交换两个变量
来源：http://qa.colortex.cn

Py:   a, b = b, a
来源：http://qi.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wt.colortex.cn

JS:   [a, b] = [b, a];
来源：http://kx.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://ke.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://oz.lnxyls.cn

Go:   a, b = b, a
来源：http://az.hnjuh.cn

Ruby: a, b = b, a
来源：http://cc.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://na.muxihuayi.cn

[A20] 读取标准输入
来源：http://fv.9csxet.cn

Py:   name = input("请输入：")
来源：http://iu.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mz.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xn.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://pi.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://vb.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fv.muxihuayi.cn

Ruby: gets.chomp
来源：http://lq.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://dt.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://jt.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://di.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gr.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://ge.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://zi.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://zl.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xj.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://mb.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://ki.nicolike.cn

[A22] 获取字符串长度
来源：http://yx.hahajie.cn

Py:   len(s)
来源：http://go.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ns.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ng.muxihuayi.cn

TS:   s.length
来源：http://sq.hahajie.cn

Java: s.length()
来源：http://fi.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yj.asd995.cn

Ruby: s.length
来源：http://hz.huixiangedu.cn

C#:   s.Length
来源：http://vf.panjiajie.cn

[A23] 大小写转换
来源：http://nq.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://na.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bj.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jd.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uw.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cc.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nj.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ri.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bx.huixiangedu.cn

[A24] 去除首尾空白
来源：http://ti.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wk.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://te.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wy.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fj.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jv.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://bo.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xf.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ti.9csxet.cn

[A25] 字符串比较
来源：http://dy.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://wo.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pm.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bj.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xv.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vh.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xl.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ix.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dx.lnxyls.cn

[A26] 类型转换总览
来源：http://bz.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zn.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zw.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iu.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://ns.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lg.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://px.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://at.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rx.muxihuayi.cn

================================================================================
来源：http://un.521024.cn

B. 流程控制
来源：http://wa.shxzukj.cn

================================================================================
来源：http://ng.lnxyls.cn

[B01] 条件判断 if / else
来源：http://rc.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hy.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vy.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cm.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mj.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://et.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://to.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://we.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oi.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://gr.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://em.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://st.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sm.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dy.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hv.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fl.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://az.9csxet.cn

[B03] switch / match / case
来源：http://fv.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hs.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oi.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nd.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mv.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kf.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gf.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ga.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kl.huixiangedu.cn

[B04] for 计数循环
来源：http://nt.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://mz.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ap.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vf.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ty.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ke.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://de.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://cz.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zx.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://yh.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://nw.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ye.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dm.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wf.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ni.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zz.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://de.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tk.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://dg.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ww.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tp.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mv.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ny.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://de.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ep.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://or.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ao.chemitech.net.cn

[B07] while 循环
来源：http://vk.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://sd.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yb.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://ty.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://oa.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://un.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kw.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://qu.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://zi.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://lc.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://fv.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://br.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://hm.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://sv.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://oj.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ox.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qh.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://si.szsharing.cn

[B09] break 与 continue
来源：http://tb.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sq.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ny.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ev.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yq.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bc.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ya.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fo.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sh.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://rn.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dm.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kw.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jm.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nf.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nf.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jy.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bi.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ke.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://sj.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://yj.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://vm.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rq.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nj.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rr.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jy.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://vm.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zo.jctech888.com.cn

[B12] 跳出多层循环
来源：http://dj.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://af.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lo.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ah.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ym.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ej.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cd.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hk.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://by.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://td.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://xe.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://bm.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cc.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mk.chemitech.net.cn

Java: x instanceof Number
来源：http://og.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ll.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://yy.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://qe.nszjky.cn

[B14] 判断值是否在集合内
来源：http://lk.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dl.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lt.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://xg.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://xt.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cd.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xy.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pf.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ka.gzmigu.cn

[B15] 布尔运算与取反
来源：http://gm.lnxyls.cn

Py:   a and b or not c
来源：http://kr.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://eh.asd995.cn

JS:   a && b || !c
来源：http://oh.muxihuayi.cn

TS:   a && b || !c
来源：http://nl.9csxet.cn

Java: a && b || !c
来源：http://km.szsharing.cn

Go:   a && b || !c
来源：http://ig.asd995.cn

Ruby: a && b || !c
来源：http://gm.jianghongdianzi.cn

C#:   a && b || !c
来源：http://kg.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uc.huanxung.cn

Py:   if not data: return
来源：http://nm.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://pe.muxihuayi.cn

JS:   if (!data) return;
来源：http://bz.yuexingan06.cn

TS:   if (!data) return;
来源：http://qv.huanxung.cn

Java: if (data == null) return;
来源：http://xw.szsharing.cn

Go:   if data == nil { return }
来源：http://ig.wgjwhj.cn

Ruby: return if data.nil?
来源：http://se.nicolike.cn

C#:   if (data == null) return;
来源：http://xu.chemitech.net.cn

================================================================================
来源：http://ht.panjiajie.cn

C. 函数与作用域
来源：http://wc.huixiangedu.cn

================================================================================
来源：http://jz.nicolike.cn

[C01] 定义函数
来源：http://ao.colortex.cn

Py:   def add(a, b): return a + b
来源：http://re.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tc.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://mz.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eh.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mt.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rp.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://uf.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ey.jianghongdianzi.cn

[C02] 默认参数
来源：http://wd.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://um.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://en.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ee.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mi.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gc.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bl.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://mv.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://iy.huanxung.cn

[C03] 可变参数
来源：http://rm.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://id.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jn.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gw.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://et.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pw.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pg.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oj.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ct.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://hh.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ct.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pm.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zr.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lk.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://lf.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://eb.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://fo.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://ig.huixiangedu.cn

[C05] 返回多个值
来源：http://rh.panjiajie.cn

Py:   return a, b
来源：http://zt.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://qk.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ax.shxzukj.cn

TS:   return { a, b };
来源：http://kz.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tw.yuntaijiaju.cn

Go:   return a, b
来源：http://uk.shxzskj.cn

Ruby: return a, b
来源：http://lk.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ao.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://ay.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://gq.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cs.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://sv.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://dl.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dl.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iz.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://xn.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wr.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://fu.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xw.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mv.chemitech.net.cn


<!-- 参考信息 -->