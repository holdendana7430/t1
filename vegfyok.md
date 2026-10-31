代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tm.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xm.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://id.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cn.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mx.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qw.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://us.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://il.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://kq.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://oh.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://rx.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lc.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jg.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://si.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ub.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://va.asd995.cn

C#:   (int)'A'; (char)65
来源：http://br.nszjky.cn

[A19] 交换两个变量
来源：http://yp.yuexingan06.cn

Py:   a, b = b, a
来源：http://jk.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xw.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://nt.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://em.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://qy.yuexingan06.cn

Go:   a, b = b, a
来源：http://oq.nicolike.cn

Ruby: a, b = b, a
来源：http://ma.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://rc.wgjwhj.cn

[A20] 读取标准输入
来源：http://rg.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://wf.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nf.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wx.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://dq.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://ru.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xi.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://wk.521024.cn

C#:   Console.ReadLine();
来源：http://vh.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://ln.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://hr.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://el.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://fv.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://zl.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://nq.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zv.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://qo.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://mx.nicolike.cn

[A22] 获取字符串长度
来源：http://ws.lnxyls.cn

Py:   len(s)
来源：http://gc.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yz.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cx.hahajie.cn

TS:   s.length
来源：http://hz.nicolike.cn

Java: s.length()
来源：http://po.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vx.huixiangedu.cn

Ruby: s.length
来源：http://dp.szsharing.cn

C#:   s.Length
来源：http://tf.huixiangedu.cn

[A23] 大小写转换
来源：http://yn.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tq.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jf.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ax.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hp.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pj.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vx.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hc.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uo.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://fv.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wr.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kh.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zi.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ya.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jg.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://cq.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hq.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sm.wgjwhj.cn

[A25] 字符串比较
来源：http://kp.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://bx.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fz.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gi.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uj.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rw.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qx.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mq.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cv.asd995.cn

[A26] 类型转换总览
来源：http://lh.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hs.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nt.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uy.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://sc.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tv.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pf.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pm.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ox.hahajie.cn

================================================================================
来源：http://zi.chemitech.net.cn

B. 流程控制
来源：http://jx.asd995.cn

================================================================================
来源：http://vd.shxzskj.cn

[B01] 条件判断 if / else
来源：http://ia.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kf.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gj.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ik.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yh.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vg.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fc.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vg.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sv.colortex.cn

[B02] 多分支 else if / elif
来源：http://tr.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wv.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rd.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cq.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zm.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ra.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xf.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://em.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vz.521024.cn

[B03] switch / match / case
来源：http://om.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tq.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://un.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tj.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gy.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ed.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pe.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ip.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ml.jianghongdianzi.cn

[B04] for 计数循环
来源：http://of.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://bz.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tm.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bd.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vr.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pd.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pp.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://vn.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mn.asd995.cn

[B05] 遍历数组 / 列表
来源：http://im.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://qa.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gy.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ci.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gk.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kw.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://up.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://mz.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fv.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://tj.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tw.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xp.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uw.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wf.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://si.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ga.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oo.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hm.nicolike.cn

[B07] while 循环
来源：http://dc.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://pw.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ui.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://ei.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://oq.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://ku.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ml.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://fb.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://vz.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://wy.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://zl.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vg.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://av.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://mo.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://qf.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eh.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://et.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://fl.huixinmuqiang.cn

[B09] break 与 continue
来源：http://el.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jz.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uh.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ks.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ba.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://it.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dy.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rp.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://ma.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bg.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oc.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jw.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ig.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rd.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hf.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hf.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zo.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://jf.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://wl.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://al.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jq.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sd.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fd.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yz.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://jx.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dc.panjiajie.cn

[B12] 跳出多层循环
来源：http://fc.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yh.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ry.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kl.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qs.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gy.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ql.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bh.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pg.shxzskj.cn

[B13] 判断是否为数字
来源：http://mh.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://yq.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://xz.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zw.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tg.huixiangedu.cn

Java: x instanceof Number
来源：http://ii.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zs.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://qf.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://mg.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://ln.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zq.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ab.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://zb.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://rd.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://er.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zx.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fb.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rv.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://fu.panjiajie.cn

Py:   a and b or not c
来源：http://ma.nicolike.cn

PHP:  $a && $b || !$c
来源：http://lm.nicolike.cn

JS:   a && b || !c
来源：http://il.huanxung.cn

TS:   a && b || !c
来源：http://ft.521024.cn

Java: a && b || !c
来源：http://xz.newstarts.cn

Go:   a && b || !c
来源：http://or.9csxet.cn

Ruby: a && b || !c
来源：http://jt.muxihuayi.cn

C#:   a && b || !c
来源：http://pd.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://os.muxihuayi.cn

Py:   if not data: return
来源：http://ge.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://ff.asd995.cn

JS:   if (!data) return;
来源：http://ec.newstarts.cn

TS:   if (!data) return;
来源：http://rc.gzmigu.cn

Java: if (data == null) return;
来源：http://oz.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://ft.shxzukj.cn

Ruby: return if data.nil?
来源：http://qn.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://hv.huixiangedu.cn

================================================================================
来源：http://tw.hahajie.cn

C. 函数与作用域
来源：http://in.nszjky.cn

================================================================================
来源：http://re.bookmarksfly.cn

[C01] 定义函数
来源：http://lw.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://vt.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nw.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://vn.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iz.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pa.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mz.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://oy.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hs.521024.cn

[C02] 默认参数
来源：http://hm.521024.cn

Py:   def greet(name="World"): return name
来源：http://ba.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zc.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://zv.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xw.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hm.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ef.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ur.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://io.bookmarksfly.cn

[C03] 可变参数
来源：http://wo.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://cg.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bt.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sk.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ri.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jz.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mq.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mx.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pf.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://dg.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ij.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dk.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://da.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sn.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://bx.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://cq.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://kg.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://cy.9csxet.cn

[C05] 返回多个值
来源：http://db.jianghongdianzi.cn

Py:   return a, b
来源：http://mk.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://ha.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ke.newstarts.cn

TS:   return { a, b };
来源：http://vl.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://og.chemitech.net.cn

Go:   return a, b
来源：http://bm.yuntaijiaju.cn

Ruby: return a, b
来源：http://ob.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://zw.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://vm.nicolike.cn

Py:   square = lambda x: x * x
来源：http://jj.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tz.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://gk.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://tv.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ok.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kj.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://qx.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://li.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://nh.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wk.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vi.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zl.521024.cn

TS:   arr.map(String)
来源：http://tm.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oz.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ur.jctech888.com.cn


<!-- 参考信息 -->