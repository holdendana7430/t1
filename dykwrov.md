代发 wailian999

Java: "第一行\n第二行"
来源：http://vn.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://up.asd995.cn

Ruby: "第一行\n第二行"
来源：http://uq.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://mh.panjiajie.cn

[A14] 注释写法
来源：http://ne.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ab.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gs.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://wf.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://pp.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wb.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://dr.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://or.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://mh.panjiajie.cn

[A15] 空值判断与默认值
来源：http://gu.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://xi.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://hy.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://ap.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://ck.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rm.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://wc.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://gt.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://ht.nszjky.cn

[A16] 真假值判断规则
来源：http://ul.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kw.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kw.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bq.newstarts.cn

TS:   if (!x) {}
来源：http://ae.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://po.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vs.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yg.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ci.szsharing.cn

[A17] 位运算
来源：http://sd.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lq.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pg.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nk.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mp.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gy.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dp.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xh.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xp.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://nf.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://ae.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://rt.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qo.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://at.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://ok.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mp.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://if.colortex.cn

C#:   (int)'A'; (char)65
来源：http://mx.lnxyls.cn

[A19] 交换两个变量
来源：http://mu.bjjhwx.cn

Py:   a, b = b, a
来源：http://kx.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jk.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://lg.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://uy.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://ud.colortex.cn

Go:   a, b = b, a
来源：http://rd.nicolike.cn

Ruby: a, b = b, a
来源：http://iv.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://up.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ur.shxzskj.cn

Py:   name = input("请输入：")
来源：http://ux.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mr.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tx.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://ij.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://fa.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tz.nszjky.cn

Ruby: gets.chomp
来源：http://hk.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://ci.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://do.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://yr.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ws.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://zs.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://ov.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://gz.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ae.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://df.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://ez.gzmigu.cn

[A22] 获取字符串长度
来源：http://pg.hahajie.cn

Py:   len(s)
来源：http://xi.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fu.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jp.lnxyls.cn

TS:   s.length
来源：http://oh.szxytkj.cn

Java: s.length()
来源：http://hd.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ez.shtwfgs.cn

Ruby: s.length
来源：http://yt.bookmarksfly.cn

C#:   s.Length
来源：http://nm.hahajie.cn

[A23] 大小写转换
来源：http://eq.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kf.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vp.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ui.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wg.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cn.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qs.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fe.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hl.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://jk.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ic.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qf.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nk.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pa.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xe.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://xe.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cq.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mm.shtwfgs.cn

[A25] 字符串比较
来源：http://ol.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://ep.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wc.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://er.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zh.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://av.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ou.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vq.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fs.colortex.cn

[A26] 类型转换总览
来源：http://gy.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vj.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ii.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vz.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://vo.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oy.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wq.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sy.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ln.bjjhwx.cn

================================================================================
来源：http://vh.wgjwhj.cn

B. 流程控制
来源：http://md.chemitech.net.cn

================================================================================
来源：http://ds.szsharing.cn

[B01] 条件判断 if / else
来源：http://xh.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bs.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lh.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tp.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ov.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://de.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tn.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://en.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kz.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://mt.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mi.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oo.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://as.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ta.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kw.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ih.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nq.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tk.lnxyls.cn

[B03] switch / match / case
来源：http://oj.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lr.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://td.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wl.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eo.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bn.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sl.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bc.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pw.huanxung.cn

[B04] for 计数循环
来源：http://ck.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://hw.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qw.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tl.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yv.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qy.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://op.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://tj.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cn.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://ui.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://az.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sl.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tr.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tj.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://du.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://my.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://aj.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wb.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ak.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tf.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wf.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mb.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cc.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lc.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oi.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tm.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://us.nszjky.cn

[B07] while 循环
来源：http://ty.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://lq.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ph.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://nt.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://tk.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://bi.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kl.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://ut.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://ci.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://rz.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://el.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ls.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://em.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://gu.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://in.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pg.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sc.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://ew.9csxet.cn

[B09] break 与 continue
来源：http://sg.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mb.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ui.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nf.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zt.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ta.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://in.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xv.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ol.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://dx.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qs.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yy.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gb.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ms.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://le.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zk.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pw.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hl.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://ac.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://kp.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://zu.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vv.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uh.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qa.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wc.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://ws.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cu.521024.cn

[B12] 跳出多层循环
来源：http://sx.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qg.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://el.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ob.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ek.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zm.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wj.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pm.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xa.nszjky.cn

[B13] 判断是否为数字
来源：http://gx.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://bo.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://mp.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://br.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ns.shxzskj.cn

Java: x instanceof Number
来源：http://oz.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xj.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://my.nszjky.cn

C#:   x is int or double or decimal
来源：http://pd.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://en.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ht.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zh.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://hx.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://nf.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://je.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://so.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eo.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kt.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://rr.szsharing.cn

Py:   a and b or not c
来源：http://zg.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://vh.521024.cn

JS:   a && b || !c
来源：http://lt.chemitech.net.cn

TS:   a && b || !c
来源：http://fx.yuntaijiaju.cn

Java: a && b || !c
来源：http://nq.huixinmuqiang.cn

Go:   a && b || !c
来源：http://kl.shtwfgs.cn

Ruby: a && b || !c
来源：http://po.hnjuh.cn

C#:   a && b || !c
来源：http://jb.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://be.huixiangedu.cn

Py:   if not data: return
来源：http://pv.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://og.panjiajie.cn

JS:   if (!data) return;
来源：http://pg.huixiangedu.cn

TS:   if (!data) return;
来源：http://jp.panjiajie.cn

Java: if (data == null) return;
来源：http://ei.huanxung.cn

Go:   if data == nil { return }
来源：http://vx.szxytkj.cn

Ruby: return if data.nil?
来源：http://tg.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://sp.jctech888.com.cn

================================================================================
来源：http://zd.nszjky.cn

C. 函数与作用域
来源：http://hg.nszjky.cn

================================================================================
来源：http://xl.lnxyls.cn

[C01] 定义函数
来源：http://lf.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://io.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ed.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://ej.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sj.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vr.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ow.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://ob.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ov.jctech888.com.cn

[C02] 默认参数
来源：http://bh.asd995.cn

Py:   def greet(name="World"): return name
来源：http://xr.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ff.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://nh.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ee.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://av.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yf.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://ky.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://dp.huanxung.cn

[C03] 可变参数
来源：http://fn.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://rm.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://op.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vq.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pb.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dz.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zm.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hk.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rn.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://ec.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uz.shxzskj.cn


<!-- 参考信息 -->