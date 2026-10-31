代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ug.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yg.colortex.cn

TS:   if (!x) {}
来源：http://sx.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iv.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ah.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pg.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fq.panjiajie.cn

[A17] 位运算
来源：http://jf.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ob.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ux.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nd.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dv.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fg.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yz.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hg.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bq.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://os.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://vh.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://ym.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tn.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xj.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://sk.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ct.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://xl.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://pb.newstarts.cn

[A19] 交换两个变量
来源：http://yv.huixiangedu.cn

Py:   a, b = b, a
来源：http://zu.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ee.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://gu.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://wm.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://ey.hnjuh.cn

Go:   a, b = b, a
来源：http://mb.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://wh.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://ua.asd995.cn

[A20] 读取标准输入
来源：http://tk.shxzskj.cn

Py:   name = input("请输入：")
来源：http://og.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aq.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uw.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://pl.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://oa.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hp.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://tl.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://fn.521024.cn

[A21] 保留指定小数位输出
来源：http://lz.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://he.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zh.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://st.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://mu.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://lf.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://to.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://pq.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://bn.nicolike.cn

[A22] 获取字符串长度
来源：http://tg.shxzukj.cn

Py:   len(s)
来源：http://dk.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://um.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qy.szsharing.cn

TS:   s.length
来源：http://jl.gzmigu.cn

Java: s.length()
来源：http://ob.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ig.haigaiapp.cn

Ruby: s.length
来源：http://fq.yuntaijiaju.cn

C#:   s.Length
来源：http://td.jianghongdianzi.cn

[A23] 大小写转换
来源：http://gx.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vj.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dc.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xo.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vc.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vl.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ui.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zh.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://js.szxytkj.cn

[A24] 去除首尾空白
来源：http://ri.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nj.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dq.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ud.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xm.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ky.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://dm.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zy.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ti.wgjwhj.cn

[A25] 字符串比较
来源：http://wr.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://sy.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wt.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ni.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://di.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ea.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xf.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sc.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eh.hahajie.cn

[A26] 类型转换总览
来源：http://pf.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://om.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sq.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rx.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://gd.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mu.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sv.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kv.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://up.haigaiapp.cn

================================================================================
来源：http://tl.bookmarksfly.cn

B. 流程控制
来源：http://ii.9csxet.cn

================================================================================
来源：http://rl.colortex.cn

[B01] 条件判断 if / else
来源：http://za.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ad.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mx.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://he.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xz.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://do.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vy.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ou.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zf.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://hk.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gf.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nx.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bk.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dc.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wf.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ww.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cr.asd995.cn

[B03] switch / match / case
来源：http://sq.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gc.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://co.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ix.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://na.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xn.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xi.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xf.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://is.newstarts.cn

[B04] for 计数循环
来源：http://py.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://qi.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://re.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jl.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ey.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mk.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wl.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://rq.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://im.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://ok.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://iq.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hh.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wn.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wk.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lu.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jg.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://hp.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://at.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://za.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kb.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nn.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fr.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xx.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iv.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gy.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bk.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fr.huanxung.cn

[B07] while 循环
来源：http://qb.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://hc.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qt.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://hk.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://jq.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://nb.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wt.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://xa.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://kr.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://sz.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://gp.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lv.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://kz.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://fl.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://gh.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tp.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ui.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://zs.521024.cn

[B09] break 与 continue
来源：http://lz.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zk.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hi.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qe.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xh.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://le.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xn.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ti.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ho.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ut.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cd.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fj.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gh.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fk.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dk.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://be.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gq.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wh.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://at.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://vh.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://nr.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lf.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://og.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lk.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://by.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://me.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bu.shxzukj.cn

[B12] 跳出多层循环
来源：http://nf.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xe.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dw.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sq.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bf.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bp.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cd.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wr.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vz.wgjwhj.cn

[B13] 判断是否为数字
来源：http://vo.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://cv.huanxung.cn

PHP:  is_numeric($x)
来源：http://vj.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dj.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sw.yuntaijiaju.cn

Java: x instanceof Number
来源：http://jt.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://af.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://ad.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://sa.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://ty.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iy.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bd.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://jt.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ka.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uu.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zd.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mq.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fe.shxzukj.cn

[B15] 布尔运算与取反
来源：http://qr.lnxyls.cn

Py:   a and b or not c
来源：http://kv.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://vh.haigaiapp.cn

JS:   a && b || !c
来源：http://of.huixinmuqiang.cn

TS:   a && b || !c
来源：http://ym.lnxyls.cn

Java: a && b || !c
来源：http://bf.hnjuh.cn

Go:   a && b || !c
来源：http://xv.nicolike.cn

Ruby: a && b || !c
来源：http://ti.huixiangedu.cn

C#:   a && b || !c
来源：http://sv.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xy.huanxung.cn

Py:   if not data: return
来源：http://me.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://xy.9csxet.cn

JS:   if (!data) return;
来源：http://ki.huixiangedu.cn

TS:   if (!data) return;
来源：http://la.wgjwhj.cn

Java: if (data == null) return;
来源：http://kf.szsharing.cn

Go:   if data == nil { return }
来源：http://hz.gzmigu.cn

Ruby: return if data.nil?
来源：http://sp.huanxung.cn

C#:   if (data == null) return;
来源：http://sq.shxzskj.cn

================================================================================
来源：http://la.521024.cn

C. 函数与作用域
来源：http://rl.shxzukj.cn

================================================================================
来源：http://xs.bookmarksfly.cn

[C01] 定义函数
来源：http://ek.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://aq.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ei.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ih.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uw.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://by.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kd.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://hw.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://di.jianghongdianzi.cn

[C02] 默认参数
来源：http://qi.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://zn.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dx.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://yw.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dh.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://th.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vk.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://mg.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://df.bookmarksfly.cn

[C03] 可变参数
来源：http://gj.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://co.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://re.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ga.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oa.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mw.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dw.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gj.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xn.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://io.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xd.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qk.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ab.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ps.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://td.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://ta.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://kg.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://wb.colortex.cn

[C05] 返回多个值
来源：http://sc.panjiajie.cn

Py:   return a, b
来源：http://yu.szsharing.cn

PHP:  return [$a, $b];
来源：http://fq.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zx.haigaiapp.cn

TS:   return { a, b };
来源：http://cj.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bl.nicolike.cn

Go:   return a, b
来源：http://lf.nicolike.cn

Ruby: return a, b
来源：http://lp.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://kh.521024.cn

[C06] 匿名函数 / lambda
来源：http://ks.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://tz.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vp.szsharing.cn

JS:   const square = x => x * x;
来源：http://bf.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://kc.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dk.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rh.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://kh.huanxung.cn


<!-- 参考信息 -->