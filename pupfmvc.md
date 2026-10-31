代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://iv.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rp.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://df.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://px.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dw.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nv.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://si.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ia.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://td.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://ha.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://tl.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://ly.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wq.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://ma.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://fs.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qn.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://ul.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://jy.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://fo.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://hx.9csxet.cn

Java: "第一行\n第二行"
来源：http://aq.szsharing.cn

Go:   "第一行\n第二行"
来源：http://ef.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://qf.521024.cn

C#:   "第一行\n第二行"
来源：http://rg.bookmarksfly.cn

[A14] 注释写法
来源：http://yo.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rd.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vo.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://dy.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://rb.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://re.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://ef.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://en.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://kz.asd995.cn

[A15] 空值判断与默认值
来源：http://na.lnxyls.cn

Py:   value = data or "默认值"
来源：http://ee.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://ro.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://ay.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://qz.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ma.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ho.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://ky.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://ue.nicolike.cn

[A16] 真假值判断规则
来源：http://hz.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gh.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://em.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nh.jctech888.com.cn

TS:   if (!x) {}
来源：http://bn.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ss.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kt.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nj.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qf.huixiangedu.cn

[A17] 位运算
来源：http://xd.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zf.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mj.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vm.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://am.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://di.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qu.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kb.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qf.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://it.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://jk.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://cx.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://do.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tz.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://uf.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://im.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://wo.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://yg.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://hy.shxzskj.cn

Py:   a, b = b, a
来源：http://uh.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ry.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://sw.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://mx.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://mv.shxzukj.cn

Go:   a, b = b, a
来源：http://eq.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://nv.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://wl.szxytkj.cn

[A20] 读取标准输入
来源：http://sh.hahajie.cn

Py:   name = input("请输入：")
来源：http://yx.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ns.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pt.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://il.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ja.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yd.haigaiapp.cn

Ruby: gets.chomp
来源：http://ke.nszjky.cn

C#:   Console.ReadLine();
来源：http://fr.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://fr.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://jr.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rv.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://gv.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://fc.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://cz.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ld.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://ip.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://xw.huanxung.cn

[A22] 获取字符串长度
来源：http://at.huixinmuqiang.cn

Py:   len(s)
来源：http://jy.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yv.colortex.cn

TS:   s.length
来源：http://st.shxzukj.cn

Java: s.length()
来源：http://ws.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yx.shxzskj.cn

Ruby: s.length
来源：http://qy.lnxyls.cn

C#:   s.Length
来源：http://vc.hahajie.cn

[A23] 大小写转换
来源：http://iy.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sn.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eq.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wg.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ie.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://us.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nv.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fs.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mh.huixiangedu.cn

[A24] 去除首尾空白
来源：http://xg.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pt.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ii.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eq.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ii.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ji.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://gi.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nf.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tg.panjiajie.cn

[A25] 字符串比较
来源：http://hv.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://tq.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oe.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://er.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wh.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ag.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gd.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eg.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lb.szxytkj.cn

[A26] 类型转换总览
来源：http://di.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hv.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bt.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pp.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://gr.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pf.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fo.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ow.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://po.muxihuayi.cn

================================================================================
来源：http://be.colortex.cn

B. 流程控制
来源：http://zh.colortex.cn

================================================================================
来源：http://aw.shxzukj.cn

[B01] 条件判断 if / else
来源：http://rh.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://py.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ph.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jc.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://df.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://km.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qe.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rj.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fz.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://nh.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zi.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cx.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wj.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ck.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vh.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sb.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tl.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sm.szxytkj.cn

[B03] switch / match / case
来源：http://tk.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mc.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mj.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kj.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nz.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ne.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ac.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bi.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jk.shxzskj.cn

[B04] for 计数循环
来源：http://qy.colortex.cn

Py:   for i in range(10): print(i)
来源：http://jv.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://va.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dv.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ql.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ap.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tg.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://qh.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cg.521024.cn

[B05] 遍历数组 / 列表
来源：http://hw.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://oy.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ms.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yk.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nu.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hs.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ks.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://ws.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uf.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://it.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cd.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hu.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gu.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jf.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bk.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zp.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tz.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cd.bjjhwx.cn

[B07] while 循环
来源：http://kc.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://ig.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fe.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://qf.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://nq.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://dm.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hi.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://au.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://fs.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://yn.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ex.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wk.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://le.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://fp.521024.cn

Java: do { i++; } while (i < 10);
来源：http://jb.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jd.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uu.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://ps.newstarts.cn

[B09] break 与 continue
来源：http://uv.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sr.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kt.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nm.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rn.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uv.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://td.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://la.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ql.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://gr.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rk.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wb.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gm.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ac.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://az.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yi.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cu.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xc.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://tj.521024.cn

Py:   list(range(0, 10, 2))
来源：http://wm.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://eo.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://df.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pa.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qz.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qj.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://pr.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dy.panjiajie.cn

[B12] 跳出多层循环
来源：http://fs.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vu.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://if.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ar.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wr.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gi.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pq.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ak.gzmigu.cn

[B13] 判断是否为数字
来源：http://xp.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://yq.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://ll.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ag.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mg.szxytkj.cn

Java: x instanceof Number
来源：http://br.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vx.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://as.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://en.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://ab.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ke.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wx.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://ml.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://vm.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ai.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rq.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://of.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qz.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://iy.huixinmuqiang.cn

Py:   a and b or not c
来源：http://oo.521024.cn

PHP:  $a && $b || !$c
来源：http://ej.521024.cn

JS:   a && b || !c
来源：http://mr.521024.cn

TS:   a && b || !c
来源：http://ip.hnjuh.cn

Java: a && b || !c
来源：http://ow.521024.cn

Go:   a && b || !c
来源：http://eg.hnjuh.cn

Ruby: a && b || !c
来源：http://ux.shtwfgs.cn

C#:   a && b || !c
来源：http://dl.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://my.lnxyls.cn

Py:   if not data: return
来源：http://jl.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://mi.hnjuh.cn

JS:   if (!data) return;
来源：http://lc.bookmarksfly.cn

TS:   if (!data) return;
来源：http://zq.szsharing.cn

Java: if (data == null) return;
来源：http://nl.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://tj.asd995.cn

Ruby: return if data.nil?
来源：http://kx.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://eq.hnjuh.cn

================================================================================
来源：http://jt.bookmarksfly.cn

C. 函数与作用域
来源：http://rz.lnxyls.cn

================================================================================
来源：http://ce.szxytkj.cn

[C01] 定义函数
来源：http://jd.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://hi.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mr.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://ed.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ki.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fj.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kx.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://vx.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dt.panjiajie.cn


<!-- 参考信息 -->