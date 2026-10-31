代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://um.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://bk.colortex.cn

C#:   $"Hello, {name}!"
来源：http://cq.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cz.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://kf.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://tq.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://yu.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://ku.nicolike.cn

Java: "第一行\n第二行"
来源：http://oe.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ae.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://pv.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://wq.yuntaijiaju.cn

[A14] 注释写法
来源：http://mp.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ff.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lr.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://ux.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://is.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://th.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://qp.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ca.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://uo.nicolike.cn

[A15] 空值判断与默认值
来源：http://lz.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://ic.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://mo.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://nu.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://hx.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ao.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://aw.hahajie.cn

Ruby: value = data || "默认值"
来源：http://gf.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://fg.szsharing.cn

[A16] 真假值判断规则
来源：http://ij.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fw.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sm.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iq.colortex.cn

TS:   if (!x) {}
来源：http://ij.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ch.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cr.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sa.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gi.panjiajie.cn

[A17] 位运算
来源：http://mi.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uf.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sv.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gu.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yy.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bm.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fj.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kh.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://is.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://sz.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://zs.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://iz.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rc.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nf.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://nt.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sz.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://sb.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://hn.bookmarksfly.cn

[A19] 交换两个变量
来源：http://jz.jctech888.com.cn

Py:   a, b = b, a
来源：http://df.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nl.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://zt.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://tv.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://xj.9csxet.cn

Go:   a, b = b, a
来源：http://aq.9csxet.cn

Ruby: a, b = b, a
来源：http://cf.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://kq.szsharing.cn

[A20] 读取标准输入
来源：http://lf.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://qb.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wo.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zn.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://nm.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://kt.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vz.huixiangedu.cn

Ruby: gets.chomp
来源：http://aa.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://dx.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://lo.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://yu.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ok.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://xz.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://hn.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://om.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://us.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://dm.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://ib.nicolike.cn

[A22] 获取字符串长度
来源：http://ca.lnxyls.cn

Py:   len(s)
来源：http://lg.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kh.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jr.haigaiapp.cn

TS:   s.length
来源：http://uy.bookmarksfly.cn

Java: s.length()
来源：http://py.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kb.chemitech.net.cn

Ruby: s.length
来源：http://gh.huixiangedu.cn

C#:   s.Length
来源：http://ns.shtwfgs.cn

[A23] 大小写转换
来源：http://vs.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kw.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://os.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gu.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kl.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ak.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wa.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hy.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lt.panjiajie.cn

[A24] 去除首尾空白
来源：http://kz.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zc.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cw.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gx.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ku.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://da.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://ns.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vm.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pg.wgjwhj.cn

[A25] 字符串比较
来源：http://hq.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://cx.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gf.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bu.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yy.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://un.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ap.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ha.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fq.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://nl.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yu.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ef.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wo.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://qh.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xb.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://co.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ri.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uk.lnxyls.cn

================================================================================
来源：http://vk.jctech888.com.cn

B. 流程控制
来源：http://jq.yuexingan06.cn

================================================================================
来源：http://tm.lnxyls.cn

[B01] 条件判断 if / else
来源：http://xr.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vi.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tn.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hw.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ok.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wl.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ea.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gj.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qs.nicolike.cn

[B02] 多分支 else if / elif
来源：http://co.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://il.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tk.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pw.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cw.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fe.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ni.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://af.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zp.shxzukj.cn

[B03] switch / match / case
来源：http://du.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pp.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://do.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zx.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mp.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ix.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rf.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://og.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lp.lnxyls.cn

[B04] for 计数循环
来源：http://ef.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://zz.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ro.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hd.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ko.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ma.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gy.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://bt.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://js.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://nz.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://nk.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vo.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ew.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kf.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ld.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ba.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://ep.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qf.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://gg.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iw.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gy.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nu.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://go.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nj.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://po.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xp.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vx.jianghongdianzi.cn

[B07] while 循环
来源：http://kw.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://iz.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vf.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://yk.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://ol.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://kr.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dw.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://sx.521024.cn

C#:   while (i < 10) { i++; }
来源：http://ds.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://sx.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://jf.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fj.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://nz.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://ec.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://nz.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cz.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lx.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://xl.hnjuh.cn

[B09] break 与 continue
来源：http://ku.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xb.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://da.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ea.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dp.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fr.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nu.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ia.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ka.asd995.cn

[B10] 遍历同时拿索引
来源：http://of.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yt.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nc.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://by.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lz.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://op.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://px.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://po.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lc.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://yp.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://nj.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://uh.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pa.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bm.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xr.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dk.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://wm.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vx.wgjwhj.cn

[B12] 跳出多层循环
来源：http://qo.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://us.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rr.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://em.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rg.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mc.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ht.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oi.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oj.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://pg.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://lv.huanxung.cn

PHP:  is_numeric($x)
来源：http://ys.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mn.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pt.bjjhwx.cn

Java: x instanceof Number
来源：http://df.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://es.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://it.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://ut.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://eb.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ms.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://me.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://lp.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://yo.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nc.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://if.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mv.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yz.lnxyls.cn

[B15] 布尔运算与取反
来源：http://zl.lnxyls.cn

Py:   a and b or not c
来源：http://qw.nicolike.cn

PHP:  $a && $b || !$c
来源：http://pa.jianghongdianzi.cn

JS:   a && b || !c
来源：http://xk.szsharing.cn

TS:   a && b || !c
来源：http://dg.bjjhwx.cn

Java: a && b || !c
来源：http://jx.chemitech.net.cn

Go:   a && b || !c
来源：http://tq.jctech888.com.cn

Ruby: a && b || !c
来源：http://zf.521024.cn

C#:   a && b || !c
来源：http://sn.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ld.wgjwhj.cn

Py:   if not data: return
来源：http://ft.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://gb.jctech888.com.cn

JS:   if (!data) return;
来源：http://bf.hnjuh.cn

TS:   if (!data) return;
来源：http://zp.huixiangedu.cn

Java: if (data == null) return;
来源：http://ri.gzmigu.cn

Go:   if data == nil { return }
来源：http://vx.jctech888.com.cn

Ruby: return if data.nil?
来源：http://is.521024.cn

C#:   if (data == null) return;
来源：http://td.9csxet.cn

================================================================================
来源：http://qn.nicolike.cn

C. 函数与作用域
来源：http://jz.huanxung.cn

================================================================================
来源：http://oc.bjjhwx.cn

[C01] 定义函数
来源：http://aa.521024.cn

Py:   def add(a, b): return a + b
来源：http://fc.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oe.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://eg.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://id.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ki.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://or.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://xm.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eo.muxihuayi.cn

[C02] 默认参数
来源：http://ju.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://jg.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cp.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://sq.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://li.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://no.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sc.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://es.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://aj.hnjuh.cn

[C03] 可变参数
来源：http://bz.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://cw.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zo.shxzskj.cn


<!-- 参考信息 -->