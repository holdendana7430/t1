代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://gq.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://aw.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qv.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://cn.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://mq.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://my.nszjky.cn

[A16] 真假值判断规则
来源：http://ob.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://il.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wb.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sw.hnjuh.cn

TS:   if (!x) {}
来源：http://bc.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gn.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eq.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jw.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://za.huanxung.cn

[A17] 位运算
来源：http://ly.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mo.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zh.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sj.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ca.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nv.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aw.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ct.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jf.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://gr.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://ep.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://ka.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ft.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tr.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://ko.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qd.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://hq.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://bf.bookmarksfly.cn

[A19] 交换两个变量
来源：http://es.panjiajie.cn

Py:   a, b = b, a
来源：http://zy.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://np.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://sk.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://uz.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://qq.muxihuayi.cn

Go:   a, b = b, a
来源：http://ef.haigaiapp.cn

Ruby: a, b = b, a
来源：http://hx.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://qs.gzmigu.cn

[A20] 读取标准输入
来源：http://gb.newstarts.cn

Py:   name = input("请输入：")
来源：http://qe.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://di.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mf.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://en.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://uf.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ap.hahajie.cn

Ruby: gets.chomp
来源：http://ow.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://nc.huanxung.cn

[A21] 保留指定小数位输出
来源：http://ll.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://nw.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ox.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://yo.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://sv.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://jp.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ct.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://kz.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://ko.yuexingan06.cn

[A22] 获取字符串长度
来源：http://jt.nicolike.cn

Py:   len(s)
来源：http://go.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ty.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wy.shxzukj.cn

TS:   s.length
来源：http://rc.yuexingan06.cn

Java: s.length()
来源：http://sf.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gf.colortex.cn

Ruby: s.length
来源：http://mq.shxzukj.cn

C#:   s.Length
来源：http://vo.hnjuh.cn

[A23] 大小写转换
来源：http://nh.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tw.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cf.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ji.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cy.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cm.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zx.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://re.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jx.newstarts.cn

[A24] 去除首尾空白
来源：http://tq.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wt.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://go.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hi.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ul.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uy.521024.cn

Go:   strings.TrimSpace(s)
来源：http://ff.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dw.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xi.521024.cn

[A25] 字符串比较
来源：http://lb.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://nr.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ws.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://le.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wn.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sv.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kt.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nd.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mb.nszjky.cn

[A26] 类型转换总览
来源：http://ec.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mu.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hb.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ql.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://eg.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kr.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://md.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zb.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wi.huanxung.cn

================================================================================
来源：http://if.colortex.cn

B. 流程控制
来源：http://fe.9csxet.cn

================================================================================
来源：http://gz.nicolike.cn

[B01] 条件判断 if / else
来源：http://ah.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://td.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pf.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hl.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hx.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fw.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yf.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qv.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kz.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://nq.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gk.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xw.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://im.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tz.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bs.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mv.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ib.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yk.wgjwhj.cn

[B03] switch / match / case
来源：http://ov.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ki.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ls.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yz.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://av.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ge.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jp.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gu.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://li.yuexingan06.cn

[B04] for 计数循环
来源：http://gj.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://bg.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ui.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bb.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gt.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ln.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://no.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://rk.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://op.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://py.szsharing.cn

Py:   for item in arr: print(item)
来源：http://xd.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://se.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tf.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://go.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vs.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ew.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://cq.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ky.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://nm.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jt.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nw.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://on.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yk.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nm.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ym.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ig.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nt.wgjwhj.cn

[B07] while 循环
来源：http://ft.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://zc.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mh.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://dh.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://qu.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://ma.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zg.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://op.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://gp.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://hv.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://es.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ga.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://zq.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://jm.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://dz.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xi.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qi.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://qq.panjiajie.cn

[B09] break 与 continue
来源：http://zr.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://js.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qy.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jg.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mt.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dj.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oi.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dk.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qz.9csxet.cn

[B10] 遍历同时拿索引
来源：http://py.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bc.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://en.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://db.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pm.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nf.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oh.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nx.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kg.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://eu.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://xh.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://mc.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://on.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mb.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rb.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mm.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://nv.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oj.newstarts.cn

[B12] 跳出多层循环
来源：http://ly.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kj.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sq.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ee.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wt.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qn.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ao.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hx.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nv.muxihuayi.cn

[B13] 判断是否为数字
来源：http://vs.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://dy.panjiajie.cn

PHP:  is_numeric($x)
来源：http://be.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dv.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ss.yuntaijiaju.cn

Java: x instanceof Number
来源：http://ft.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://os.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://et.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://nx.9csxet.cn

[B14] 判断值是否在集合内
来源：http://ik.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hf.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nf.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://od.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://tw.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ki.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://me.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jf.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://to.9csxet.cn

[B15] 布尔运算与取反
来源：http://pj.nszjky.cn

Py:   a and b or not c
来源：http://df.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://ib.colortex.cn

JS:   a && b || !c
来源：http://ls.shtwfgs.cn

TS:   a && b || !c
来源：http://hm.521024.cn

Java: a && b || !c
来源：http://ud.wgjwhj.cn

Go:   a && b || !c
来源：http://uj.muxihuayi.cn

Ruby: a && b || !c
来源：http://ag.hnjuh.cn

C#:   a && b || !c
来源：http://xg.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://iv.shxzukj.cn

Py:   if not data: return
来源：http://tk.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://cg.9csxet.cn

JS:   if (!data) return;
来源：http://bo.huixiangedu.cn

TS:   if (!data) return;
来源：http://xg.asd995.cn

Java: if (data == null) return;
来源：http://fs.shtwfgs.cn

Go:   if data == nil { return }
来源：http://ct.muxihuayi.cn

Ruby: return if data.nil?
来源：http://ur.wgjwhj.cn

C#:   if (data == null) return;
来源：http://eh.shxzukj.cn

================================================================================
来源：http://bg.bjjhwx.cn

C. 函数与作用域
来源：http://vr.colortex.cn

================================================================================
来源：http://nv.bookmarksfly.cn

[C01] 定义函数
来源：http://jy.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://ae.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ys.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://yx.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iu.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ye.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wu.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://bw.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ka.huanxung.cn

[C02] 默认参数
来源：http://wj.521024.cn

Py:   def greet(name="World"): return name
来源：http://mn.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gi.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qb.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kd.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dk.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://df.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://vm.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://og.newstarts.cn

[C03] 可变参数
来源：http://jc.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://ge.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uj.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://is.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bu.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gx.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qq.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dj.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ht.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://dy.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sz.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eo.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wy.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://du.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://yj.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://ej.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://af.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://ey.panjiajie.cn

[C05] 返回多个值
来源：http://zd.yuntaijiaju.cn

Py:   return a, b
来源：http://oa.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://wn.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vj.szxytkj.cn

TS:   return { a, b };
来源：http://hq.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xl.9csxet.cn

Go:   return a, b
来源：http://kc.yuexingan06.cn

Ruby: return a, b
来源：http://jb.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://ne.shxzskj.cn


<!-- 参考信息 -->