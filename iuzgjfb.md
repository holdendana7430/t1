代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ep.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://tm.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://qb.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bb.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://ob.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://ai.colortex.cn

JS:   "第一行\n第二行"
来源：http://yi.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://bu.hahajie.cn

Java: "第一行\n第二行"
来源：http://dc.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://nu.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://nn.newstarts.cn

C#:   "第一行\n第二行"
来源：http://kt.yuexingan06.cn

[A14] 注释写法
来源：http://wf.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://un.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zy.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://zt.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://um.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zm.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://ay.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yu.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://ez.nszjky.cn

[A15] 空值判断与默认值
来源：http://pi.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://sm.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://zu.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://lp.521024.cn

TS:   const value = data ?? "默认值";
来源：http://ve.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cz.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://uc.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://kx.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://ke.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://dr.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lt.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kt.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oi.nicolike.cn

TS:   if (!x) {}
来源：http://ib.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jq.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bo.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yz.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xb.muxihuayi.cn

[A17] 位运算
来源：http://cn.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xu.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://az.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ov.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://it.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ut.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cs.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rv.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://px.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://kl.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://xl.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://bx.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vb.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zr.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://ip.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ch.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://zm.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://gr.colortex.cn

[A19] 交换两个变量
来源：http://sx.wgjwhj.cn

Py:   a, b = b, a
来源：http://zy.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lv.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://ki.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://cv.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://hf.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://up.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://jy.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://ir.jctech888.com.cn

[A20] 读取标准输入
来源：http://uj.huanxung.cn

Py:   name = input("请输入：")
来源：http://by.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ee.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gg.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://ls.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ur.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nw.shxzskj.cn

Ruby: gets.chomp
来源：http://qg.asd995.cn

C#:   Console.ReadLine();
来源：http://vg.colortex.cn

[A21] 保留指定小数位输出
来源：http://sc.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://vh.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mp.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://ml.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://bj.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ib.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lz.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://qt.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://wg.panjiajie.cn

[A22] 获取字符串长度
来源：http://lq.newstarts.cn

Py:   len(s)
来源：http://vx.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eb.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ip.lnxyls.cn

TS:   s.length
来源：http://nj.hnjuh.cn

Java: s.length()
来源：http://ik.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hs.asd995.cn

Ruby: s.length
来源：http://fg.yuexingan06.cn

C#:   s.Length
来源：http://vn.hahajie.cn

[A23] 大小写转换
来源：http://hl.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ml.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vj.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zg.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vk.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zv.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yx.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vt.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xi.9csxet.cn

[A24] 去除首尾空白
来源：http://mt.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hx.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jd.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://at.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zq.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://px.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://tx.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sc.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nj.521024.cn

[A25] 字符串比较
来源：http://pi.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://ug.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fy.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xp.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mh.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sp.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://de.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ex.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hs.bjjhwx.cn

[A26] 类型转换总览
来源：http://oc.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eu.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fb.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sh.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://jt.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ya.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mj.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cs.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fm.panjiajie.cn

================================================================================
来源：http://bi.nszjky.cn

B. 流程控制
来源：http://tz.asd995.cn

================================================================================
来源：http://nk.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://uz.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oi.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bg.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tw.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gx.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vb.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xr.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ez.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oo.colortex.cn

[B02] 多分支 else if / elif
来源：http://uj.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jc.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wp.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bf.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ex.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lh.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dl.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gn.asd995.cn

[B03] switch / match / case
来源：http://rq.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bl.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dj.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yo.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://am.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rv.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uc.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ze.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hf.haigaiapp.cn

[B04] for 计数循环
来源：http://uf.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://ah.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aj.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xz.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cd.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ah.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lt.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://ao.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yh.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://kd.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://zx.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vd.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xa.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pt.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uh.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://le.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://ju.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oj.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://sx.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sp.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wp.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eb.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qm.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kh.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://es.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ca.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wd.shxzskj.cn

[B07] while 循环
来源：http://ln.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://sv.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ga.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://qz.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://dr.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://ev.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ha.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://rt.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://qz.asd995.cn

[B08] do-while（至少执行一次）
来源：http://tb.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://iz.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jx.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://cn.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://md.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://kh.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wu.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fc.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://ce.muxihuayi.cn

[B09] break 与 continue
来源：http://to.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bp.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sd.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fr.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lv.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ns.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ij.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xz.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xq.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://xq.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rw.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eu.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zz.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ow.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ma.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ko.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qe.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uv.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://gb.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://xa.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://jw.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yi.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oz.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rb.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sd.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://wc.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xb.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://in.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ta.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yu.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://re.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ub.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ru.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wm.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sb.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sc.lnxyls.cn

[B13] 判断是否为数字
来源：http://ab.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://be.szxytkj.cn

PHP:  is_numeric($x)
来源：http://yj.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cs.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fc.huanxung.cn

Java: x instanceof Number
来源：http://fr.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hv.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://ur.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://wq.9csxet.cn

[B14] 判断值是否在集合内
来源：http://fs.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yb.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xj.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://jk.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://zy.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kv.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uf.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kn.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cq.shxzskj.cn

[B15] 布尔运算与取反
来源：http://nv.9csxet.cn

Py:   a and b or not c
来源：http://qc.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ih.szsharing.cn

JS:   a && b || !c
来源：http://hr.chemitech.net.cn

TS:   a && b || !c
来源：http://ui.asd995.cn

Java: a && b || !c
来源：http://ru.panjiajie.cn

Go:   a && b || !c
来源：http://od.panjiajie.cn

Ruby: a && b || !c
来源：http://ox.bjjhwx.cn

C#:   a && b || !c
来源：http://ej.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://og.haigaiapp.cn

Py:   if not data: return
来源：http://al.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://uj.szxytkj.cn

JS:   if (!data) return;
来源：http://ck.huixiangedu.cn

TS:   if (!data) return;
来源：http://lq.nicolike.cn

Java: if (data == null) return;
来源：http://oz.gzmigu.cn

Go:   if data == nil { return }
来源：http://fh.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://yd.haigaiapp.cn

C#:   if (data == null) return;
来源：http://li.szsharing.cn

================================================================================
来源：http://yd.panjiajie.cn

C. 函数与作用域
来源：http://kh.chemitech.net.cn

================================================================================
来源：http://zw.hahajie.cn

[C01] 定义函数
来源：http://ss.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://rb.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kf.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://vf.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xc.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jk.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bw.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://nj.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ky.yuexingan06.cn

[C02] 默认参数
来源：http://mi.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://kb.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fr.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://ce.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qz.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zd.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sf.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://mu.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://nq.jianghongdianzi.cn

[C03] 可变参数
来源：http://zs.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://qq.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ia.wgjwhj.cn


<!-- 参考信息 -->