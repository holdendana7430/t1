代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xz.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://zj.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://lq.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://iu.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dz.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://pd.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://ec.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xo.colortex.cn

Py:   "第一行\n第二行"
来源：http://zk.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://xs.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://kw.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://rd.szsharing.cn

Java: "第一行\n第二行"
来源：http://nj.huanxung.cn

Go:   "第一行\n第二行"
来源：http://mo.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://sb.521024.cn

C#:   "第一行\n第二行"
来源：http://gn.huixiangedu.cn

[A14] 注释写法
来源：http://ng.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ke.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rn.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://yl.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://fn.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nv.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://sp.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://op.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://yu.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://it.nszjky.cn

Py:   value = data or "默认值"
来源：http://hm.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://av.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://zy.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://jy.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xf.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://pi.asd995.cn

Ruby: value = data || "默认值"
来源：http://ru.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://rv.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://dc.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://db.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sj.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oc.hnjuh.cn

TS:   if (!x) {}
来源：http://un.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ew.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sn.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zf.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dp.gzmigu.cn

[A17] 位运算
来源：http://tg.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ng.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ys.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vq.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mk.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xw.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hq.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ra.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://ak.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://xm.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://zf.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rs.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sn.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://dx.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xt.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://pk.colortex.cn

C#:   (int)'A'; (char)65
来源：http://ya.shxzskj.cn

[A19] 交换两个变量
来源：http://os.lnxyls.cn

Py:   a, b = b, a
来源：http://bt.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jf.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://no.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://ox.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://tn.wgjwhj.cn

Go:   a, b = b, a
来源：http://vy.yuexingan06.cn

Ruby: a, b = b, a
来源：http://ba.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://sy.hnjuh.cn

[A20] 读取标准输入
来源：http://uc.hahajie.cn

Py:   name = input("请输入：")
来源：http://tu.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yn.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ub.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://jx.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://kg.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qf.wgjwhj.cn

Ruby: gets.chomp
来源：http://rf.hnjuh.cn

C#:   Console.ReadLine();
来源：http://ax.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://ru.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://pe.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bt.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://hg.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://aj.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://ou.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qr.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://jw.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://ff.shtwfgs.cn

[A22] 获取字符串长度
来源：http://xu.nicolike.cn

Py:   len(s)
来源：http://ik.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cr.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kn.jctech888.com.cn

TS:   s.length
来源：http://wi.huixiangedu.cn

Java: s.length()
来源：http://vs.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iz.panjiajie.cn

Ruby: s.length
来源：http://wr.jianghongdianzi.cn

C#:   s.Length
来源：http://xd.jctech888.com.cn

[A23] 大小写转换
来源：http://zn.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ao.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ir.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yd.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tm.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ux.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hx.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rv.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tq.muxihuayi.cn

[A24] 去除首尾空白
来源：http://nq.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nd.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pn.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ga.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xc.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kj.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://jf.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ke.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pt.lnxyls.cn

[A25] 字符串比较
来源：http://hh.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://ap.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kg.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yg.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ak.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ve.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://os.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://an.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oo.shxzskj.cn

[A26] 类型转换总览
来源：http://lx.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bp.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://np.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fk.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://fs.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qo.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nn.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ty.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qu.szxytkj.cn

================================================================================
来源：http://qz.nicolike.cn

B. 流程控制
来源：http://ak.gzmigu.cn

================================================================================
来源：http://at.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://ob.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oe.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gh.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uu.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://il.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xv.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ju.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qy.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ro.asd995.cn

[B02] 多分支 else if / elif
来源：http://bh.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rb.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bn.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gx.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rj.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zm.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jy.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://va.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vc.521024.cn

[B03] switch / match / case
来源：http://zm.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lv.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qs.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kd.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ot.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mq.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hb.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tq.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iy.bookmarksfly.cn

[B04] for 计数循环
来源：http://rd.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://jx.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ve.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nc.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://my.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qc.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bw.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://zw.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://np.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://ca.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://sm.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mr.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aj.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xn.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fb.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ol.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://hp.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ts.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://te.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ua.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zs.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kq.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hk.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hj.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jt.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pw.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hs.hahajie.cn

[B07] while 循环
来源：http://nh.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://jl.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mq.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://ei.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://ah.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://gj.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nd.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://yg.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://yl.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://ty.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://sc.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://on.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://fe.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://sl.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://er.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ku.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qn.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://gt.wgjwhj.cn

[B09] break 与 continue
来源：http://ch.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vv.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pj.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xa.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zy.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ay.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sn.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cc.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://gk.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://do.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kd.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uh.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sj.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wu.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mq.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nh.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bu.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://gc.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://vi.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://ob.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://na.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://io.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bv.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cu.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://oa.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yq.wgjwhj.cn

[B12] 跳出多层循环
来源：http://wj.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qc.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ta.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cd.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gv.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ru.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sb.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ki.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://of.lnxyls.cn

[B13] 判断是否为数字
来源：http://th.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://pv.szsharing.cn

PHP:  is_numeric($x)
来源：http://ba.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bc.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://em.panjiajie.cn

Java: x instanceof Number
来源：http://nd.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bp.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://no.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://ow.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ze.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ya.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jk.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://to.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://yz.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nq.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wo.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sw.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iw.nszjky.cn

[B15] 布尔运算与取反
来源：http://ni.huixinmuqiang.cn

Py:   a and b or not c
来源：http://cg.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://sy.muxihuayi.cn

JS:   a && b || !c
来源：http://iw.yuntaijiaju.cn

TS:   a && b || !c
来源：http://at.haigaiapp.cn

Java: a && b || !c
来源：http://kl.shxzukj.cn

Go:   a && b || !c
来源：http://jy.lnxyls.cn

Ruby: a && b || !c
来源：http://uk.9csxet.cn

C#:   a && b || !c
来源：http://fw.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tr.hahajie.cn

Py:   if not data: return
来源：http://au.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://of.bookmarksfly.cn

JS:   if (!data) return;
来源：http://hp.shtwfgs.cn

TS:   if (!data) return;
来源：http://ay.gzmigu.cn

Java: if (data == null) return;
来源：http://ot.yuexingan06.cn

Go:   if data == nil { return }
来源：http://zk.hnjuh.cn

Ruby: return if data.nil?
来源：http://ya.panjiajie.cn

C#:   if (data == null) return;
来源：http://lk.bjjhwx.cn

================================================================================
来源：http://oo.wgjwhj.cn

C. 函数与作用域
来源：http://qw.wgjwhj.cn

================================================================================
来源：http://he.chemitech.net.cn

[C01] 定义函数
来源：http://ff.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://lw.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dc.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://nh.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://py.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ku.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qi.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://cf.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hh.jianghongdianzi.cn

[C02] 默认参数
来源：http://fn.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://go.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vs.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://qb.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fs.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hi.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://da.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://eb.nszjky.cn


<!-- 参考信息 -->