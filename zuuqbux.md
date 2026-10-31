代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fz.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hy.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rk.hnjuh.cn

[A17] 位运算
来源：http://zv.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wo.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sd.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yz.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oq.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mb.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tv.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kk.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://it.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://vm.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://yu.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ot.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mx.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://dt.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zl.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://va.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://xv.panjiajie.cn

[A19] 交换两个变量
来源：http://wd.newstarts.cn

Py:   a, b = b, a
来源：http://pa.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tj.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://ce.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://xy.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://qt.huixiangedu.cn

Go:   a, b = b, a
来源：http://ng.lnxyls.cn

Ruby: a, b = b, a
来源：http://to.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://vw.9csxet.cn

[A20] 读取标准输入
来源：http://tv.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://kv.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sg.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bn.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://fg.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://qo.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zs.521024.cn

Ruby: gets.chomp
来源：http://gk.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://zh.huanxung.cn

[A21] 保留指定小数位输出
来源：http://nl.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://we.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wb.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://sh.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://sg.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://wz.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yo.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://zf.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://yh.wgjwhj.cn

[A22] 获取字符串长度
来源：http://xb.chemitech.net.cn

Py:   len(s)
来源：http://cb.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xq.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gq.newstarts.cn

TS:   s.length
来源：http://yr.gzmigu.cn

Java: s.length()
来源：http://pd.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ng.nicolike.cn

Ruby: s.length
来源：http://jp.asd995.cn

C#:   s.Length
来源：http://vs.panjiajie.cn

[A23] 大小写转换
来源：http://yv.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dd.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vp.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tb.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qk.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mq.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qj.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://md.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ni.yuexingan06.cn

[A24] 去除首尾空白
来源：http://nx.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uk.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ap.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eo.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xp.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fx.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://iu.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://my.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gf.lnxyls.cn

[A25] 字符串比较
来源：http://he.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://jw.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xy.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xx.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wo.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yn.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://te.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jh.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.shtwfgs.cn

[A26] 类型转换总览
来源：http://or.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jp.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ua.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vt.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://te.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bv.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ur.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iw.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vl.hahajie.cn

================================================================================
来源：http://uk.szsharing.cn

B. 流程控制
来源：http://dz.huanxung.cn

================================================================================
来源：http://sq.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://je.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nt.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tc.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ng.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wp.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bl.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fr.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://id.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rn.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://iv.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ca.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cj.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mw.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kq.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qi.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://et.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gj.gzmigu.cn

[B03] switch / match / case
来源：http://jf.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://so.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cq.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vf.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ci.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mc.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ef.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zp.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bk.nszjky.cn

[B04] for 计数循环
来源：http://zc.521024.cn

Py:   for i in range(10): print(i)
来源：http://vq.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wo.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dj.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ga.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eh.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ay.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://wj.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cw.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://ms.huanxung.cn

Py:   for item in arr: print(item)
来源：http://sv.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ff.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ji.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vm.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nk.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wz.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://lq.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vt.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://gg.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yg.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yq.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xa.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gh.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wv.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gr.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rd.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yj.yuexingan06.cn

[B07] while 循环
来源：http://zn.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://mo.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ev.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://id.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://el.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://yw.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mz.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://ph.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://ce.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://ym.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://tg.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sn.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://wd.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://vr.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://pr.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jo.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yh.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://at.huanxung.cn

[B09] break 与 continue
来源：http://nk.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ta.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eb.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gh.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nw.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mi.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mh.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mb.szsharing.cn

[B10] 遍历同时拿索引
来源：http://vj.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iv.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nl.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gf.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hm.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gc.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mt.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cx.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://py.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://ho.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://fj.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://ku.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xi.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sj.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vz.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qp.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://aw.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pi.panjiajie.cn

[B12] 跳出多层循环
来源：http://jz.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rp.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ob.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cj.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jt.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fx.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gp.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qk.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sc.521024.cn

[B13] 判断是否为数字
来源：http://ei.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://sq.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://rw.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hx.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wy.lnxyls.cn

Java: x instanceof Number
来源：http://sw.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sl.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://fl.huanxung.cn

C#:   x is int or double or decimal
来源：http://pj.newstarts.cn

[B14] 判断值是否在集合内
来源：http://bz.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jp.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zu.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://bg.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://wo.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mq.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tz.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mx.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lp.gzmigu.cn

[B15] 布尔运算与取反
来源：http://wp.shxzukj.cn

Py:   a and b or not c
来源：http://tf.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://wd.9csxet.cn

JS:   a && b || !c
来源：http://jl.521024.cn

TS:   a && b || !c
来源：http://qe.jctech888.com.cn

Java: a && b || !c
来源：http://oo.muxihuayi.cn

Go:   a && b || !c
来源：http://qj.haigaiapp.cn

Ruby: a && b || !c
来源：http://md.asd995.cn

C#:   a && b || !c
来源：http://ko.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mq.nicolike.cn

Py:   if not data: return
来源：http://bz.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://gk.hahajie.cn

JS:   if (!data) return;
来源：http://ue.huanxung.cn

TS:   if (!data) return;
来源：http://hm.gzmigu.cn

Java: if (data == null) return;
来源：http://kb.colortex.cn

Go:   if data == nil { return }
来源：http://ih.huanxung.cn

Ruby: return if data.nil?
来源：http://zt.shxzskj.cn

C#:   if (data == null) return;
来源：http://xm.asd995.cn

================================================================================
来源：http://gu.nicolike.cn

C. 函数与作用域
来源：http://gf.gzmigu.cn

================================================================================
来源：http://hp.colortex.cn

[C01] 定义函数
来源：http://ei.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ag.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zf.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://gp.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jd.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fx.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lk.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://fm.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rl.panjiajie.cn

[C02] 默认参数
来源：http://wk.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://fx.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nc.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://vv.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cq.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nw.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wx.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://vq.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://ym.nicolike.cn

[C03] 可变参数
来源：http://kp.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://nq.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mp.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ie.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vy.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cz.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bb.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eq.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://is.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://xy.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://in.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bm.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ez.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oy.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://yd.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://un.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://qf.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://tl.haigaiapp.cn

[C05] 返回多个值
来源：http://qr.asd995.cn

Py:   return a, b
来源：http://gd.nszjky.cn

PHP:  return [$a, $b];
来源：http://wv.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bx.nszjky.cn

TS:   return { a, b };
来源：http://re.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fu.yuntaijiaju.cn

Go:   return a, b
来源：http://ka.muxihuayi.cn

Ruby: return a, b
来源：http://uz.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://vb.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://wp.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://zd.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uw.panjiajie.cn

JS:   const square = x => x * x;
来源：http://hp.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://me.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qz.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vg.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://oj.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sn.nicolike.cn

[C07] 把函数作为参数传入
来源：http://fb.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mg.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fq.shtwfgs.cn


<!-- 参考信息 -->