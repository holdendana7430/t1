代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ag.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://mq.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://bm.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://pt.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bq.521024.cn

Ruby: "Hello, #{name}!"
来源：http://jy.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://wr.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vw.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://gk.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://ps.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://bm.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://ut.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://yi.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://ul.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://sy.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://sf.wgjwhj.cn

[A14] 注释写法
来源：http://qf.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vk.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yw.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://pi.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://ch.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://as.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://hk.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vc.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://fw.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://av.hnjuh.cn

Py:   value = data or "默认值"
来源：http://ea.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://gl.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://pk.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://xv.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xx.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://qh.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://ps.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://dr.shxzukj.cn

[A16] 真假值判断规则
来源：http://jr.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qh.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aw.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ev.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://or.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lg.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qr.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bn.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://er.shxzukj.cn

[A17] 位运算
来源：http://fe.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ke.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sa.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fe.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zd.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xc.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://do.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ko.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://li.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://hi.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://jj.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://zw.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ep.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cg.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://zl.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bm.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://hw.colortex.cn

C#:   (int)'A'; (char)65
来源：http://ow.chemitech.net.cn

[A19] 交换两个变量
来源：http://zs.szsharing.cn

Py:   a, b = b, a
来源：http://xq.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://om.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://ak.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://me.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://nl.asd995.cn

Go:   a, b = b, a
来源：http://nt.521024.cn

Ruby: a, b = b, a
来源：http://re.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://xi.panjiajie.cn

[A20] 读取标准输入
来源：http://zx.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://zc.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nv.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ll.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://bv.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://wf.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gd.nicolike.cn

Ruby: gets.chomp
来源：http://iy.hahajie.cn

C#:   Console.ReadLine();
来源：http://bn.colortex.cn

[A21] 保留指定小数位输出
来源：http://xe.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://of.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ow.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://id.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://ur.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://im.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kr.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://ab.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://ko.huixiangedu.cn

[A22] 获取字符串长度
来源：http://xf.9csxet.cn

Py:   len(s)
来源：http://hz.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lt.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sg.muxihuayi.cn

TS:   s.length
来源：http://gb.gzmigu.cn

Java: s.length()
来源：http://yr.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fp.lnxyls.cn

Ruby: s.length
来源：http://od.asd995.cn

C#:   s.Length
来源：http://jq.jctech888.com.cn

[A23] 大小写转换
来源：http://nx.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ll.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://be.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yt.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sj.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qt.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ck.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cy.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fh.lnxyls.cn

[A24] 去除首尾空白
来源：http://fb.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yt.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gx.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ad.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hm.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fp.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://de.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gn.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uw.asd995.cn

[A25] 字符串比较
来源：http://gg.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://yr.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rh.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lw.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bg.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kg.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tc.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rn.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wx.9csxet.cn

[A26] 类型转换总览
来源：http://tp.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zf.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hh.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rd.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://wq.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hp.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fi.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nz.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://or.wgjwhj.cn

================================================================================
来源：http://qd.szxytkj.cn

B. 流程控制
来源：http://gg.521024.cn

================================================================================
来源：http://yq.9csxet.cn

[B01] 条件判断 if / else
来源：http://zb.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xn.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bl.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gl.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jc.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nq.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pp.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tz.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xh.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://pu.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yn.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xa.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ui.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ek.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kk.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lv.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lg.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dz.colortex.cn

[B03] switch / match / case
来源：http://po.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qm.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ho.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sj.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ob.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nb.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hl.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sz.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sg.huixiangedu.cn

[B04] for 计数循环
来源：http://vz.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://cl.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wt.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ev.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ht.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ja.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gz.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://ri.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://br.asd995.cn

[B05] 遍历数组 / 列表
来源：http://af.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://mu.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hq.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dt.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qv.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zh.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sh.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://dm.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jk.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://io.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://es.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hp.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wi.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://el.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dk.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bb.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://or.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://od.chemitech.net.cn

[B07] while 循环
来源：http://xf.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://by.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://em.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://ka.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://le.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://cy.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mh.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://th.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://mg.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://fy.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://vf.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vd.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://yz.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://aw.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://vl.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oi.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nu.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://gj.hahajie.cn

[B09] break 与 continue
来源：http://fo.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yo.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ge.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fz.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ej.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oh.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ec.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zi.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xa.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://yc.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bs.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ln.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xq.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xj.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wy.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zs.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eg.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://eb.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://hd.colortex.cn

PHP:  range(0, 10, 2);
来源：http://ls.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gi.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://py.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tm.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ew.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://gp.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cy.521024.cn

[B12] 跳出多层循环
来源：http://ij.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hq.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gq.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cc.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xz.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ot.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dv.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sk.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ok.panjiajie.cn

[B13] 判断是否为数字
来源：http://ct.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://bv.szsharing.cn

PHP:  is_numeric($x)
来源：http://rh.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dz.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nb.yuntaijiaju.cn

Java: x instanceof Number
来源：http://kt.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yo.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://cm.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://tx.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://no.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fo.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ne.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://xg.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://jm.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hl.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eh.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qu.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fp.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://ku.shtwfgs.cn

Py:   a and b or not c
来源：http://xw.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://pq.yuexingan06.cn

JS:   a && b || !c
来源：http://xi.jctech888.com.cn

TS:   a && b || !c
来源：http://xa.shxzukj.cn

Java: a && b || !c
来源：http://up.nszjky.cn

Go:   a && b || !c
来源：http://je.szsharing.cn

Ruby: a && b || !c
来源：http://eq.colortex.cn

C#:   a && b || !c
来源：http://yo.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bx.muxihuayi.cn

Py:   if not data: return
来源：http://hw.asd995.cn

PHP:  if (!$data) { return; }
来源：http://qc.muxihuayi.cn

JS:   if (!data) return;
来源：http://cs.shxzskj.cn

TS:   if (!data) return;
来源：http://hy.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://vz.colortex.cn

Go:   if data == nil { return }
来源：http://hm.colortex.cn

Ruby: return if data.nil?
来源：http://pa.asd995.cn

C#:   if (data == null) return;
来源：http://gg.yuexingan06.cn

================================================================================
来源：http://wc.shtwfgs.cn

C. 函数与作用域
来源：http://ds.hahajie.cn

================================================================================
来源：http://md.9csxet.cn

[C01] 定义函数
来源：http://bk.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://tz.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ej.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://ps.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dh.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://km.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mz.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://bo.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://te.chemitech.net.cn

[C02] 默认参数
来源：http://ji.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://tm.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hu.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://eo.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vx.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zu.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mx.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://kf.panjiajie.cn


<!-- 参考信息 -->