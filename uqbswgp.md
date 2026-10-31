代发 wailian999

Py:   "第一行\n第二行"
来源：http://wg.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://fx.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://cr.hahajie.cn

TS:   "第一行\n第二行"
来源：http://rt.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://qe.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://ka.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://mr.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://yh.newstarts.cn

[A14] 注释写法
来源：http://og.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rk.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lh.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://cp.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://lz.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dm.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://vx.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ih.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://hr.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://ej.asd995.cn

Py:   value = data or "默认值"
来源：http://sm.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://gb.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://bz.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://rq.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ml.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://zj.asd995.cn

Ruby: value = data || "默认值"
来源：http://uy.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://ew.asd995.cn

[A16] 真假值判断规则
来源：http://oc.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bn.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ee.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ps.hahajie.cn

TS:   if (!x) {}
来源：http://ku.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fu.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sr.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://in.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lm.yuexingan06.cn

[A17] 位运算
来源：http://xu.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mj.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://do.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fn.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sl.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://so.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rg.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fz.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pb.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://vh.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://ta.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://xt.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zv.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ni.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://gn.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cd.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://wl.521024.cn

C#:   (int)'A'; (char)65
来源：http://hx.bjjhwx.cn

[A19] 交换两个变量
来源：http://kg.szsharing.cn

Py:   a, b = b, a
来源：http://ww.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ee.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://je.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://vk.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://bp.9csxet.cn

Go:   a, b = b, a
来源：http://fs.newstarts.cn

Ruby: a, b = b, a
来源：http://xj.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://wu.lnxyls.cn

[A20] 读取标准输入
来源：http://tg.hahajie.cn

Py:   name = input("请输入：")
来源：http://tj.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gu.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hy.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://hi.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://zk.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lx.521024.cn

Ruby: gets.chomp
来源：http://dg.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://qo.hahajie.cn

[A21] 保留指定小数位输出
来源：http://pw.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://ut.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ta.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://td.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://kq.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://oc.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ya.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://oi.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://ki.hnjuh.cn

[A22] 获取字符串长度
来源：http://ce.lnxyls.cn

Py:   len(s)
来源：http://pm.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jt.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cx.chemitech.net.cn

TS:   s.length
来源：http://bg.huixiangedu.cn

Java: s.length()
来源：http://gk.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ur.szxytkj.cn

Ruby: s.length
来源：http://rx.521024.cn

C#:   s.Length
来源：http://md.bjjhwx.cn

[A23] 大小写转换
来源：http://cm.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cr.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bk.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ml.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://in.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vl.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tn.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tx.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://aj.huanxung.cn

[A24] 去除首尾空白
来源：http://tv.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mm.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zy.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jr.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fn.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fd.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://go.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dz.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pc.shxzskj.cn

[A25] 字符串比较
来源：http://dj.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://yj.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ea.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ti.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xg.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uw.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fu.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ax.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jk.wgjwhj.cn

[A26] 类型转换总览
来源：http://no.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lt.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yb.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xp.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://fz.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nf.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cv.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dh.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fm.9csxet.cn

================================================================================
来源：http://ju.gzmigu.cn

B. 流程控制
来源：http://wc.asd995.cn

================================================================================
来源：http://vs.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://bz.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mv.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cz.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://to.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ej.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ii.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kl.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://at.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pq.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://rm.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hd.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gv.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xy.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uy.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qt.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vp.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vk.asd995.cn

[B03] switch / match / case
来源：http://nx.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ac.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kl.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bh.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hc.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zg.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hr.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xy.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zv.jctech888.com.cn

[B04] for 计数循环
来源：http://vi.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://lk.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wk.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fp.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ox.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pr.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://jt.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vm.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://od.nszjky.cn

Py:   for item in arr: print(item)
来源：http://dd.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fq.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fb.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ye.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bc.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aw.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://kg.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oa.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://dx.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vj.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qj.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bw.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kp.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zr.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zd.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nn.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hahajie.cn

[B07] while 循环
来源：http://gi.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://of.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://re.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://ml.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://kw.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://yb.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ox.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://cl.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://qw.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://xk.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://jh.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qx.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://qx.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://ls.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://fd.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fx.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wx.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://se.szxytkj.cn

[B09] break 与 continue
来源：http://rk.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hs.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rr.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lj.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zc.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yr.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yj.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lw.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mg.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://lf.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ce.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ag.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pl.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pe.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aa.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hv.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ru.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hg.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://pt.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://cm.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://oa.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://os.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yq.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mb.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lq.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://ai.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lw.wgjwhj.cn

[B12] 跳出多层循环
来源：http://xy.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://he.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vo.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sv.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qn.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jy.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uz.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tq.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ku.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://ap.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://ul.szxytkj.cn

PHP:  is_numeric($x)
来源：http://en.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ur.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hw.chemitech.net.cn

Java: x instanceof Number
来源：http://qf.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://um.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://st.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://st.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://ju.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://od.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pn.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://mu.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://fh.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fc.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vs.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://id.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vi.nszjky.cn

[B15] 布尔运算与取反
来源：http://bt.newstarts.cn

Py:   a and b or not c
来源：http://cn.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://mz.shxzukj.cn

JS:   a && b || !c
来源：http://cw.shxzskj.cn

TS:   a && b || !c
来源：http://zw.newstarts.cn

Java: a && b || !c
来源：http://ez.yuntaijiaju.cn

Go:   a && b || !c
来源：http://ir.bjjhwx.cn

Ruby: a && b || !c
来源：http://px.nszjky.cn

C#:   a && b || !c
来源：http://we.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vg.bjjhwx.cn

Py:   if not data: return
来源：http://en.colortex.cn

PHP:  if (!$data) { return; }
来源：http://ye.newstarts.cn

JS:   if (!data) return;
来源：http://jn.wgjwhj.cn

TS:   if (!data) return;
来源：http://aa.bjjhwx.cn

Java: if (data == null) return;
来源：http://ha.panjiajie.cn

Go:   if data == nil { return }
来源：http://xz.jctech888.com.cn

Ruby: return if data.nil?
来源：http://au.hahajie.cn

C#:   if (data == null) return;
来源：http://vn.hnjuh.cn

================================================================================
来源：http://ea.asd995.cn

C. 函数与作用域
来源：http://nz.bjjhwx.cn

================================================================================
来源：http://uv.huixiangedu.cn

[C01] 定义函数
来源：http://yl.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://ar.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bo.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://jd.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mj.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://in.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gy.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://nc.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gf.shxzukj.cn

[C02] 默认参数
来源：http://rx.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://tu.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://px.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://dy.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ax.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cy.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tv.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ro.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://ti.szxytkj.cn

[C03] 可变参数
来源：http://tr.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://pi.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xp.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ha.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kc.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bt.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://si.shxzskj.cn


<!-- 参考信息 -->