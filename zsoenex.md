代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://ll.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gj.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://zr.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dv.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://eo.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xf.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://ws.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mm.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yn.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://cp.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://wr.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://hg.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://re.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://ez.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://fr.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uk.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://ik.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://rr.hahajie.cn

JS:   "第一行\n第二行"
来源：http://rk.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://tf.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://xh.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://qi.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://hs.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://jc.szsharing.cn

[A14] 注释写法
来源：http://do.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qn.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kd.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://pz.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://bg.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rv.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://ij.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uj.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://gh.huanxung.cn

[A15] 空值判断与默认值
来源：http://wb.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://yd.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://ou.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://zr.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://nr.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sn.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://jx.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://fh.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://cg.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://lm.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tn.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xl.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tf.chemitech.net.cn

TS:   if (!x) {}
来源：http://kr.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nc.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nc.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fz.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eu.yuexingan06.cn

[A17] 位运算
来源：http://rf.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dn.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yx.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zr.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cm.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ib.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ov.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bx.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zg.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://yq.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://vx.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://sh.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cq.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yi.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://fm.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hw.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://sd.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://jh.nszjky.cn

[A19] 交换两个变量
来源：http://yv.wgjwhj.cn

Py:   a, b = b, a
来源：http://uf.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ui.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://av.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://rb.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://ae.jctech888.com.cn

Go:   a, b = b, a
来源：http://zq.jctech888.com.cn

Ruby: a, b = b, a
来源：http://vq.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://tv.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://lj.huanxung.cn

Py:   name = input("请输入：")
来源：http://ke.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ql.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rn.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://nx.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://fm.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wb.shxzukj.cn

Ruby: gets.chomp
来源：http://pa.gzmigu.cn

C#:   Console.ReadLine();
来源：http://pq.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://si.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://en.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://su.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://xi.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://oj.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://vw.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oy.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://rp.521024.cn

C#:   3.14159.ToString("F2")
来源：http://cs.nicolike.cn

[A22] 获取字符串长度
来源：http://gs.nicolike.cn

Py:   len(s)
来源：http://jf.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xi.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gp.newstarts.cn

TS:   s.length
来源：http://tw.szxytkj.cn

Java: s.length()
来源：http://zi.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sm.hnjuh.cn

Ruby: s.length
来源：http://fk.gzmigu.cn

C#:   s.Length
来源：http://ww.shtwfgs.cn

[A23] 大小写转换
来源：http://mz.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rj.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xf.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ta.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ly.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kc.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xb.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mf.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nt.szxytkj.cn

[A24] 去除首尾空白
来源：http://xu.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ae.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pd.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tk.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dt.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ch.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://ro.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qq.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cj.nicolike.cn

[A25] 字符串比较
来源：http://qi.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://zm.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ln.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rs.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nh.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qe.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://st.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zx.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fc.huixiangedu.cn

[A26] 类型转换总览
来源：http://qy.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tb.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kr.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sn.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://tl.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gy.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://du.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://na.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mv.huanxung.cn

================================================================================
来源：http://fh.newstarts.cn

B. 流程控制
来源：http://rl.yuntaijiaju.cn

================================================================================
来源：http://fz.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://qy.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ft.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pe.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://md.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ns.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ss.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rz.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pp.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mx.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://ev.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ay.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://li.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sy.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tv.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rr.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zs.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qq.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uw.shtwfgs.cn

[B03] switch / match / case
来源：http://oh.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ev.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ni.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ni.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ww.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dm.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dm.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ju.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://br.huanxung.cn

[B04] for 计数循环
来源：http://yz.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://pn.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vy.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nv.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zw.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wu.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dy.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://rs.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mo.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://go.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://ae.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xw.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jx.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ae.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ji.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nc.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://mi.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cz.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://ak.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mq.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lv.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yt.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nf.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yv.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://we.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lb.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ni.bookmarksfly.cn

[B07] while 循环
来源：http://nw.nszjky.cn

Py:   while i < 10: i += 1
来源：http://da.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tm.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://fy.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://vb.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://vk.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uk.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://iu.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://iz.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://cv.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://xc.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pq.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://mz.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://qo.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://ko.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ya.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xy.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://ii.9csxet.cn

[B09] break 与 continue
来源：http://ua.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gj.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ll.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rp.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zz.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qv.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://px.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nr.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mh.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://fv.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sp.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://be.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://km.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tf.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rt.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sa.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nx.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vu.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://rg.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://ey.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://it.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ed.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cn.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hb.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pl.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://eu.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://su.nszjky.cn

[B12] 跳出多层循环
来源：http://vt.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wn.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gd.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qb.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://md.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sv.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://er.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bk.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hq.colortex.cn

[B13] 判断是否为数字
来源：http://hd.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://vw.nszjky.cn

PHP:  is_numeric($x)
来源：http://rg.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tu.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jq.colortex.cn

Java: x instanceof Number
来源：http://gi.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cq.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://lr.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://ry.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://xn.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tu.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eu.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://qx.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ji.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ip.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fp.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tb.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ab.colortex.cn

[B15] 布尔运算与取反
来源：http://bs.bookmarksfly.cn

Py:   a and b or not c
来源：http://nb.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ka.newstarts.cn

JS:   a && b || !c
来源：http://af.jianghongdianzi.cn

TS:   a && b || !c
来源：http://vw.colortex.cn

Java: a && b || !c
来源：http://ih.shtwfgs.cn

Go:   a && b || !c
来源：http://kh.9csxet.cn

Ruby: a && b || !c
来源：http://bx.yuexingan06.cn

C#:   a && b || !c
来源：http://cl.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yh.9csxet.cn

Py:   if not data: return
来源：http://ju.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://fi.newstarts.cn

JS:   if (!data) return;
来源：http://dd.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://hg.yuexingan06.cn

Java: if (data == null) return;
来源：http://bj.muxihuayi.cn

Go:   if data == nil { return }
来源：http://ey.chemitech.net.cn

Ruby: return if data.nil?
来源：http://io.colortex.cn

C#:   if (data == null) return;
来源：http://sy.szsharing.cn

================================================================================
来源：http://rf.hnjuh.cn

C. 函数与作用域
来源：http://fb.asd995.cn

================================================================================
来源：http://hv.szxytkj.cn

[C01] 定义函数
来源：http://ab.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://mh.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sq.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ms.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lf.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eb.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://um.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://vj.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qw.yuntaijiaju.cn


<!-- 参考信息 -->