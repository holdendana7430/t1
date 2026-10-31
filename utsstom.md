代发 wailian999

Ruby: value = data || "默认值"
来源：http://oj.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://la.bjjhwx.cn

[A16] 真假值判断规则
来源：http://mk.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wk.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mu.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nu.bjjhwx.cn

TS:   if (!x) {}
来源：http://vx.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yl.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ir.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gq.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://as.szsharing.cn

[A17] 位运算
来源：http://au.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rx.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rx.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vn.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ss.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ta.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fc.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ws.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vx.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://at.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://nr.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://sp.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jd.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tg.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://xk.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kd.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://sw.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://aj.hahajie.cn

[A19] 交换两个变量
来源：http://kp.nicolike.cn

Py:   a, b = b, a
来源：http://yr.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mh.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://iq.521024.cn

TS:   [a, b] = [b, a];
来源：http://wp.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://fo.9csxet.cn

Go:   a, b = b, a
来源：http://kw.asd995.cn

Ruby: a, b = b, a
来源：http://qy.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://bl.szsharing.cn

[A20] 读取标准输入
来源：http://oq.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://tb.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tb.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pw.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://jf.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://hk.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bg.asd995.cn

Ruby: gets.chomp
来源：http://jp.nszjky.cn

C#:   Console.ReadLine();
来源：http://oj.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://ba.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://bp.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jq.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://jq.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://bj.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://au.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iz.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://og.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://ij.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://pm.shxzskj.cn

Py:   len(s)
来源：http://hy.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://es.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zn.hahajie.cn

TS:   s.length
来源：http://of.lnxyls.cn

Java: s.length()
来源：http://lz.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cp.hahajie.cn

Ruby: s.length
来源：http://oz.jctech888.com.cn

C#:   s.Length
来源：http://qw.yuntaijiaju.cn

[A23] 大小写转换
来源：http://nr.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qz.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dy.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ky.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vi.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cq.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uz.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uw.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dx.9csxet.cn

[A24] 去除首尾空白
来源：http://ys.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zz.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://op.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kw.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ez.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gx.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://xm.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cn.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fg.jianghongdianzi.cn

[A25] 字符串比较
来源：http://gm.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://hv.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yu.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ol.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wk.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nw.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bf.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kl.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://to.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://xy.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pw.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bm.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rj.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://bx.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ag.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mk.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ff.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mk.yuntaijiaju.cn

================================================================================
来源：http://bm.szsharing.cn

B. 流程控制
来源：http://cn.szsharing.cn

================================================================================
来源：http://vo.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://ee.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jz.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gs.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bc.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oc.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nq.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zb.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tc.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://um.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://pt.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ls.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yf.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nn.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ac.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tc.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yc.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ic.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zh.nicolike.cn

[B03] switch / match / case
来源：http://rd.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xc.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gc.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ro.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ro.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qh.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xd.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rw.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cx.9csxet.cn

[B04] for 计数循环
来源：http://mo.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://xv.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uq.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ip.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wq.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hc.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zm.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://zy.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yd.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://ix.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://ix.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ek.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://br.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://br.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ob.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ry.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://nb.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cp.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://dd.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tx.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://if.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ih.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bt.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://us.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fk.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nx.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ng.asd995.cn

[B07] while 循环
来源：http://cy.hahajie.cn

Py:   while i < 10: i += 1
来源：http://gp.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iz.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://rc.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://cn.colortex.cn

Java: while (i < 10) { i++; }
来源：http://il.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fw.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ca.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://nk.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://fb.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ak.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lp.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://sn.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://fn.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://vl.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ro.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iz.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://al.bookmarksfly.cn

[B09] break 与 continue
来源：http://wj.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dr.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://in.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zd.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sk.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ky.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wt.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pj.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://er.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qf.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ww.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wq.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gu.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://em.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eo.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pl.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vi.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://uc.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://ch.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://pv.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ys.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://re.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zt.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://so.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://cd.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wm.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://ed.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sn.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wl.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nb.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ru.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ti.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dj.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bb.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pu.chemitech.net.cn

[B13] 判断是否为数字
来源：http://ca.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://fu.nszjky.cn

PHP:  is_numeric($x)
来源：http://cd.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xw.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oy.yuexingan06.cn

Java: x instanceof Number
来源：http://wz.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fj.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://rp.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://tu.nicolike.cn

[B14] 判断值是否在集合内
来源：http://wh.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fo.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bk.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://dh.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://rw.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ay.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ma.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qo.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bn.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://bo.jianghongdianzi.cn

Py:   a and b or not c
来源：http://up.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://ks.yuntaijiaju.cn

JS:   a && b || !c
来源：http://zo.szxytkj.cn

TS:   a && b || !c
来源：http://rf.shxzskj.cn

Java: a && b || !c
来源：http://zy.521024.cn

Go:   a && b || !c
来源：http://la.nszjky.cn

Ruby: a && b || !c
来源：http://nw.colortex.cn

C#:   a && b || !c
来源：http://jt.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dd.shxzukj.cn

Py:   if not data: return
来源：http://gv.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://ts.haigaiapp.cn

JS:   if (!data) return;
来源：http://rb.panjiajie.cn

TS:   if (!data) return;
来源：http://ty.bookmarksfly.cn

Java: if (data == null) return;
来源：http://vh.shxzskj.cn

Go:   if data == nil { return }
来源：http://mc.haigaiapp.cn

Ruby: return if data.nil?
来源：http://lb.jctech888.com.cn

C#:   if (data == null) return;
来源：http://ua.shxzukj.cn

================================================================================
来源：http://gk.hnjuh.cn

C. 函数与作用域
来源：http://qu.huixiangedu.cn

================================================================================
来源：http://la.jianghongdianzi.cn

[C01] 定义函数
来源：http://kg.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ou.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nv.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://sq.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ms.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xw.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mm.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://ce.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cg.wgjwhj.cn

[C02] 默认参数
来源：http://wj.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://eb.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ae.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://hm.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gm.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gp.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xi.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://zi.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://hs.nszjky.cn

[C03] 可变参数
来源：http://wv.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://qk.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cr.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uq.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eh.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cq.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xc.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mn.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dw.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://sm.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ny.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ig.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eg.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://su.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://zx.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://ur.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://bn.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://dx.haigaiapp.cn

[C05] 返回多个值
来源：http://ik.colortex.cn

Py:   return a, b
来源：http://xn.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://gx.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zn.lnxyls.cn

TS:   return { a, b };
来源：http://ih.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://re.9csxet.cn

Go:   return a, b
来源：http://pp.hahajie.cn

Ruby: return a, b
来源：http://dy.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://hk.521024.cn

[C06] 匿名函数 / lambda
来源：http://it.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://el.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ca.shxzskj.cn

JS:   const square = x => x * x;
来源：http://it.huanxung.cn


<!-- 参考信息 -->