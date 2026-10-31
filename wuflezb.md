代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jw.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eg.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lh.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://av.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://at.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iv.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hf.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wc.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://gq.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://yk.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://it.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fp.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zv.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://yv.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kw.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://oh.colortex.cn

C#:   (int)'A'; (char)65
来源：http://mw.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://ol.chemitech.net.cn

Py:   a, b = b, a
来源：http://de.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zj.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://ry.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://gb.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://nn.gzmigu.cn

Go:   a, b = b, a
来源：http://jy.muxihuayi.cn

Ruby: a, b = b, a
来源：http://ff.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://da.shxzskj.cn

[A20] 读取标准输入
来源：http://tj.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://so.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fs.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gp.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://ko.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://hs.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://we.hnjuh.cn

Ruby: gets.chomp
来源：http://sg.521024.cn

C#:   Console.ReadLine();
来源：http://cb.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://vp.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://ti.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hx.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://jn.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://db.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://lp.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wb.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://yr.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://qt.521024.cn

[A22] 获取字符串长度
来源：http://yw.szxytkj.cn

Py:   len(s)
来源：http://ip.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pc.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jp.hahajie.cn

TS:   s.length
来源：http://ka.shxzskj.cn

Java: s.length()
来源：http://sr.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://df.wgjwhj.cn

Ruby: s.length
来源：http://qy.colortex.cn

C#:   s.Length
来源：http://ob.wgjwhj.cn

[A23] 大小写转换
来源：http://pd.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rg.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uq.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xj.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xu.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hy.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gh.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://un.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sf.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://dz.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sa.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ck.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bf.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bj.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://np.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://er.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cs.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hc.newstarts.cn

[A25] 字符串比较
来源：http://fe.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://ow.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kp.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fz.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://te.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ud.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iy.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wy.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gf.bjjhwx.cn

[A26] 类型转换总览
来源：http://wr.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://be.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://av.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ni.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://bs.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ri.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ps.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rb.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://po.panjiajie.cn

================================================================================
来源：http://jk.yuntaijiaju.cn

B. 流程控制
来源：http://lw.yuexingan06.cn

================================================================================
来源：http://bz.newstarts.cn

[B01] 条件判断 if / else
来源：http://qg.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ms.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zw.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://la.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lq.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yx.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jd.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dy.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ur.nszjky.cn

[B02] 多分支 else if / elif
来源：http://pe.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zr.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ij.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bg.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vt.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://im.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jr.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jq.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ay.muxihuayi.cn

[B03] switch / match / case
来源：http://um.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ki.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qh.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ei.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fr.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ak.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ur.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gj.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zk.huixinmuqiang.cn

[B04] for 计数循环
来源：http://ou.colortex.cn

Py:   for i in range(10): print(i)
来源：http://sz.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://np.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rb.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jg.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://za.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://az.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://dp.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dp.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://rs.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://bn.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ea.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ng.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ab.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nw.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://az.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://nq.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://up.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://bc.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ca.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uu.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://el.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://if.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uj.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://od.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dt.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hh.szxytkj.cn

[B07] while 循环
来源：http://rt.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://bl.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gq.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://vx.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://fi.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://rm.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mq.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://sv.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://lt.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://gm.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://mm.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://de.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://vu.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://ay.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://qp.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wm.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yl.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://mc.panjiajie.cn

[B09] break 与 continue
来源：http://cd.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ym.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ox.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ml.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kk.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uv.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yv.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sg.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ov.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://dz.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mc.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xt.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sv.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ol.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wm.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ex.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fz.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ul.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://ir.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://mr.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://dq.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sq.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://re.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kh.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ba.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://jn.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yt.asd995.cn

[B12] 跳出多层循环
来源：http://po.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xr.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qb.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nv.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bi.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://km.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lg.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ny.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://um.chemitech.net.cn

[B13] 判断是否为数字
来源：http://xz.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://bd.shxzskj.cn

PHP:  is_numeric($x)
来源：http://ot.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oi.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fm.jianghongdianzi.cn

Java: x instanceof Number
来源：http://xs.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://td.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://na.hahajie.cn

C#:   x is int or double or decimal
来源：http://ap.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://wk.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://td.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ke.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://mm.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://ya.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fd.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zb.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dl.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fq.asd995.cn

[B15] 布尔运算与取反
来源：http://cn.lnxyls.cn

Py:   a and b or not c
来源：http://hi.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ex.bjjhwx.cn

JS:   a && b || !c
来源：http://gn.521024.cn

TS:   a && b || !c
来源：http://ki.jianghongdianzi.cn

Java: a && b || !c
来源：http://cl.gzmigu.cn

Go:   a && b || !c
来源：http://bf.panjiajie.cn

Ruby: a && b || !c
来源：http://sa.wgjwhj.cn

C#:   a && b || !c
来源：http://al.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yo.huixiangedu.cn

Py:   if not data: return
来源：http://ry.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://sc.nszjky.cn

JS:   if (!data) return;
来源：http://sy.panjiajie.cn

TS:   if (!data) return;
来源：http://lq.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://if.chemitech.net.cn

Go:   if data == nil { return }
来源：http://em.lnxyls.cn

Ruby: return if data.nil?
来源：http://py.jctech888.com.cn

C#:   if (data == null) return;
来源：http://rk.jctech888.com.cn

================================================================================
来源：http://yw.9csxet.cn

C. 函数与作用域
来源：http://oc.shtwfgs.cn

================================================================================
来源：http://em.asd995.cn

[C01] 定义函数
来源：http://ly.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://ma.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ax.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://wu.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gp.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pg.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ll.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://tf.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tv.lnxyls.cn

[C02] 默认参数
来源：http://eq.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://md.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iy.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://zw.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ek.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pg.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ae.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://nb.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://ne.haigaiapp.cn

[C03] 可变参数
来源：http://qm.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://qz.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kz.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cv.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zp.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ne.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://in.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nb.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ku.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://qg.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://in.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uw.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nn.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fo.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://dn.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://jy.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://dv.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://lp.huixiangedu.cn

[C05] 返回多个值
来源：http://iv.asd995.cn

Py:   return a, b
来源：http://at.hahajie.cn

PHP:  return [$a, $b];
来源：http://vp.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pp.521024.cn

TS:   return { a, b };
来源：http://yd.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rs.szxytkj.cn

Go:   return a, b
来源：http://wy.bjjhwx.cn

Ruby: return a, b
来源：http://xb.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://yx.colortex.cn

[C06] 匿名函数 / lambda
来源：http://er.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://qg.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dp.huanxung.cn

JS:   const square = x => x * x;
来源：http://wd.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://gx.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ph.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dz.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://bg.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dr.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://gc.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vz.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xv.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dl.nszjky.cn

TS:   arr.map(String)
来源：http://lv.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bw.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nh.bjjhwx.cn


<!-- 参考信息 -->