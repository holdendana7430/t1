代发 wailian999

Py:   "第一行\n第二行"
来源：http://wy.521024.cn

PHP:  "第一行\n第二行"
来源：http://tj.hahajie.cn

JS:   "第一行\n第二行"
来源：http://ag.nszjky.cn

TS:   "第一行\n第二行"
来源：http://os.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://ok.hahajie.cn

Go:   "第一行\n第二行"
来源：http://gx.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://qc.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://vd.shxzskj.cn

[A14] 注释写法
来源：http://wv.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qg.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wj.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://un.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://hq.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vf.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://ca.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jk.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://cu.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://yy.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://px.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ks.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://uj.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://io.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://il.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://uj.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://vp.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://ft.shxzukj.cn

[A16] 真假值判断规则
来源：http://jf.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ud.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bv.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qv.newstarts.cn

TS:   if (!x) {}
来源：http://ov.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oo.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ea.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zb.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://al.panjiajie.cn

[A17] 位运算
来源：http://ao.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dx.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pp.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yn.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://po.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oy.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ar.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hj.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kt.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://lk.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://zb.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://xi.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ow.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ub.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://hh.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fq.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://oi.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://un.asd995.cn

[A19] 交换两个变量
来源：http://rg.wgjwhj.cn

Py:   a, b = b, a
来源：http://lw.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ty.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://lc.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://qt.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://if.yuexingan06.cn

Go:   a, b = b, a
来源：http://jd.yuexingan06.cn

Ruby: a, b = b, a
来源：http://tm.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://uq.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://gu.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://jt.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zc.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bd.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://rc.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://li.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wc.9csxet.cn

Ruby: gets.chomp
来源：http://as.shxzskj.cn

C#:   Console.ReadLine();
来源：http://yw.521024.cn

[A21] 保留指定小数位输出
来源：http://ck.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://jh.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fl.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://dp.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://cr.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://cc.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hx.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://mp.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://cr.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://lg.bjjhwx.cn

Py:   len(s)
来源：http://wg.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lm.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://le.colortex.cn

TS:   s.length
来源：http://rv.szxytkj.cn

Java: s.length()
来源：http://xi.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fo.muxihuayi.cn

Ruby: s.length
来源：http://po.newstarts.cn

C#:   s.Length
来源：http://bs.521024.cn

[A23] 大小写转换
来源：http://jc.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wt.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qw.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wg.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://io.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rs.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jm.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://on.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hj.asd995.cn

[A24] 去除首尾空白
来源：http://ot.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cd.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hr.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ih.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zf.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vj.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://va.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jh.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://np.shtwfgs.cn

[A25] 字符串比较
来源：http://em.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://fi.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ru.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oq.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xo.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ck.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qo.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ho.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xu.colortex.cn

[A26] 类型转换总览
来源：http://iz.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fh.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qo.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zp.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://hx.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ux.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ug.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uu.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rf.shxzukj.cn

================================================================================
来源：http://lo.chemitech.net.cn

B. 流程控制
来源：http://nr.nszjky.cn

================================================================================
来源：http://nx.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://tx.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hx.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gw.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xq.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nu.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://on.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rf.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hu.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eb.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://pw.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nn.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fn.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dr.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://um.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yb.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wa.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qu.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://se.shtwfgs.cn

[B03] switch / match / case
来源：http://hy.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://em.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ea.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://id.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cj.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cj.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vf.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jl.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://re.jianghongdianzi.cn

[B04] for 计数循环
来源：http://vg.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://ws.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tt.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://et.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sa.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qh.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zi.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://gf.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lr.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://gw.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://bo.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mi.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gm.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://az.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nu.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://em.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://pr.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fa.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://sl.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ap.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gj.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qe.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://or.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://in.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fm.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mu.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://um.hnjuh.cn

[B07] while 循环
来源：http://rr.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://sd.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jj.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://gc.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://um.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://kl.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ux.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://mm.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://at.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://gh.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://jb.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yv.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://tr.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://yk.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://ll.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rv.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wp.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://sd.9csxet.cn

[B09] break 与 continue
来源：http://hj.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zy.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yw.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ti.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://co.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lw.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pq.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hr.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rf.asd995.cn

[B10] 遍历同时拿索引
来源：http://cn.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wp.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xc.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wp.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xf.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xg.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cd.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nw.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tz.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://cl.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://sj.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://nb.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gm.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ga.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rr.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fm.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://bq.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://us.hnjuh.cn

[B12] 跳出多层循环
来源：http://ld.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ty.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vy.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kg.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kn.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vx.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ji.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zr.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cz.wgjwhj.cn

[B13] 判断是否为数字
来源：http://ba.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://iq.nicolike.cn

PHP:  is_numeric($x)
来源：http://rk.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kt.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ns.bjjhwx.cn

Java: x instanceof Number
来源：http://yt.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lt.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://zf.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://uk.9csxet.cn

[B14] 判断值是否在集合内
来源：http://bo.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://le.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pv.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://yg.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://gq.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ev.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lq.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sw.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kx.hnjuh.cn

[B15] 布尔运算与取反
来源：http://am.521024.cn

Py:   a and b or not c
来源：http://jx.nszjky.cn

PHP:  $a && $b || !$c
来源：http://vu.chemitech.net.cn

JS:   a && b || !c
来源：http://qd.chemitech.net.cn

TS:   a && b || !c
来源：http://xr.panjiajie.cn

Java: a && b || !c
来源：http://ep.lnxyls.cn

Go:   a && b || !c
来源：http://kj.shtwfgs.cn

Ruby: a && b || !c
来源：http://ko.muxihuayi.cn

C#:   a && b || !c
来源：http://cr.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tm.huixinmuqiang.cn

Py:   if not data: return
来源：http://mw.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://uj.521024.cn

JS:   if (!data) return;
来源：http://rl.szsharing.cn

TS:   if (!data) return;
来源：http://xs.huanxung.cn

Java: if (data == null) return;
来源：http://ab.huanxung.cn

Go:   if data == nil { return }
来源：http://pc.bjjhwx.cn

Ruby: return if data.nil?
来源：http://pq.shtwfgs.cn

C#:   if (data == null) return;
来源：http://ed.asd995.cn

================================================================================
来源：http://uk.asd995.cn

C. 函数与作用域
来源：http://hl.shtwfgs.cn

================================================================================
来源：http://gf.gzmigu.cn

[C01] 定义函数
来源：http://by.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://zw.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qm.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://ng.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sx.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rg.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bx.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://ze.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ke.shtwfgs.cn

[C02] 默认参数
来源：http://bl.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://wk.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://si.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://ak.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://di.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hq.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://up.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://cw.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://mn.lnxyls.cn

[C03] 可变参数
来源：http://yc.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://ch.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://br.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lo.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cm.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xn.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bz.huixiangedu.cn


<!-- 参考信息 -->