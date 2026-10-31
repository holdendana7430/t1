代发 wailian999

Java: "第一行\n第二行"
来源：http://yn.hahajie.cn

Go:   "第一行\n第二行"
来源：http://oj.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://wk.nszjky.cn

C#:   "第一行\n第二行"
来源：http://rr.wgjwhj.cn

[A14] 注释写法
来源：http://xi.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rn.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://md.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://uf.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://fs.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vd.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://kz.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hr.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://oh.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://ff.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://oc.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://sl.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://by.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://vc.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://it.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://lw.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://cl.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://ms.521024.cn

[A16] 真假值判断规则
来源：http://zf.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pj.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dn.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ww.huixiangedu.cn

TS:   if (!x) {}
来源：http://aw.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xt.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kp.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cb.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://or.szxytkj.cn

[A17] 位运算
来源：http://nx.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ei.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yq.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nf.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yv.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rj.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jv.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://if.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pj.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://oi.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://oz.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://ix.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vx.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lv.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://fj.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nv.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://zu.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://os.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://gm.asd995.cn

Py:   a, b = b, a
来源：http://rs.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nf.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://de.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://oy.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://rx.haigaiapp.cn

Go:   a, b = b, a
来源：http://ry.shxzukj.cn

Ruby: a, b = b, a
来源：http://bv.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://ou.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://du.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://hk.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kt.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lq.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://cw.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://le.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://en.wgjwhj.cn

Ruby: gets.chomp
来源：http://ct.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://jz.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://ld.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://rv.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hi.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://qr.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://xy.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://ts.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yi.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://cu.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://ts.bjjhwx.cn

[A22] 获取字符串长度
来源：http://bp.yuexingan06.cn

Py:   len(s)
来源：http://jm.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fg.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vv.lnxyls.cn

TS:   s.length
来源：http://td.yuexingan06.cn

Java: s.length()
来源：http://yp.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fl.wgjwhj.cn

Ruby: s.length
来源：http://ai.muxihuayi.cn

C#:   s.Length
来源：http://dl.wgjwhj.cn

[A23] 大小写转换
来源：http://oh.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ec.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ug.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nh.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rs.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://on.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tk.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zd.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jk.muxihuayi.cn

[A24] 去除首尾空白
来源：http://mt.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://al.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bv.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qn.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wa.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kv.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://ek.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kt.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ys.haigaiapp.cn

[A25] 字符串比较
来源：http://jp.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://rc.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rc.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yi.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kx.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fa.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xa.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fu.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ph.colortex.cn

[A26] 类型转换总览
来源：http://jb.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lm.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ow.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wp.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://an.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ga.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qr.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qk.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gm.9csxet.cn

================================================================================
来源：http://qt.chemitech.net.cn

B. 流程控制
来源：http://kl.gzmigu.cn

================================================================================
来源：http://we.hnjuh.cn

[B01] 条件判断 if / else
来源：http://ks.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pc.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cv.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cf.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://le.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://td.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cb.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ax.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jn.9csxet.cn

[B02] 多分支 else if / elif
来源：http://hw.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sy.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jm.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yr.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://na.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ip.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kt.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ks.colortex.cn

[B03] switch / match / case
来源：http://am.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ei.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bt.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tp.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://re.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ux.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jh.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vq.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sh.bjjhwx.cn

[B04] for 计数循环
来源：http://ly.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://ty.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ev.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vi.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aj.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xx.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://us.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://be.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://if.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://zn.asd995.cn

Py:   for item in arr: print(item)
来源：http://zb.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gz.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xl.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zu.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vw.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zz.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://kt.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qg.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://hs.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pz.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tj.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jx.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ic.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fj.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sm.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vi.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wa.huanxung.cn

[B07] while 循环
来源：http://pc.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://lt.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://um.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://uw.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://yc.521024.cn

Java: while (i < 10) { i++; }
来源：http://fi.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mv.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://zj.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://ze.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://ad.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://is.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bo.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://ub.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://vy.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://zq.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pz.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fc.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://ui.szsharing.cn

[B09] break 与 continue
来源：http://uv.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gd.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fp.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lo.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mg.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uf.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bh.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mf.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cu.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://hh.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ue.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ol.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nv.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vp.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kk.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sh.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wn.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://go.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://xr.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://fm.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://xm.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tc.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ly.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wq.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tf.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://fe.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://do.jctech888.com.cn

[B12] 跳出多层循环
来源：http://mm.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ku.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tx.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jo.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ds.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bn.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ld.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hp.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bl.wgjwhj.cn

[B13] 判断是否为数字
来源：http://sr.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://zx.asd995.cn

PHP:  is_numeric($x)
来源：http://td.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://op.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kv.szsharing.cn

Java: x instanceof Number
来源：http://bw.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sf.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://sb.521024.cn

C#:   x is int or double or decimal
来源：http://ab.newstarts.cn

[B14] 判断值是否在集合内
来源：http://wz.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jk.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fx.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://hh.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ku.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mv.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://id.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qd.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xd.huanxung.cn

[B15] 布尔运算与取反
来源：http://jr.muxihuayi.cn

Py:   a and b or not c
来源：http://wb.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://ya.huixiangedu.cn

JS:   a && b || !c
来源：http://fq.shtwfgs.cn

TS:   a && b || !c
来源：http://wu.shtwfgs.cn

Java: a && b || !c
来源：http://da.huanxung.cn

Go:   a && b || !c
来源：http://qx.hahajie.cn

Ruby: a && b || !c
来源：http://dv.asd995.cn

C#:   a && b || !c
来源：http://pp.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gc.yuntaijiaju.cn

Py:   if not data: return
来源：http://ei.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://hk.szsharing.cn

JS:   if (!data) return;
来源：http://fh.bookmarksfly.cn

TS:   if (!data) return;
来源：http://xr.jctech888.com.cn

Java: if (data == null) return;
来源：http://zy.yuexingan06.cn

Go:   if data == nil { return }
来源：http://db.chemitech.net.cn

Ruby: return if data.nil?
来源：http://ld.shxzukj.cn

C#:   if (data == null) return;
来源：http://kb.muxihuayi.cn

================================================================================
来源：http://oc.jctech888.com.cn

C. 函数与作用域
来源：http://ya.shtwfgs.cn

================================================================================
来源：http://kn.hnjuh.cn

[C01] 定义函数
来源：http://ev.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://df.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ym.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://jc.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ie.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jr.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vq.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://di.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xw.yuntaijiaju.cn

[C02] 默认参数
来源：http://wv.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://vv.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vz.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://vv.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tg.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cc.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xm.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://oq.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://gb.panjiajie.cn

[C03] 可变参数
来源：http://lj.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://ne.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zs.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ui.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oy.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ld.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sq.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lw.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ar.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ll.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qw.nicolike.cn


<!-- 参考信息 -->