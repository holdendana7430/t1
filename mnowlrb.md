代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://pc.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://eq.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ba.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://nd.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://ih.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://wd.shtwfgs.cn

[A16] 真假值判断规则
来源：http://pq.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mx.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rs.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oi.asd995.cn

TS:   if (!x) {}
来源：http://dw.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lm.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://en.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zc.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cd.szsharing.cn

[A17] 位运算
来源：http://yz.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pg.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ip.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gg.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qi.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nr.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vl.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hd.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://da.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://br.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://nu.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://pa.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uc.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wb.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://sd.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oh.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://sp.521024.cn

C#:   (int)'A'; (char)65
来源：http://gn.hahajie.cn

[A19] 交换两个变量
来源：http://xu.nszjky.cn

Py:   a, b = b, a
来源：http://ix.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lt.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://rc.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://hn.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://am.521024.cn

Go:   a, b = b, a
来源：http://kc.jctech888.com.cn

Ruby: a, b = b, a
来源：http://jn.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://fo.9csxet.cn

[A20] 读取标准输入
来源：http://zq.shxzukj.cn

Py:   name = input("请输入：")
来源：http://uc.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zc.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://rd.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://yc.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vp.bookmarksfly.cn

Ruby: gets.chomp
来源：http://gu.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://wt.nicolike.cn

[A21] 保留指定小数位输出
来源：http://dk.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://bq.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hp.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://gv.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://sc.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://fg.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://id.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ci.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://ay.colortex.cn

[A22] 获取字符串长度
来源：http://ir.asd995.cn

Py:   len(s)
来源：http://lv.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wu.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ju.wgjwhj.cn

TS:   s.length
来源：http://sl.nszjky.cn

Java: s.length()
来源：http://gk.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yl.shxzskj.cn

Ruby: s.length
来源：http://ji.chemitech.net.cn

C#:   s.Length
来源：http://uh.9csxet.cn

[A23] 大小写转换
来源：http://df.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yn.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kk.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pz.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ig.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ok.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zl.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wd.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sg.chemitech.net.cn

[A24] 去除首尾空白
来源：http://oe.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ex.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ok.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gn.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ea.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lk.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://bb.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://af.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ob.gzmigu.cn

[A25] 字符串比较
来源：http://iq.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://xy.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hh.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rk.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bo.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dz.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ye.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bd.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kn.haigaiapp.cn

[A26] 类型转换总览
来源：http://of.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hk.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tw.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dj.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://dm.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rg.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ta.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wx.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://co.shxzskj.cn

================================================================================
来源：http://la.521024.cn

B. 流程控制
来源：http://vz.shtwfgs.cn

================================================================================
来源：http://ts.gzmigu.cn

[B01] 条件判断 if / else
来源：http://sk.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zy.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://um.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ay.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fc.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pg.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sp.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://am.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sa.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://xl.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ez.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hx.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jq.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gh.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xw.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ne.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ua.shxzukj.cn

[B03] switch / match / case
来源：http://if.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vw.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ii.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cj.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oz.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eu.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ns.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fu.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ey.yuntaijiaju.cn

[B04] for 计数循环
来源：http://bq.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://oc.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://da.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wo.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jz.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cf.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://rs.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rr.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://yp.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://fa.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vl.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gs.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://er.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nn.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nl.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://en.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ub.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://zn.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hq.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bd.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wr.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aq.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eg.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ly.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cg.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ia.nszjky.cn

[B07] while 循环
来源：http://qi.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://qo.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jo.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://at.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://yn.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://at.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ma.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://gr.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://tz.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://pv.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ao.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vg.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://vu.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://sb.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://nr.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fb.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://da.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ov.bookmarksfly.cn

[B09] break 与 continue
来源：http://by.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tt.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yx.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wg.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gc.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://df.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hp.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ht.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sj.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://ik.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ls.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ju.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yc.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ic.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sd.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bf.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dk.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qe.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://re.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://ca.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://ym.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kc.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wk.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qw.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yf.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://yk.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tp.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://iw.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ui.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gr.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://od.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aw.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bk.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xc.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nl.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ca.shtwfgs.cn

[B13] 判断是否为数字
来源：http://iw.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://de.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://uu.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://le.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yr.jctech888.com.cn

Java: x instanceof Number
来源：http://rw.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jl.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://by.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://ov.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://bn.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://np.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xm.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ee.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://zn.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yv.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dq.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ru.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ge.shxzskj.cn

[B15] 布尔运算与取反
来源：http://mg.szxytkj.cn

Py:   a and b or not c
来源：http://vq.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ds.szsharing.cn

JS:   a && b || !c
来源：http://tq.shxzskj.cn

TS:   a && b || !c
来源：http://ds.newstarts.cn

Java: a && b || !c
来源：http://jb.muxihuayi.cn

Go:   a && b || !c
来源：http://mn.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://jx.huixiangedu.cn

C#:   a && b || !c
来源：http://um.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sv.shtwfgs.cn

Py:   if not data: return
来源：http://vj.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://ad.wgjwhj.cn

JS:   if (!data) return;
来源：http://ui.nszjky.cn

TS:   if (!data) return;
来源：http://du.huanxung.cn

Java: if (data == null) return;
来源：http://yu.huanxung.cn

Go:   if data == nil { return }
来源：http://cw.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://er.hahajie.cn

C#:   if (data == null) return;
来源：http://zk.gzmigu.cn

================================================================================
来源：http://eq.hnjuh.cn

C. 函数与作用域
来源：http://oa.haigaiapp.cn

================================================================================
来源：http://af.yuexingan06.cn

[C01] 定义函数
来源：http://xv.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://pt.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rg.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://hl.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://da.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yn.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://il.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://jf.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ma.huanxung.cn

[C02] 默认参数
来源：http://fd.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://hi.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ne.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://lq.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ys.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nt.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dh.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://yx.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://fa.huanxung.cn

[C03] 可变参数
来源：http://xi.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://st.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vf.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jj.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://th.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://de.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qu.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lo.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mn.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://yt.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nh.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rl.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sj.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ay.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://gg.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://zy.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://by.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://co.jianghongdianzi.cn

[C05] 返回多个值
来源：http://be.wgjwhj.cn

Py:   return a, b
来源：http://fj.asd995.cn

PHP:  return [$a, $b];
来源：http://mm.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bw.yuexingan06.cn

TS:   return { a, b };
来源：http://ho.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jo.muxihuayi.cn

Go:   return a, b
来源：http://vi.lnxyls.cn

Ruby: return a, b
来源：http://bk.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://rt.yuntaijiaju.cn


<!-- 参考信息 -->