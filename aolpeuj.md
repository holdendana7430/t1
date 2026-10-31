代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dt.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://nx.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://lj.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://up.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ym.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://hc.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://nq.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dq.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://wd.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://dd.nszjky.cn

JS:   "第一行\n第二行"
来源：http://nz.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://kg.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://mn.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://ez.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://sq.hahajie.cn

C#:   "第一行\n第二行"
来源：http://kq.nicolike.cn

[A14] 注释写法
来源：http://ow.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pm.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bz.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://lo.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://zm.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zj.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://tp.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zq.521024.cn

C#:   // 单行；/* 多行 */
来源：http://ag.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://hz.newstarts.cn

Py:   value = data or "默认值"
来源：http://bw.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://gj.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://ri.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://ln.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tb.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://zh.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://kr.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://tp.lnxyls.cn

[A16] 真假值判断规则
来源：http://qx.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gd.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dx.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vh.521024.cn

TS:   if (!x) {}
来源：http://mh.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zd.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kg.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cf.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bj.yuntaijiaju.cn

[A17] 位运算
来源：http://ki.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fr.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cd.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ti.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ns.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tc.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cb.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ue.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hn.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://zp.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://dm.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://or.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xp.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zc.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://bt.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rh.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://gh.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://in.asd995.cn

[A19] 交换两个变量
来源：http://pj.gzmigu.cn

Py:   a, b = b, a
来源：http://bu.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yh.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://kg.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://pq.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://it.shxzskj.cn

Go:   a, b = b, a
来源：http://vo.huixiangedu.cn

Ruby: a, b = b, a
来源：http://cc.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://xe.shxzukj.cn

[A20] 读取标准输入
来源：http://iw.colortex.cn

Py:   name = input("请输入：")
来源：http://fi.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yw.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vf.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://wc.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://fj.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ej.shxzskj.cn

Ruby: gets.chomp
来源：http://pj.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://ak.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://st.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://nz.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://um.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://vt.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://ha.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://de.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://we.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ip.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://ln.panjiajie.cn

[A22] 获取字符串长度
来源：http://xu.shxzskj.cn

Py:   len(s)
来源：http://rx.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ie.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rw.haigaiapp.cn

TS:   s.length
来源：http://wn.jianghongdianzi.cn

Java: s.length()
来源：http://zi.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://de.shxzskj.cn

Ruby: s.length
来源：http://zx.colortex.cn

C#:   s.Length
来源：http://wv.jianghongdianzi.cn

[A23] 大小写转换
来源：http://eq.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tv.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jz.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wu.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kz.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tv.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sv.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pj.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uz.hahajie.cn

[A24] 去除首尾空白
来源：http://td.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aa.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nq.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nk.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ny.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zx.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://ya.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sn.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kr.yuexingan06.cn

[A25] 字符串比较
来源：http://ah.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://ui.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qq.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kx.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dp.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://le.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lk.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fi.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ul.shtwfgs.cn

[A26] 类型转换总览
来源：http://pq.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oa.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jg.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uz.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://rj.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ri.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bc.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pl.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ns.szxytkj.cn

================================================================================
来源：http://wq.wgjwhj.cn

B. 流程控制
来源：http://zo.nszjky.cn

================================================================================
来源：http://cc.huanxung.cn

[B01] 条件判断 if / else
来源：http://bo.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cx.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vm.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gg.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xw.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rm.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iw.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yd.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ae.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://az.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eb.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uq.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ut.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eo.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://of.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qh.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vk.shtwfgs.cn

[B03] switch / match / case
来源：http://wn.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tq.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bb.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qx.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://el.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://og.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jj.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eq.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://od.9csxet.cn

[B04] for 计数循环
来源：http://bg.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://rb.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wv.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tz.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ko.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eq.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xp.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://vi.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dv.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://tr.521024.cn

Py:   for item in arr: print(item)
来源：http://ht.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wc.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qb.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ih.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uk.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lt.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://ax.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vh.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://iy.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wf.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://el.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uh.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ny.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qn.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yt.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qp.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uu.nszjky.cn

[B07] while 循环
来源：http://kh.521024.cn

Py:   while i < 10: i += 1
来源：http://ex.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yu.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://yg.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://sp.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://nq.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vp.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://no.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://pz.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://vy.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://ym.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fp.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://ds.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://id.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://ur.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wj.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jz.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://hk.chemitech.net.cn

[B09] break 与 continue
来源：http://pc.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://re.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://up.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://di.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sl.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://od.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zf.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bt.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wq.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://gm.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pp.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nx.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oa.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pe.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kz.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kk.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://si.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fi.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://dj.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://zj.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://ye.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zz.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vz.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qw.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ti.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://ln.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wq.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://nh.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://he.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eo.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sm.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hx.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uh.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ry.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uv.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ju.szsharing.cn

[B13] 判断是否为数字
来源：http://em.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://lu.shxzskj.cn

PHP:  is_numeric($x)
来源：http://xn.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ca.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hx.hnjuh.cn

Java: x instanceof Number
来源：http://kn.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hd.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://ev.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://cr.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://pf.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://in.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qx.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://el.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://xi.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kg.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://st.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mb.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ej.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://jc.haigaiapp.cn

Py:   a and b or not c
来源：http://bh.szsharing.cn

PHP:  $a && $b || !$c
来源：http://lc.hnjuh.cn

JS:   a && b || !c
来源：http://cj.panjiajie.cn

TS:   a && b || !c
来源：http://gz.asd995.cn

Java: a && b || !c
来源：http://ct.yuntaijiaju.cn

Go:   a && b || !c
来源：http://fr.521024.cn

Ruby: a && b || !c
来源：http://vr.nicolike.cn

C#:   a && b || !c
来源：http://bb.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ji.jianghongdianzi.cn

Py:   if not data: return
来源：http://tq.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://dx.asd995.cn

JS:   if (!data) return;
来源：http://xe.huixiangedu.cn

TS:   if (!data) return;
来源：http://si.jctech888.com.cn

Java: if (data == null) return;
来源：http://fn.shtwfgs.cn

Go:   if data == nil { return }
来源：http://cg.shxzskj.cn

Ruby: return if data.nil?
来源：http://hg.nicolike.cn

C#:   if (data == null) return;
来源：http://gb.jianghongdianzi.cn

================================================================================
来源：http://qk.szxytkj.cn

C. 函数与作用域
来源：http://lp.szxytkj.cn

================================================================================
来源：http://bw.huanxung.cn

[C01] 定义函数
来源：http://bi.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://yk.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://um.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://kr.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pa.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yu.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sp.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://tq.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jl.gzmigu.cn

[C02] 默认参数
来源：http://jv.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://bn.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mv.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://it.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dh.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tg.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uh.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://by.hahajie.cn


<!-- 参考信息 -->