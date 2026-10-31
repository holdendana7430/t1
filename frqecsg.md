代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://lr.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bc.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://uj.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mn.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://td.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://sm.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://xz.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://en.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rb.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://fk.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://jj.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vw.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://ra.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://il.huanxung.cn

JS:   "第一行\n第二行"
来源：http://uj.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://yb.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://cj.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://at.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://yg.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://eh.nszjky.cn

[A14] 注释写法
来源：http://pz.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xf.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xw.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://dt.521024.cn

TS:   // 单行；/* 多行 */
来源：http://tp.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vw.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://cl.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kb.521024.cn

C#:   // 单行；/* 多行 */
来源：http://me.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://ff.hnjuh.cn

Py:   value = data or "默认值"
来源：http://ax.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://tg.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://up.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://nc.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hs.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://jr.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://yj.521024.cn

C#:   var value = data ?? "默认值";
来源：http://zp.chemitech.net.cn

[A16] 真假值判断规则
来源：http://ln.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kp.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ot.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lh.shxzukj.cn

TS:   if (!x) {}
来源：http://xo.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vf.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ne.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ts.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vf.newstarts.cn

[A17] 位运算
来源：http://kk.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ft.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qt.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ak.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ep.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dr.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ey.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yb.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pw.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://wn.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://gb.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://lf.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bf.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kg.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://oe.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yf.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://xr.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://xy.bjjhwx.cn

[A19] 交换两个变量
来源：http://ba.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://uk.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qd.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://kf.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://pc.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://jf.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://gm.szsharing.cn

Ruby: a, b = b, a
来源：http://zx.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://zu.9csxet.cn

[A20] 读取标准输入
来源：http://oa.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://mr.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ge.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wb.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://ui.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://to.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ye.9csxet.cn

Ruby: gets.chomp
来源：http://vv.colortex.cn

C#:   Console.ReadLine();
来源：http://vu.hahajie.cn

[A21] 保留指定小数位输出
来源：http://wq.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://xw.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sf.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://jd.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://wc.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://zh.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mz.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://bi.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://zc.szsharing.cn

[A22] 获取字符串长度
来源：http://ca.huanxung.cn

Py:   len(s)
来源：http://kj.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tc.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://an.szsharing.cn

TS:   s.length
来源：http://gm.shtwfgs.cn

Java: s.length()
来源：http://ak.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cq.9csxet.cn

Ruby: s.length
来源：http://ms.lnxyls.cn

C#:   s.Length
来源：http://xm.szxytkj.cn

[A23] 大小写转换
来源：http://ar.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bw.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hd.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hy.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gx.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kd.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ft.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mq.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ru.hahajie.cn

[A24] 去除首尾空白
来源：http://fb.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wf.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zz.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ho.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ly.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xd.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://qx.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yc.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sb.521024.cn

[A25] 字符串比较
来源：http://eb.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://ad.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kh.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mc.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qf.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bm.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bg.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tp.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hg.muxihuayi.cn

[A26] 类型转换总览
来源：http://wm.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lq.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zs.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nq.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://xt.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bq.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nm.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xb.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cq.haigaiapp.cn

================================================================================
来源：http://np.gzmigu.cn

B. 流程控制
来源：http://ra.huanxung.cn

================================================================================
来源：http://kq.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://tm.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fp.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sa.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rb.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hr.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iu.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pm.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vh.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zm.szsharing.cn

[B02] 多分支 else if / elif
来源：http://ut.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ip.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jq.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://su.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://me.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qw.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ac.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kx.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qq.hahajie.cn

[B03] switch / match / case
来源：http://cd.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ye.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gv.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wd.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mo.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vl.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gi.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nm.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zi.lnxyls.cn

[B04] for 计数循环
来源：http://rx.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://gv.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fn.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ku.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vk.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dx.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://re.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://cq.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nr.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://rk.newstarts.cn

Py:   for item in arr: print(item)
来源：http://zt.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tv.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fi.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ih.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xv.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://st.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://bc.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ji.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://tl.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vl.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ei.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lk.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ow.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oa.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://se.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sc.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vl.hnjuh.cn

[B07] while 循环
来源：http://av.nicolike.cn

Py:   while i < 10: i += 1
来源：http://vt.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jy.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://vo.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://vg.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://et.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fo.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://dj.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://wx.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://or.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://yq.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aw.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://cs.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://gv.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://ax.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ia.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://od.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://wx.9csxet.cn

[B09] break 与 continue
来源：http://aa.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jb.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ss.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hs.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://md.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://do.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rp.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vz.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dp.szsharing.cn

[B10] 遍历同时拿索引
来源：http://kf.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hy.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hs.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ko.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iu.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ky.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zo.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tz.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zk.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://lr.521024.cn

Py:   list(range(0, 10, 2))
来源：http://hc.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://zo.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ag.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zv.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ek.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wh.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://zt.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qh.szsharing.cn

[B12] 跳出多层循环
来源：http://ek.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wt.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bx.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zk.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ga.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kw.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tc.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://np.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ud.haigaiapp.cn

[B13] 判断是否为数字
来源：http://wt.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://yq.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://qy.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ev.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pj.gzmigu.cn

Java: x instanceof Number
来源：http://dq.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gc.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://zq.shxzukj.cn

C#:   x is int or double or decimal
来源：http://je.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://bx.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yj.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bb.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://xx.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://dm.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ig.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qz.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yj.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wh.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://lf.9csxet.cn

Py:   a and b or not c
来源：http://og.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://um.huixiangedu.cn

JS:   a && b || !c
来源：http://lz.gzmigu.cn

TS:   a && b || !c
来源：http://gh.haigaiapp.cn

Java: a && b || !c
来源：http://lz.wgjwhj.cn

Go:   a && b || !c
来源：http://ni.lnxyls.cn

Ruby: a && b || !c
来源：http://oo.szsharing.cn

C#:   a && b || !c
来源：http://do.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ne.wgjwhj.cn

Py:   if not data: return
来源：http://gn.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://aj.shtwfgs.cn

JS:   if (!data) return;
来源：http://iq.shxzskj.cn

TS:   if (!data) return;
来源：http://jg.bookmarksfly.cn

Java: if (data == null) return;
来源：http://wt.shtwfgs.cn

Go:   if data == nil { return }
来源：http://jv.newstarts.cn

Ruby: return if data.nil?
来源：http://io.newstarts.cn

C#:   if (data == null) return;
来源：http://tp.szxytkj.cn

================================================================================
来源：http://jx.asd995.cn

C. 函数与作用域
来源：http://sd.colortex.cn

================================================================================
来源：http://qv.colortex.cn

[C01] 定义函数
来源：http://xx.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://at.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hq.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://nh.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gi.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wm.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sj.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://ok.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ka.gzmigu.cn

[C02] 默认参数
来源：http://jo.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://th.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ku.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://nv.bookmarksfly.cn


<!-- 参考信息 -->