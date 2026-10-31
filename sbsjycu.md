代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dy.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xv.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eo.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lf.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gg.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ke.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yf.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hq.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://mj.asd995.cn

Py:   ord("A"); chr(65)
来源：http://ap.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://sw.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gp.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jv.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://ym.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ha.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://ma.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://jd.muxihuayi.cn

[A19] 交换两个变量
来源：http://qg.haigaiapp.cn

Py:   a, b = b, a
来源：http://qf.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bk.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://gh.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://ap.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://gy.shxzskj.cn

Go:   a, b = b, a
来源：http://eh.newstarts.cn

Ruby: a, b = b, a
来源：http://ta.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://xg.chemitech.net.cn

[A20] 读取标准输入
来源：http://qb.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://ei.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zj.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cp.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://fx.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://tv.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ym.nszjky.cn

Ruby: gets.chomp
来源：http://ld.gzmigu.cn

C#:   Console.ReadLine();
来源：http://tn.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://eb.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://wk.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oy.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://az.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://ev.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://qf.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://li.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://do.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://fg.shtwfgs.cn

[A22] 获取字符串长度
来源：http://ec.huixinmuqiang.cn

Py:   len(s)
来源：http://wr.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mr.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://et.9csxet.cn

TS:   s.length
来源：http://am.yuntaijiaju.cn

Java: s.length()
来源：http://hj.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bs.asd995.cn

Ruby: s.length
来源：http://sh.hnjuh.cn

C#:   s.Length
来源：http://ds.yuntaijiaju.cn

[A23] 大小写转换
来源：http://bi.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gn.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gz.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cx.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ev.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lm.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tu.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uj.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cu.yuexingan06.cn

[A24] 去除首尾空白
来源：http://lr.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uz.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vi.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ss.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ij.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fb.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://tv.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ge.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xg.lnxyls.cn

[A25] 字符串比较
来源：http://fp.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://ay.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ky.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gs.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bb.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ow.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ha.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jh.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hr.asd995.cn

[A26] 类型转换总览
来源：http://an.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ks.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wy.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ma.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://vq.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sv.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zm.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ur.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sb.szxytkj.cn

================================================================================
来源：http://is.huixinmuqiang.cn

B. 流程控制
来源：http://lg.jctech888.com.cn

================================================================================
来源：http://lw.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://sa.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bb.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://om.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hy.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zy.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rd.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://um.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cr.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rz.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://vc.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cz.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gw.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gz.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dr.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://im.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gr.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pf.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xz.bookmarksfly.cn

[B03] switch / match / case
来源：http://pr.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ov.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wd.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dn.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mm.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bp.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://at.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kg.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sw.newstarts.cn

[B04] for 计数循环
来源：http://gl.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://xl.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yt.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mv.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yy.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oj.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rq.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://fl.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rt.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://dn.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://rq.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ng.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://he.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://be.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ud.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wv.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://qf.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oa.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://hh.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bt.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ok.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dv.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://af.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cp.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://up.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ip.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dz.muxihuayi.cn

[B07] while 循环
来源：http://bp.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://yl.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bl.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://au.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://pv.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://mq.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jm.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://nv.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://bd.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://ub.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://ey.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pd.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://jg.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://ee.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://ub.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yh.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zs.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://ca.bjjhwx.cn

[B09] break 与 continue
来源：http://bz.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bs.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vf.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qf.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zx.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zp.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gx.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lf.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://od.huanxung.cn

[B10] 遍历同时拿索引
来源：http://hi.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ok.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zm.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ep.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sd.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wm.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mo.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qs.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mu.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://ds.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://hg.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://wm.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qt.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hw.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eo.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ru.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://xd.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pn.shxzskj.cn

[B12] 跳出多层循环
来源：http://uj.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qv.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vc.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ac.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bb.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iy.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kr.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uo.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qh.wgjwhj.cn

[B13] 判断是否为数字
来源：http://ln.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://zl.shxzukj.cn

PHP:  is_numeric($x)
来源：http://od.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://av.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hj.521024.cn

Java: x instanceof Number
来源：http://ap.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fb.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://gw.9csxet.cn

C#:   x is int or double or decimal
来源：http://dp.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://vf.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gj.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tl.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://oj.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://qi.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ul.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mv.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ao.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hn.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://kj.szsharing.cn

Py:   a and b or not c
来源：http://dd.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://hg.szsharing.cn

JS:   a && b || !c
来源：http://av.hnjuh.cn

TS:   a && b || !c
来源：http://kl.newstarts.cn

Java: a && b || !c
来源：http://gr.shxzukj.cn

Go:   a && b || !c
来源：http://qj.9csxet.cn

Ruby: a && b || !c
来源：http://ea.jctech888.com.cn

C#:   a && b || !c
来源：http://gc.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ok.bjjhwx.cn

Py:   if not data: return
来源：http://aa.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://bp.newstarts.cn

JS:   if (!data) return;
来源：http://qh.shtwfgs.cn

TS:   if (!data) return;
来源：http://ls.9csxet.cn

Java: if (data == null) return;
来源：http://ve.muxihuayi.cn

Go:   if data == nil { return }
来源：http://sr.wgjwhj.cn

Ruby: return if data.nil?
来源：http://fd.haigaiapp.cn

C#:   if (data == null) return;
来源：http://fn.muxihuayi.cn

================================================================================
来源：http://jd.muxihuayi.cn

C. 函数与作用域
来源：http://fp.hahajie.cn

================================================================================
来源：http://bk.wgjwhj.cn

[C01] 定义函数
来源：http://bc.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://ve.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ti.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://hy.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pr.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zv.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://os.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://us.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jv.jctech888.com.cn

[C02] 默认参数
来源：http://ul.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://hm.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sw.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://bc.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nt.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pe.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wd.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://dn.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://er.521024.cn

[C03] 可变参数
来源：http://tb.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://zz.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://be.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zt.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yf.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jv.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://it.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pw.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://em.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://gi.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fw.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qu.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pm.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zl.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://cb.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://nu.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://qb.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://uv.gzmigu.cn

[C05] 返回多个值
来源：http://nu.muxihuayi.cn

Py:   return a, b
来源：http://op.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://gf.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gn.asd995.cn

TS:   return { a, b };
来源：http://cw.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xq.newstarts.cn

Go:   return a, b
来源：http://zq.yuexingan06.cn

Ruby: return a, b
来源：http://un.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://fj.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://rb.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://ni.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ki.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://iy.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://mr.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yt.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tr.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://vu.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qn.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://uf.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zm.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://di.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dy.hahajie.cn

TS:   arr.map(String)
来源：http://ud.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bv.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ui.shxzukj.cn


<!-- 参考信息 -->