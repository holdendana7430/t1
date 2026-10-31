代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bk.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://sf.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://ar.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://xn.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yr.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://mv.colortex.cn

C#:   $"Hello, {name}!"
来源：http://wa.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pg.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://vc.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://nf.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://im.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://mh.9csxet.cn

Java: "第一行\n第二行"
来源：http://it.szsharing.cn

Go:   "第一行\n第二行"
来源：http://yp.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://eo.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://aa.lnxyls.cn

[A14] 注释写法
来源：http://kk.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cx.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mb.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://dw.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://rw.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ji.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://me.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://am.521024.cn

C#:   // 单行；/* 多行 */
来源：http://rk.colortex.cn

[A15] 空值判断与默认值
来源：http://gf.9csxet.cn

Py:   value = data or "默认值"
来源：http://wu.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://sk.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://cn.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://hf.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zz.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://zp.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://ok.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://wa.muxihuayi.cn

[A16] 真假值判断规则
来源：http://mr.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sa.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ij.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lc.shxzskj.cn

TS:   if (!x) {}
来源：http://iw.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vd.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://on.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hc.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ls.huixinmuqiang.cn

[A17] 位运算
来源：http://xy.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fr.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zq.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ki.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ue.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rk.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pa.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dt.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://ur.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://sm.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://mv.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ni.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hm.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://ac.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://co.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://ki.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://ua.9csxet.cn

[A19] 交换两个变量
来源：http://ds.asd995.cn

Py:   a, b = b, a
来源：http://ge.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oi.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://zh.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://bx.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://hk.newstarts.cn

Go:   a, b = b, a
来源：http://xg.521024.cn

Ruby: a, b = b, a
来源：http://np.asd995.cn

C#:   (a, b) = (b, a);
来源：http://bk.hnjuh.cn

[A20] 读取标准输入
来源：http://jf.nszjky.cn

Py:   name = input("请输入：")
来源：http://dg.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://td.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gy.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://wq.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://qo.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hd.chemitech.net.cn

Ruby: gets.chomp
来源：http://rq.nicolike.cn

C#:   Console.ReadLine();
来源：http://ey.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://pu.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://xb.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iw.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://rh.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://jd.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://zb.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qn.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://oq.521024.cn

C#:   3.14159.ToString("F2")
来源：http://oy.huixiangedu.cn

[A22] 获取字符串长度
来源：http://sd.bjjhwx.cn

Py:   len(s)
来源：http://vt.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rh.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ed.szsharing.cn

TS:   s.length
来源：http://pk.huanxung.cn

Java: s.length()
来源：http://gl.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vl.521024.cn

Ruby: s.length
来源：http://jc.colortex.cn

C#:   s.Length
来源：http://bf.muxihuayi.cn

[A23] 大小写转换
来源：http://ea.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pd.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cn.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eb.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oz.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://md.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qt.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xr.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nq.huanxung.cn

[A24] 去除首尾空白
来源：http://tx.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ck.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pu.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vu.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aj.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ba.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://sh.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rn.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sx.bookmarksfly.cn

[A25] 字符串比较
来源：http://jz.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://as.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iu.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ax.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uo.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wi.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tt.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oi.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://os.wgjwhj.cn

[A26] 类型转换总览
来源：http://md.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xd.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yz.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vv.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://nv.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uf.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pe.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lt.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://le.bjjhwx.cn

================================================================================
来源：http://kr.gzmigu.cn

B. 流程控制
来源：http://pq.huanxung.cn

================================================================================
来源：http://xx.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://qu.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hc.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://le.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tp.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cc.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vm.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sa.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ft.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xw.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://yo.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mz.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fu.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uk.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dq.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dl.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://po.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zx.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cs.9csxet.cn

[B03] switch / match / case
来源：http://cv.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gg.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rp.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dd.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rp.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tz.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rm.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gh.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ge.lnxyls.cn

[B04] for 计数循环
来源：http://ao.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://zw.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://li.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jg.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uu.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qh.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://za.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://eu.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lm.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://sp.huanxung.cn

Py:   for item in arr: print(item)
来源：http://bn.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ud.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qg.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://db.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lv.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wu.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://ba.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tc.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://aj.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fg.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://up.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bg.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hp.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://id.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ry.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sk.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dv.shxzskj.cn

[B07] while 循环
来源：http://xk.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://nx.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uz.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://lh.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://tp.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://be.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://am.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://dz.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://hd.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://md.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://db.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aj.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://jb.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://wh.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://qz.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oo.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sz.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://ph.bookmarksfly.cn

[B09] break 与 continue
来源：http://ck.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ie.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qk.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://si.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qm.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aq.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cl.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ic.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ol.colortex.cn

[B10] 遍历同时拿索引
来源：http://sw.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nh.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vm.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ms.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ti.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uz.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qo.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kl.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qy.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://kn.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://qr.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://ur.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oc.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pf.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dp.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xx.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://vz.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nm.yuexingan06.cn

[B12] 跳出多层循环
来源：http://ce.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xz.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sq.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fx.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mm.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qk.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lq.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nr.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hd.szsharing.cn

[B13] 判断是否为数字
来源：http://xq.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://th.shxzukj.cn

PHP:  is_numeric($x)
来源：http://kd.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://os.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qm.panjiajie.cn

Java: x instanceof Number
来源：http://nc.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pm.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://bk.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://xu.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://qr.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zv.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://db.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://hu.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://rk.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eb.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yx.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nu.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hg.newstarts.cn

[B15] 布尔运算与取反
来源：http://md.szsharing.cn

Py:   a and b or not c
来源：http://gt.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://wh.haigaiapp.cn

JS:   a && b || !c
来源：http://lu.muxihuayi.cn

TS:   a && b || !c
来源：http://px.haigaiapp.cn

Java: a && b || !c
来源：http://tx.wgjwhj.cn

Go:   a && b || !c
来源：http://cj.szsharing.cn

Ruby: a && b || !c
来源：http://ur.huixiangedu.cn

C#:   a && b || !c
来源：http://mf.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zu.521024.cn

Py:   if not data: return
来源：http://jv.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://cl.haigaiapp.cn

JS:   if (!data) return;
来源：http://rf.chemitech.net.cn

TS:   if (!data) return;
来源：http://dx.hnjuh.cn

Java: if (data == null) return;
来源：http://xy.wgjwhj.cn

Go:   if data == nil { return }
来源：http://bd.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://sc.chemitech.net.cn

C#:   if (data == null) return;
来源：http://vw.panjiajie.cn

================================================================================
来源：http://to.lnxyls.cn

C. 函数与作用域
来源：http://rt.nszjky.cn

================================================================================
来源：http://rj.haigaiapp.cn

[C01] 定义函数
来源：http://pq.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://nc.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iw.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://rh.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eq.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cx.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zf.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://cm.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rq.jctech888.com.cn

[C02] 默认参数
来源：http://ri.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://vl.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://km.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://eo.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eh.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ma.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ld.521024.cn

Ruby: def greet(name = "World") = name
来源：http://dz.jianghongdianzi.cn


<!-- 参考信息 -->