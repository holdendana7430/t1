代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://rl.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://iy.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xc.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://um.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://qu.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://uq.szsharing.cn

[A16] 真假值判断规则
来源：http://ca.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zz.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gx.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ra.nicolike.cn

TS:   if (!x) {}
来源：http://cj.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kz.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rz.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://aa.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nw.bjjhwx.cn

[A17] 位运算
来源：http://jb.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://py.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://np.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ud.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cz.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ob.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ci.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gu.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nf.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://fs.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://jt.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://xa.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xe.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ix.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://xt.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mg.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://vi.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://tc.szxytkj.cn

[A19] 交换两个变量
来源：http://is.colortex.cn

Py:   a, b = b, a
来源：http://su.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nc.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://hc.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://qw.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://ji.wgjwhj.cn

Go:   a, b = b, a
来源：http://lj.9csxet.cn

Ruby: a, b = b, a
来源：http://at.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://mp.hahajie.cn

[A20] 读取标准输入
来源：http://jo.nszjky.cn

Py:   name = input("请输入：")
来源：http://hr.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hc.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jp.521024.cn

TS:   // Node.js：readline 模块
来源：http://ps.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://hl.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jz.nszjky.cn

Ruby: gets.chomp
来源：http://kg.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://hh.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://zo.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://rw.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uw.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://fy.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://uh.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://bh.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wr.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ka.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://rc.haigaiapp.cn

[A22] 获取字符串长度
来源：http://bd.shtwfgs.cn

Py:   len(s)
来源：http://or.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://to.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rr.9csxet.cn

TS:   s.length
来源：http://ln.muxihuayi.cn

Java: s.length()
来源：http://mt.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eo.9csxet.cn

Ruby: s.length
来源：http://qk.newstarts.cn

C#:   s.Length
来源：http://zf.bjjhwx.cn

[A23] 大小写转换
来源：http://zc.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ao.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xs.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vc.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yx.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://as.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pn.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bk.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://co.9csxet.cn

[A24] 去除首尾空白
来源：http://xg.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://am.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ka.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ty.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vf.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ha.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://tf.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oe.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://my.shtwfgs.cn

[A25] 字符串比较
来源：http://xi.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://av.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hk.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bw.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rw.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gk.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mj.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ea.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hw.yuexingan06.cn

[A26] 类型转换总览
来源：http://hu.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aw.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zy.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qb.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://ge.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ha.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://es.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ke.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uf.shtwfgs.cn

================================================================================
来源：http://zr.chemitech.net.cn

B. 流程控制
来源：http://qf.jianghongdianzi.cn

================================================================================
来源：http://wg.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://vs.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tu.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ys.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ut.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oi.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hl.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ji.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fa.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://il.szsharing.cn

[B02] 多分支 else if / elif
来源：http://fg.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ty.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jb.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mv.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oa.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://di.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fe.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nt.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dz.wgjwhj.cn

[B03] switch / match / case
来源：http://qi.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fv.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bn.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://du.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kv.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qw.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dk.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eg.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://am.gzmigu.cn

[B04] for 计数循环
来源：http://ws.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://qz.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vk.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ny.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://um.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mf.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cw.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://nu.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xg.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://qb.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://rg.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xl.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bk.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lo.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xw.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zo.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://hu.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mw.asd995.cn

[B06] 遍历字典 / 对象
来源：http://nx.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zk.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mv.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jw.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ro.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tj.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ki.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fq.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vy.panjiajie.cn

[B07] while 循环
来源：http://jy.nicolike.cn

Py:   while i < 10: i += 1
来源：http://vm.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kt.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://pd.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://lm.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://jd.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zr.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://mo.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://bt.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://uq.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://nb.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vf.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://yi.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://wy.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://aa.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eu.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vq.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://kc.muxihuayi.cn

[B09] break 与 continue
来源：http://an.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qm.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bx.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fa.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oq.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kd.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lb.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lh.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cu.hahajie.cn

[B10] 遍历同时拿索引
来源：http://mq.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://og.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lj.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cc.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sx.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ft.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kr.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bx.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://al.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://aw.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://bq.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://or.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dh.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ek.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://se.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://co.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://mz.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dd.huixiangedu.cn

[B12] 跳出多层循环
来源：http://zj.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wb.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xl.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fg.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gu.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bu.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vp.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hm.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://md.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://ap.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://iq.nicolike.cn

PHP:  is_numeric($x)
来源：http://fs.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nw.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://el.9csxet.cn

Java: x instanceof Number
来源：http://rk.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tx.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://sj.asd995.cn

C#:   x is int or double or decimal
来源：http://wd.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://dp.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ky.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ee.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ys.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://uk.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zk.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lw.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lp.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cr.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://nm.shxzukj.cn

Py:   a and b or not c
来源：http://xq.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://py.lnxyls.cn

JS:   a && b || !c
来源：http://hx.hahajie.cn

TS:   a && b || !c
来源：http://wx.chemitech.net.cn

Java: a && b || !c
来源：http://zc.huanxung.cn

Go:   a && b || !c
来源：http://oy.gzmigu.cn

Ruby: a && b || !c
来源：http://vb.shtwfgs.cn

C#:   a && b || !c
来源：http://hn.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cd.jianghongdianzi.cn

Py:   if not data: return
来源：http://tc.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://ll.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://ib.jctech888.com.cn

TS:   if (!data) return;
来源：http://wx.huanxung.cn

Java: if (data == null) return;
来源：http://ue.panjiajie.cn

Go:   if data == nil { return }
来源：http://lz.szxytkj.cn

Ruby: return if data.nil?
来源：http://in.jctech888.com.cn

C#:   if (data == null) return;
来源：http://gy.jctech888.com.cn

================================================================================
来源：http://dz.hnjuh.cn

C. 函数与作用域
来源：http://cg.hahajie.cn

================================================================================
来源：http://ff.gzmigu.cn

[C01] 定义函数
来源：http://op.asd995.cn

Py:   def add(a, b): return a + b
来源：http://an.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ym.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://gj.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gw.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zz.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nx.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://rk.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gn.yuntaijiaju.cn

[C02] 默认参数
来源：http://jj.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://qr.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dh.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://fl.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gq.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://es.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nj.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://hj.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://eb.asd995.cn

[C03] 可变参数
来源：http://bd.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://kw.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wr.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pj.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nh.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nv.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vj.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pz.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ss.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://hr.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yu.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sg.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wk.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gs.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://pd.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://zm.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://xf.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://dk.chemitech.net.cn

[C05] 返回多个值
来源：http://bz.huanxung.cn

Py:   return a, b
来源：http://xh.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://de.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gm.yuntaijiaju.cn

TS:   return { a, b };
来源：http://bq.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://la.wgjwhj.cn

Go:   return a, b
来源：http://tk.nicolike.cn

Ruby: return a, b
来源：http://hg.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://hn.asd995.cn


<!-- 参考信息 -->