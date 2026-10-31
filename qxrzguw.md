代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://sf.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ly.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://vb.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ok.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hg.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://lm.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://lm.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://of.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vq.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://sc.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://mz.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ql.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://zu.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://mi.hahajie.cn

JS:   "第一行\n第二行"
来源：http://xh.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://jt.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://pd.asd995.cn

Go:   "第一行\n第二行"
来源：http://jx.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://sq.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://wk.muxihuayi.cn

[A14] 注释写法
来源：http://fm.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qa.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sp.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://hj.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://ll.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qu.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://cx.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pk.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://uu.hahajie.cn

[A15] 空值判断与默认值
来源：http://eo.asd995.cn

Py:   value = data or "默认值"
来源：http://qd.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://vh.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://zg.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://kr.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pe.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://os.huanxung.cn

Ruby: value = data || "默认值"
来源：http://qa.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://zc.muxihuayi.cn

[A16] 真假值判断规则
来源：http://vg.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cm.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://df.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zo.asd995.cn

TS:   if (!x) {}
来源：http://sm.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bf.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mj.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://md.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uj.yuexingan06.cn

[A17] 位运算
来源：http://jg.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ox.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://on.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ql.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zz.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cu.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nw.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ts.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iu.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://sd.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://fj.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://jm.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tp.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jn.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://zq.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ff.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://vm.521024.cn

C#:   (int)'A'; (char)65
来源：http://pj.521024.cn

[A19] 交换两个变量
来源：http://rh.hnjuh.cn

Py:   a, b = b, a
来源：http://hx.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://np.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://lk.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://ol.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://cf.asd995.cn

Go:   a, b = b, a
来源：http://hx.muxihuayi.cn

Ruby: a, b = b, a
来源：http://lf.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://ji.hahajie.cn

[A20] 读取标准输入
来源：http://ip.szxytkj.cn

Py:   name = input("请输入：")
来源：http://cs.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wl.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://st.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://us.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://go.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gy.newstarts.cn

Ruby: gets.chomp
来源：http://rf.nicolike.cn

C#:   Console.ReadLine();
来源：http://dc.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://fm.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://wq.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yf.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://bo.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://np.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://bq.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kw.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://zb.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://wb.szxytkj.cn

[A22] 获取字符串长度
来源：http://jl.yuexingan06.cn

Py:   len(s)
来源：http://sr.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xs.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pt.szsharing.cn

TS:   s.length
来源：http://uw.hnjuh.cn

Java: s.length()
来源：http://ke.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zh.jianghongdianzi.cn

Ruby: s.length
来源：http://px.521024.cn

C#:   s.Length
来源：http://qo.lnxyls.cn

[A23] 大小写转换
来源：http://je.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pp.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gg.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dp.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gn.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eq.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wl.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fx.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xx.muxihuayi.cn

[A24] 去除首尾空白
来源：http://iq.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://es.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nb.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ky.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wh.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ku.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://fi.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lo.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rz.szsharing.cn

[A25] 字符串比较
来源：http://ii.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://hs.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qv.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lo.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xj.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dn.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bd.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rx.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jd.huixiangedu.cn

[A26] 类型转换总览
来源：http://sx.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vv.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vt.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zf.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://wg.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ku.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nu.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oc.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iv.asd995.cn

================================================================================
来源：http://nz.yuntaijiaju.cn

B. 流程控制
来源：http://nz.huixiangedu.cn

================================================================================
来源：http://qv.huanxung.cn

[B01] 条件判断 if / else
来源：http://fx.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eh.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dd.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kx.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ka.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zm.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ap.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ba.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uh.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://km.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xj.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rt.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://us.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://av.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wv.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://em.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://as.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://te.huanxung.cn

[B03] switch / match / case
来源：http://yf.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xe.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mp.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vv.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uz.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sp.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://od.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tu.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pn.hahajie.cn

[B04] for 计数循环
来源：http://tj.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://mm.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ju.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mk.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iw.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mr.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nd.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://db.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ke.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://dg.colortex.cn

Py:   for item in arr: print(item)
来源：http://fs.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nv.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rn.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cl.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://km.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wi.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://fn.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wo.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://cm.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ed.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://az.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fn.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qu.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nl.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xc.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vd.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ql.bjjhwx.cn

[B07] while 循环
来源：http://ik.hahajie.cn

Py:   while i < 10: i += 1
来源：http://xa.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xn.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://in.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://ix.asd995.cn

Java: while (i < 10) { i++; }
来源：http://rt.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cf.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://vu.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://nh.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://ln.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://fk.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pr.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://ik.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://cc.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://iw.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zn.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bs.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://nk.chemitech.net.cn

[B09] break 与 continue
来源：http://ze.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kl.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://td.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ra.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xr.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ki.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pn.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bd.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zy.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://bt.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://to.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nn.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mg.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ql.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hy.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uh.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://az.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jm.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://mj.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://aj.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://ws.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jy.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jf.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jy.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qr.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://qi.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://na.colortex.cn

[B12] 跳出多层循环
来源：http://ip.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tq.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gy.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cm.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jz.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xk.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mk.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://is.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ut.huixiangedu.cn

[B13] 判断是否为数字
来源：http://ai.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://qu.gzmigu.cn

PHP:  is_numeric($x)
来源：http://ts.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ne.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zf.bookmarksfly.cn

Java: x instanceof Number
来源：http://qo.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ls.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://yx.shxzskj.cn

C#:   x is int or double or decimal
来源：http://df.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://pu.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ed.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kn.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://uj.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://lq.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://un.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gu.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jz.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fi.huanxung.cn

[B15] 布尔运算与取反
来源：http://wc.hahajie.cn

Py:   a and b or not c
来源：http://ea.521024.cn

PHP:  $a && $b || !$c
来源：http://qd.521024.cn

JS:   a && b || !c
来源：http://gc.newstarts.cn

TS:   a && b || !c
来源：http://xx.9csxet.cn

Java: a && b || !c
来源：http://be.hnjuh.cn

Go:   a && b || !c
来源：http://ey.szsharing.cn

Ruby: a && b || !c
来源：http://ud.jianghongdianzi.cn

C#:   a && b || !c
来源：http://gd.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xv.chemitech.net.cn

Py:   if not data: return
来源：http://nt.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://qg.jctech888.com.cn

JS:   if (!data) return;
来源：http://wo.hnjuh.cn

TS:   if (!data) return;
来源：http://me.jctech888.com.cn

Java: if (data == null) return;
来源：http://ul.9csxet.cn

Go:   if data == nil { return }
来源：http://fm.gzmigu.cn

Ruby: return if data.nil?
来源：http://mp.bjjhwx.cn

C#:   if (data == null) return;
来源：http://oa.lnxyls.cn

================================================================================
来源：http://wt.szsharing.cn

C. 函数与作用域
来源：http://pu.yuntaijiaju.cn

================================================================================
来源：http://gf.wgjwhj.cn

[C01] 定义函数
来源：http://qp.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://jj.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gc.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://qy.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fu.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://no.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bx.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://nd.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dj.shxzskj.cn

[C02] 默认参数
来源：http://tx.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://uv.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ny.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://bl.yuntaijiaju.cn


<!-- 参考信息 -->