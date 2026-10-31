代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://jm.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pc.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://oe.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jq.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qv.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://fq.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://jn.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://yb.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uu.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://dd.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://gv.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yq.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://ux.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://zd.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://qa.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://nz.huanxung.cn

Java: "第一行\n第二行"
来源：http://ff.nicolike.cn

Go:   "第一行\n第二行"
来源：http://gv.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://ns.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://kc.panjiajie.cn

[A14] 注释写法
来源：http://hg.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sk.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ro.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://ba.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://so.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wk.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://rc.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fg.521024.cn

C#:   // 单行；/* 多行 */
来源：http://jr.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://cu.newstarts.cn

Py:   value = data or "默认值"
来源：http://sz.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://ru.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://jq.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://jb.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gp.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://oa.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://mc.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://ra.colortex.cn

[A16] 真假值判断规则
来源：http://zt.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://av.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ox.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://an.hahajie.cn

TS:   if (!x) {}
来源：http://xp.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rv.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pq.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gq.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bl.lnxyls.cn

[A17] 位运算
来源：http://bq.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yd.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vl.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yo.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rn.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rh.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://se.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ij.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bn.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://bm.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://el.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://ny.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pa.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qp.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://kc.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ff.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://or.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://cp.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://sv.bookmarksfly.cn

Py:   a, b = b, a
来源：http://dd.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://di.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://wd.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://wk.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://ct.gzmigu.cn

Go:   a, b = b, a
来源：http://zu.nicolike.cn

Ruby: a, b = b, a
来源：http://zy.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://ko.jctech888.com.cn

[A20] 读取标准输入
来源：http://sj.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://nk.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mg.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ou.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://sm.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://ya.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bv.shxzskj.cn

Ruby: gets.chomp
来源：http://bq.asd995.cn

C#:   Console.ReadLine();
来源：http://uc.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://qd.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://us.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jh.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://bm.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://se.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://we.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vh.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ze.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://ci.huanxung.cn

[A22] 获取字符串长度
来源：http://oj.bjjhwx.cn

Py:   len(s)
来源：http://no.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://to.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mw.jianghongdianzi.cn

TS:   s.length
来源：http://hq.bjjhwx.cn

Java: s.length()
来源：http://se.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vv.asd995.cn

Ruby: s.length
来源：http://wx.huanxung.cn

C#:   s.Length
来源：http://nw.yuexingan06.cn

[A23] 大小写转换
来源：http://fa.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kc.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://so.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://si.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ml.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ce.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jy.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ep.chemitech.net.cn

[A24] 去除首尾空白
来源：http://ak.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qm.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lb.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://df.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ry.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mf.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://qq.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ou.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sy.9csxet.cn

[A25] 字符串比较
来源：http://px.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://ad.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vs.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ns.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zi.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lw.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iu.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sv.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dj.huixiangedu.cn

[A26] 类型转换总览
来源：http://ro.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cl.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hj.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cd.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://sr.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://er.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nf.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ht.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rw.huanxung.cn

================================================================================
来源：http://gf.chemitech.net.cn

B. 流程控制
来源：http://pp.521024.cn

================================================================================
来源：http://ss.lnxyls.cn

[B01] 条件判断 if / else
来源：http://zw.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ry.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gz.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tc.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ds.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xs.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ty.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ow.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mm.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://mj.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vs.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bu.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hu.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dt.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pi.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pw.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uz.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kb.shxzskj.cn

[B03] switch / match / case
来源：http://ov.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ll.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ck.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gh.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fp.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://la.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://da.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ox.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iq.szxytkj.cn

[B04] for 计数循环
来源：http://ub.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://js.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kx.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sm.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ge.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ml.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ky.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://op.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bd.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://lh.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://pj.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wd.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zo.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qd.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mq.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lo.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://fx.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hr.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://bm.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://np.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ht.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cm.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://am.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iv.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ek.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nk.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gv.hahajie.cn

[B07] while 循环
来源：http://vn.newstarts.cn

Py:   while i < 10: i += 1
来源：http://on.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lg.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://lx.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://sd.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://da.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ca.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://yu.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://cu.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://st.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://li.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hs.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://yc.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://kp.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://si.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ki.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ic.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://im.huanxung.cn

[B09] break 与 continue
来源：http://mb.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qe.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ek.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ic.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yj.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hp.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ef.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oq.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bs.asd995.cn

[B10] 遍历同时拿索引
来源：http://lm.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qm.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lo.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bl.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kp.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yg.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qt.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gs.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vs.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://ol.521024.cn

Py:   list(range(0, 10, 2))
来源：http://as.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://fh.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wd.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bq.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zr.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oe.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://yq.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kl.hahajie.cn

[B12] 跳出多层循环
来源：http://tp.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tx.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://to.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cm.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bh.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lv.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vj.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yq.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cm.newstarts.cn

[B13] 判断是否为数字
来源：http://ny.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://dl.lnxyls.cn

PHP:  is_numeric($x)
来源：http://jt.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kf.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yd.szxytkj.cn

Java: x instanceof Number
来源：http://ld.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rl.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://td.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://eu.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://ri.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nl.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ol.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://dm.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://tz.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ed.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fz.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eq.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tx.huanxung.cn

[B15] 布尔运算与取反
来源：http://cg.yuexingan06.cn

Py:   a and b or not c
来源：http://fb.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://uh.shxzukj.cn

JS:   a && b || !c
来源：http://aw.jianghongdianzi.cn

TS:   a && b || !c
来源：http://eq.huixinmuqiang.cn

Java: a && b || !c
来源：http://uy.lnxyls.cn

Go:   a && b || !c
来源：http://ki.hahajie.cn

Ruby: a && b || !c
来源：http://nm.colortex.cn

C#:   a && b || !c
来源：http://kj.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://th.bjjhwx.cn

Py:   if not data: return
来源：http://am.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://en.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://fx.gzmigu.cn

TS:   if (!data) return;
来源：http://ci.gzmigu.cn

Java: if (data == null) return;
来源：http://da.wgjwhj.cn

Go:   if data == nil { return }
来源：http://ik.shtwfgs.cn

Ruby: return if data.nil?
来源：http://vi.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://zr.jianghongdianzi.cn

================================================================================
来源：http://sk.nszjky.cn

C. 函数与作用域
来源：http://pr.newstarts.cn

================================================================================
来源：http://ml.shtwfgs.cn

[C01] 定义函数
来源：http://mc.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://jt.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dz.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://cm.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hm.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lk.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://po.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://kr.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ga.shxzukj.cn

[C02] 默认参数
来源：http://cq.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ta.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ja.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://zy.huixiangedu.cn


<!-- 参考信息 -->