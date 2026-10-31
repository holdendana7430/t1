代发 wailian999

Py:   "第一行\n第二行"
来源：http://aj.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://hv.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://qr.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://pt.hnjuh.cn

Java: "第一行\n第二行"
来源：http://tl.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://ir.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://jv.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://dg.jianghongdianzi.cn

[A14] 注释写法
来源：http://wc.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fm.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://us.521024.cn

JS:   // 单行；/* 多行 */
来源：http://ag.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://vg.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ww.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://zy.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ng.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://zs.szsharing.cn

[A15] 空值判断与默认值
来源：http://zf.newstarts.cn

Py:   value = data or "默认值"
来源：http://rf.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://wg.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://jt.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://gg.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mx.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://bd.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://mw.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://pq.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://yj.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://up.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xj.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bf.9csxet.cn

TS:   if (!x) {}
来源：http://ex.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jj.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fn.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rp.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ra.newstarts.cn

[A17] 位运算
来源：http://rg.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://su.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jq.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rh.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pd.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jn.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ag.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vk.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kw.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://zg.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://hf.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://rf.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ii.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oy.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://be.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xb.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://mx.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://pk.haigaiapp.cn

[A19] 交换两个变量
来源：http://vp.chemitech.net.cn

Py:   a, b = b, a
来源：http://wn.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xl.asd995.cn

JS:   [a, b] = [b, a];
来源：http://et.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://px.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://tj.shxzukj.cn

Go:   a, b = b, a
来源：http://cx.szxytkj.cn

Ruby: a, b = b, a
来源：http://mx.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://dd.9csxet.cn

[A20] 读取标准输入
来源：http://yw.huanxung.cn

Py:   name = input("请输入：")
来源：http://sh.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qf.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cj.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://ya.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://pq.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cd.szxytkj.cn

Ruby: gets.chomp
来源：http://pj.9csxet.cn

C#:   Console.ReadLine();
来源：http://qg.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://lc.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://ao.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sm.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://ez.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://on.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://xz.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tl.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://qc.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://oq.shxzukj.cn

[A22] 获取字符串长度
来源：http://mw.colortex.cn

Py:   len(s)
来源：http://fu.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rg.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ve.hnjuh.cn

TS:   s.length
来源：http://rc.panjiajie.cn

Java: s.length()
来源：http://tu.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yz.asd995.cn

Ruby: s.length
来源：http://np.jianghongdianzi.cn

C#:   s.Length
来源：http://nk.gzmigu.cn

[A23] 大小写转换
来源：http://jq.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tv.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wt.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dt.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fv.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xo.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rq.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fj.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gu.shxzukj.cn

[A24] 去除首尾空白
来源：http://ic.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oc.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://di.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wg.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://np.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://no.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://of.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yd.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wn.gzmigu.cn

[A25] 字符串比较
来源：http://sw.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://ls.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vd.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://im.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kw.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hs.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rc.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wd.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mt.gzmigu.cn

[A26] 类型转换总览
来源：http://ii.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ix.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qi.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://or.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://lf.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ay.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gk.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zd.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xi.jianghongdianzi.cn

================================================================================
来源：http://fl.jctech888.com.cn

B. 流程控制
来源：http://sj.jctech888.com.cn

================================================================================
来源：http://ic.nicolike.cn

[B01] 条件判断 if / else
来源：http://hd.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ea.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fb.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zq.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yt.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gh.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tv.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mq.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jh.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://br.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tt.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zz.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uf.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://io.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ak.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bp.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ii.huixinmuqiang.cn

[B03] switch / match / case
来源：http://ru.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pa.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ul.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kp.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nn.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xc.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gl.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://on.chemitech.net.cn

[B04] for 计数循环
来源：http://lu.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://oh.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hg.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oh.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cd.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zv.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ms.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://hm.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ep.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://ng.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ij.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ja.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nr.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ov.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bd.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fk.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://dl.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nr.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://wn.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ms.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lf.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ae.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hw.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rc.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zy.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wn.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fa.haigaiapp.cn

[B07] while 循环
来源：http://dw.nicolike.cn

Py:   while i < 10: i += 1
来源：http://uh.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zi.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://if.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://pv.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://sc.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sx.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://gh.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://lk.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://vn.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://xv.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yi.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://ln.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://fl.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://ro.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://du.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sb.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://qw.521024.cn

[B09] break 与 continue
来源：http://xo.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gn.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nt.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ie.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nh.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pq.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://or.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eu.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cq.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://bp.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xj.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mm.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pq.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uq.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ro.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qw.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pa.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mo.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://ar.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://az.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://rn.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kn.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://on.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bh.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://te.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://ln.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ds.bjjhwx.cn

[B12] 跳出多层循环
来源：http://dd.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yf.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xn.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ww.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://et.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gs.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ww.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ws.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fu.huanxung.cn

[B13] 判断是否为数字
来源：http://ni.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://su.colortex.cn

PHP:  is_numeric($x)
来源：http://js.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ce.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dn.jianghongdianzi.cn

Java: x instanceof Number
来源：http://po.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://am.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://jp.szsharing.cn

C#:   x is int or double or decimal
来源：http://ed.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://lb.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dj.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tg.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://rp.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://rz.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lb.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tn.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cn.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pt.shxzukj.cn

[B15] 布尔运算与取反
来源：http://aa.asd995.cn

Py:   a and b or not c
来源：http://jp.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://gd.panjiajie.cn

JS:   a && b || !c
来源：http://bq.lnxyls.cn

TS:   a && b || !c
来源：http://rj.asd995.cn

Java: a && b || !c
来源：http://yg.panjiajie.cn

Go:   a && b || !c
来源：http://pa.yuexingan06.cn

Ruby: a && b || !c
来源：http://ju.jctech888.com.cn

C#:   a && b || !c
来源：http://fe.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hj.colortex.cn

Py:   if not data: return
来源：http://zr.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://ix.bookmarksfly.cn

JS:   if (!data) return;
来源：http://ft.bookmarksfly.cn

TS:   if (!data) return;
来源：http://bs.bjjhwx.cn

Java: if (data == null) return;
来源：http://ib.huixiangedu.cn

Go:   if data == nil { return }
来源：http://ny.nicolike.cn

Ruby: return if data.nil?
来源：http://zu.huanxung.cn

C#:   if (data == null) return;
来源：http://bz.huanxung.cn

================================================================================
来源：http://ni.colortex.cn

C. 函数与作用域
来源：http://rt.521024.cn

================================================================================
来源：http://ln.szsharing.cn

[C01] 定义函数
来源：http://ud.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://jv.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zj.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://sd.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lw.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sa.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ir.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://rb.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ke.huanxung.cn

[C02] 默认参数
来源：http://lq.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://sj.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://po.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://hs.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xa.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qq.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yw.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://rs.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://am.nicolike.cn

[C03] 可变参数
来源：http://fu.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://fh.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ep.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://or.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://no.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yq.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fp.panjiajie.cn


<!-- 参考信息 -->