代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://jo.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://ec.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zq.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://fs.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://zd.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://eg.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://ak.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wb.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mh.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cl.gzmigu.cn

TS:   if (!x) {}
来源：http://xy.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zg.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oa.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rz.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zp.panjiajie.cn

[A17] 位运算
来源：http://or.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xm.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mb.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pt.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ta.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mz.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bs.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ie.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zt.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://wy.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://pe.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://zh.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mf.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://al.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://dw.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ot.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://jb.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://zx.szxytkj.cn

[A19] 交换两个变量
来源：http://vb.lnxyls.cn

Py:   a, b = b, a
来源：http://sg.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ci.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://az.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://kl.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://ey.9csxet.cn

Go:   a, b = b, a
来源：http://vr.chemitech.net.cn

Ruby: a, b = b, a
来源：http://ue.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://ex.chemitech.net.cn

[A20] 读取标准输入
来源：http://sq.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://vt.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gw.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cz.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://cp.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://lr.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://np.yuexingan06.cn

Ruby: gets.chomp
来源：http://fa.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://zh.9csxet.cn

[A21] 保留指定小数位输出
来源：http://ku.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://fx.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fp.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://el.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://zk.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://zs.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yr.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://ew.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://ka.colortex.cn

[A22] 获取字符串长度
来源：http://qf.panjiajie.cn

Py:   len(s)
来源：http://mh.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ld.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nw.chemitech.net.cn

TS:   s.length
来源：http://os.bjjhwx.cn

Java: s.length()
来源：http://bv.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lm.haigaiapp.cn

Ruby: s.length
来源：http://mk.newstarts.cn

C#:   s.Length
来源：http://oy.asd995.cn

[A23] 大小写转换
来源：http://uu.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kp.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zs.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ay.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hs.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ws.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zd.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kt.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fl.yuexingan06.cn

[A24] 去除首尾空白
来源：http://hb.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nt.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ko.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ta.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jo.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://el.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://iv.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gj.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vf.bjjhwx.cn

[A25] 字符串比较
来源：http://na.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://mt.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hf.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pw.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gc.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cx.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tn.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://my.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lj.gzmigu.cn

[A26] 类型转换总览
来源：http://jt.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://av.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fa.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jy.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://ro.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mp.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vg.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mt.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vx.bjjhwx.cn

================================================================================
来源：http://oz.bjjhwx.cn

B. 流程控制
来源：http://eo.huixiangedu.cn

================================================================================
来源：http://lc.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://ag.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://df.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wc.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pb.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ll.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pr.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vs.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://et.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mr.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://ca.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rq.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pe.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zt.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ge.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://km.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qr.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wr.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zl.haigaiapp.cn

[B03] switch / match / case
来源：http://vc.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yq.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mv.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gj.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ny.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jr.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hi.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ld.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://su.lnxyls.cn

[B04] for 计数循环
来源：http://id.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://aa.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fl.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hj.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vr.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oc.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gm.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://bf.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yg.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://bx.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://fh.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xe.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bo.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fo.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wz.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rg.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://bn.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vd.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://iu.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tp.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pz.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nx.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uk.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hj.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://as.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fb.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ez.hahajie.cn

[B07] while 循环
来源：http://sr.hahajie.cn

Py:   while i < 10: i += 1
来源：http://be.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tj.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://pt.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://wo.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://yu.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yh.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://lh.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://ue.colortex.cn

[B08] do-while（至少执行一次）
来源：http://rf.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://zx.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mq.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://sw.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://ru.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://vr.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cj.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tp.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://uh.chemitech.net.cn

[B09] break 与 continue
来源：http://sa.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hb.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jl.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fs.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jm.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kz.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zn.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kx.9csxet.cn

[B10] 遍历同时拿索引
来源：http://ts.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qf.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cx.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ql.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hw.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ff.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kj.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://py.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zr.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://lr.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://rn.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://nj.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bl.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hn.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wb.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bs.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://gu.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ks.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://kz.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fk.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cd.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fk.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zf.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qg.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dc.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ve.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mu.szsharing.cn

[B13] 判断是否为数字
来源：http://jd.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://pm.panjiajie.cn

PHP:  is_numeric($x)
来源：http://dt.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ef.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://go.haigaiapp.cn

Java: x instanceof Number
来源：http://pd.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yu.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://bo.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://yg.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://pe.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sn.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://mc.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://pa.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jm.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://da.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vz.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zq.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://zs.nszjky.cn

Py:   a and b or not c
来源：http://pc.9csxet.cn

PHP:  $a && $b || !$c
来源：http://us.nicolike.cn

JS:   a && b || !c
来源：http://io.panjiajie.cn

TS:   a && b || !c
来源：http://bx.huixiangedu.cn

Java: a && b || !c
来源：http://gb.jctech888.com.cn

Go:   a && b || !c
来源：http://ge.haigaiapp.cn

Ruby: a && b || !c
来源：http://fw.szsharing.cn

C#:   a && b || !c
来源：http://ha.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rc.gzmigu.cn

Py:   if not data: return
来源：http://hi.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://jn.szsharing.cn

JS:   if (!data) return;
来源：http://uo.szsharing.cn

TS:   if (!data) return;
来源：http://bk.nicolike.cn

Java: if (data == null) return;
来源：http://bc.nicolike.cn

Go:   if data == nil { return }
来源：http://yi.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://jp.szxytkj.cn

C#:   if (data == null) return;
来源：http://nd.newstarts.cn

================================================================================
来源：http://py.wgjwhj.cn

C. 函数与作用域
来源：http://uc.bjjhwx.cn

================================================================================
来源：http://rg.9csxet.cn

[C01] 定义函数
来源：http://et.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://jp.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pt.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://nb.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hk.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yj.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fw.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://vn.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ss.nicolike.cn

[C02] 默认参数
来源：http://rt.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://zl.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vl.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://uv.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://aa.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vz.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ru.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://dg.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://vk.hahajie.cn

[C03] 可变参数
来源：http://ya.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://aa.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ty.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ie.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ae.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pe.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kz.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ww.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jl.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://kt.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lo.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bn.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jl.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sr.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://vy.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://sn.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://up.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://ie.bookmarksfly.cn

[C05] 返回多个值
来源：http://jf.yuntaijiaju.cn

Py:   return a, b
来源：http://ln.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://rw.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ld.yuexingan06.cn

TS:   return { a, b };
来源：http://cv.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gf.huixiangedu.cn

Go:   return a, b
来源：http://nb.9csxet.cn

Ruby: return a, b
来源：http://nc.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://mw.huixiangedu.cn


<!-- 参考信息 -->