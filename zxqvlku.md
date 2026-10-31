代发 wailian999

Ruby: value = data || "默认值"
来源：http://jl.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://fq.jctech888.com.cn

[A16] 真假值判断规则
来源：http://az.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ki.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fz.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gp.lnxyls.cn

TS:   if (!x) {}
来源：http://rr.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wd.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://at.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qg.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cd.shxzskj.cn

[A17] 位运算
来源：http://nw.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sp.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://se.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fr.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fn.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vc.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ef.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://ip.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://sc.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://qf.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pz.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mh.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://dy.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yy.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://vo.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://hf.chemitech.net.cn

[A19] 交换两个变量
来源：http://fa.szsharing.cn

Py:   a, b = b, a
来源：http://df.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jl.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://vg.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://ef.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://qi.muxihuayi.cn

Go:   a, b = b, a
来源：http://qg.chemitech.net.cn

Ruby: a, b = b, a
来源：http://gx.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://fd.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ec.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://ue.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://je.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wf.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://zj.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://sk.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sj.nicolike.cn

Ruby: gets.chomp
来源：http://un.szxytkj.cn

C#:   Console.ReadLine();
来源：http://ci.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://cg.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://yd.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hk.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://qu.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://iv.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://yu.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vf.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://ds.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://yd.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://ip.colortex.cn

Py:   len(s)
来源：http://pe.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fj.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ug.shxzukj.cn

TS:   s.length
来源：http://vn.newstarts.cn

Java: s.length()
来源：http://ms.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xe.asd995.cn

Ruby: s.length
来源：http://dl.yuexingan06.cn

C#:   s.Length
来源：http://bu.hahajie.cn

[A23] 大小写转换
来源：http://my.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ud.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vm.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://za.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mn.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qq.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vy.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tv.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kg.newstarts.cn

[A24] 去除首尾空白
来源：http://ev.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lv.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zh.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yy.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ve.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ws.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://kv.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://co.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zr.jctech888.com.cn

[A25] 字符串比较
来源：http://pn.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://en.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nc.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lo.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fj.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qq.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ok.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://en.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vd.bjjhwx.cn

[A26] 类型转换总览
来源：http://tw.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ml.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sn.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yo.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://zx.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pd.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eh.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qe.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://za.nicolike.cn

================================================================================
来源：http://no.shtwfgs.cn

B. 流程控制
来源：http://eg.szxytkj.cn

================================================================================
来源：http://nc.huanxung.cn

[B01] 条件判断 if / else
来源：http://wk.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zy.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zs.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jb.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rr.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ko.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ce.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qz.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ti.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://bf.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mo.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gx.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://it.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hw.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ps.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ue.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mx.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ji.panjiajie.cn

[B03] switch / match / case
来源：http://vs.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mi.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vc.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yd.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://um.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uc.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ym.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mm.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sk.panjiajie.cn

[B04] for 计数循环
来源：http://oj.asd995.cn

Py:   for i in range(10): print(i)
来源：http://mu.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zf.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://un.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uz.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qq.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ii.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://qf.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jd.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://cq.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://lu.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qo.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uh.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kf.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vw.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gs.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://wl.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hs.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://vk.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rp.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bq.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yh.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fy.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lw.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ux.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sm.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rz.nicolike.cn

[B07] while 循环
来源：http://mb.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://yl.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://im.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://sa.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://jt.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://hx.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ls.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://qi.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://eh.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://rr.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://xs.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kh.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://td.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://yc.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://ns.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ld.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fi.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://pv.shxzskj.cn

[B09] break 与 continue
来源：http://pn.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ez.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://my.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tm.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yo.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oe.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rm.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ti.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gj.colortex.cn

[B10] 遍历同时拿索引
来源：http://xv.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bx.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pb.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lh.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ak.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ry.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eb.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sc.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ga.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://rx.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://ee.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://wu.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zg.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qf.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nn.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://va.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://wg.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aj.bjjhwx.cn

[B12] 跳出多层循环
来源：http://go.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wp.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nx.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bm.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ga.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://da.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vl.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cy.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://no.shxzukj.cn

[B13] 判断是否为数字
来源：http://hr.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://gg.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://ey.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gh.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dv.huixinmuqiang.cn

Java: x instanceof Number
来源：http://zh.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yy.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://ib.newstarts.cn

C#:   x is int or double or decimal
来源：http://du.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://bg.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://il.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bu.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://ce.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://br.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sq.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wq.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wi.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vz.colortex.cn

[B15] 布尔运算与取反
来源：http://fm.9csxet.cn

Py:   a and b or not c
来源：http://ac.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://rd.nicolike.cn

JS:   a && b || !c
来源：http://rl.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ib.shxzskj.cn

Java: a && b || !c
来源：http://ww.szxytkj.cn

Go:   a && b || !c
来源：http://dr.asd995.cn

Ruby: a && b || !c
来源：http://os.panjiajie.cn

C#:   a && b || !c
来源：http://eq.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xk.huanxung.cn

Py:   if not data: return
来源：http://fx.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://vc.szsharing.cn

JS:   if (!data) return;
来源：http://mi.chemitech.net.cn

TS:   if (!data) return;
来源：http://nn.huixiangedu.cn

Java: if (data == null) return;
来源：http://nq.szxytkj.cn

Go:   if data == nil { return }
来源：http://kz.shtwfgs.cn

Ruby: return if data.nil?
来源：http://sv.chemitech.net.cn

C#:   if (data == null) return;
来源：http://cd.huixiangedu.cn

================================================================================
来源：http://ws.huanxung.cn

C. 函数与作用域
来源：http://pm.nicolike.cn

================================================================================
来源：http://zb.haigaiapp.cn

[C01] 定义函数
来源：http://on.asd995.cn

Py:   def add(a, b): return a + b
来源：http://on.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uo.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://lk.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fc.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ka.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wi.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ad.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ey.521024.cn

[C02] 默认参数
来源：http://ig.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://qv.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xy.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://kp.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://im.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rm.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lj.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://kl.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://hc.colortex.cn

[C03] 可变参数
来源：http://ub.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://yf.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wx.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lc.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rx.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tk.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xa.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ll.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ws.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://ao.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ra.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gb.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ri.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ch.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://lc.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://rf.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://vi.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://rq.bookmarksfly.cn

[C05] 返回多个值
来源：http://zi.chemitech.net.cn

Py:   return a, b
来源：http://gf.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://mw.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://di.nicolike.cn

TS:   return { a, b };
来源：http://he.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fz.yuexingan06.cn

Go:   return a, b
来源：http://gd.huanxung.cn

Ruby: return a, b
来源：http://xg.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://st.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://le.huanxung.cn

Py:   square = lambda x: x * x
来源：http://or.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://du.9csxet.cn

JS:   const square = x => x * x;
来源：http://tf.bookmarksfly.cn


<!-- 参考信息 -->