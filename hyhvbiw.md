代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qm.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://be.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rf.nicolike.cn

[A17] 位运算
来源：http://rr.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sm.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://or.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ql.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rt.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mq.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://il.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fi.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://xa.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://tw.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://zl.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pk.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rd.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://rh.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ya.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://eo.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://ly.colortex.cn

[A19] 交换两个变量
来源：http://nd.shxzukj.cn

Py:   a, b = b, a
来源：http://ht.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://la.521024.cn

JS:   [a, b] = [b, a];
来源：http://vr.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://hb.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://sa.wgjwhj.cn

Go:   a, b = b, a
来源：http://pz.huixiangedu.cn

Ruby: a, b = b, a
来源：http://nv.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://uq.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://sz.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://hl.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ej.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tk.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://ja.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://hb.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yu.9csxet.cn

Ruby: gets.chomp
来源：http://aa.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://oe.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://oz.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://zd.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ku.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://hd.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://py.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://fl.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://as.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://tg.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://dk.newstarts.cn

[A22] 获取字符串长度
来源：http://eu.shtwfgs.cn

Py:   len(s)
来源：http://er.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dh.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bu.jianghongdianzi.cn

TS:   s.length
来源：http://me.muxihuayi.cn

Java: s.length()
来源：http://iq.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ue.huixiangedu.cn

Ruby: s.length
来源：http://zu.szsharing.cn

C#:   s.Length
来源：http://ww.bjjhwx.cn

[A23] 大小写转换
来源：http://ro.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tg.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dk.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hx.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nd.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ja.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pa.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ik.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xb.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://pc.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rv.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kg.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lv.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qk.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ou.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://bi.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nr.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zn.9csxet.cn

[A25] 字符串比较
来源：http://cp.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://dx.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kq.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dv.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wi.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://td.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qj.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://re.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xq.bookmarksfly.cn

[A26] 类型转换总览
来源：http://il.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ii.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://om.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uu.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://of.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pn.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qf.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bh.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wt.panjiajie.cn

================================================================================
来源：http://sb.panjiajie.cn

B. 流程控制
来源：http://ya.gzmigu.cn

================================================================================
来源：http://cu.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://vm.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://br.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jb.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zp.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bt.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://av.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mw.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zk.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zt.521024.cn

[B02] 多分支 else if / elif
来源：http://iq.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fy.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qb.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gh.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vf.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kf.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ck.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pv.521024.cn

[B03] switch / match / case
来源：http://ho.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xy.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bh.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gw.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uo.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ol.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oz.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lw.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://we.nszjky.cn

[B04] for 计数循环
来源：http://hg.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://am.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fk.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hj.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://df.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rs.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://rd.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aj.asd995.cn

[B05] 遍历数组 / 列表
来源：http://lu.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://fc.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dw.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://br.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qj.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://te.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fg.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://qm.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wk.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://rz.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sj.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oi.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ak.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fz.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qz.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cy.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vm.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bj.yuexingan06.cn

[B07] while 循环
来源：http://bi.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://nq.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fu.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://gd.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://jj.asd995.cn

Java: while (i < 10) { i++; }
来源：http://wd.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bb.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://zy.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ex.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://vk.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://zz.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pv.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://sp.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://ec.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://he.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bq.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wh.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://kv.szsharing.cn

[B09] break 与 continue
来源：http://ew.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://op.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://id.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yu.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uu.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zh.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gf.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oo.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jp.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://pw.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vo.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hs.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eq.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zv.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jq.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://df.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eg.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ii.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://jr.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://ss.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://ot.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nq.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fy.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vz.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ds.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://cb.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hu.huixiangedu.cn

[B12] 跳出多层循环
来源：http://xm.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sk.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://st.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mx.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vt.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://he.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rn.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://an.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hh.wgjwhj.cn

[B13] 判断是否为数字
来源：http://qs.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://ar.nicolike.cn

PHP:  is_numeric($x)
来源：http://cb.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://as.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dv.colortex.cn

Java: x instanceof Number
来源：http://mb.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://my.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://gn.panjiajie.cn

C#:   x is int or double or decimal
来源：http://lk.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://zv.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fu.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jj.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://ls.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://cg.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sb.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://an.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vs.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ld.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://ao.nszjky.cn

Py:   a and b or not c
来源：http://sn.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://mk.wgjwhj.cn

JS:   a && b || !c
来源：http://os.521024.cn

TS:   a && b || !c
来源：http://kl.9csxet.cn

Java: a && b || !c
来源：http://il.huanxung.cn

Go:   a && b || !c
来源：http://xc.hahajie.cn

Ruby: a && b || !c
来源：http://rf.bookmarksfly.cn

C#:   a && b || !c
来源：http://os.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hf.bookmarksfly.cn

Py:   if not data: return
来源：http://nf.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://nq.huixiangedu.cn

JS:   if (!data) return;
来源：http://wz.lnxyls.cn

TS:   if (!data) return;
来源：http://uv.shxzukj.cn

Java: if (data == null) return;
来源：http://tl.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://cl.nszjky.cn

Ruby: return if data.nil?
来源：http://vr.haigaiapp.cn

C#:   if (data == null) return;
来源：http://gl.asd995.cn

================================================================================
来源：http://sl.gzmigu.cn

C. 函数与作用域
来源：http://ig.colortex.cn

================================================================================
来源：http://jy.shxzskj.cn

[C01] 定义函数
来源：http://gv.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://zh.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vu.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://dn.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gz.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tv.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://th.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://nu.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vz.bjjhwx.cn

[C02] 默认参数
来源：http://fj.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://er.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cd.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://fr.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qy.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ry.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xn.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://ao.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://mp.gzmigu.cn

[C03] 可变参数
来源：http://ai.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://zm.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fv.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kd.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pp.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ud.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ht.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cj.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fy.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://mk.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sb.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tk.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bp.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yf.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://ol.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://xb.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://hv.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://zd.shxzukj.cn

[C05] 返回多个值
来源：http://lw.yuntaijiaju.cn

Py:   return a, b
来源：http://im.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://cr.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rw.panjiajie.cn

TS:   return { a, b };
来源：http://ax.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ri.panjiajie.cn

Go:   return a, b
来源：http://eg.huixinmuqiang.cn

Ruby: return a, b
来源：http://eo.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ub.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://na.521024.cn

Py:   square = lambda x: x * x
来源：http://yy.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://re.shxzukj.cn

JS:   const square = x => x * x;
来源：http://zy.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://bq.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cj.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://by.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://qd.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qj.hahajie.cn

[C07] 把函数作为参数传入
来源：http://or.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xk.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oi.jianghongdianzi.cn


<!-- 参考信息 -->