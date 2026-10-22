代发 wailian999

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zxyadxho.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2wuzdwsaj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2kgbkgkxf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2etgmkjsx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2nvowkbcx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2avoyvtbp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ycvxkgyh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rupztejo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2gffnrbpj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2uruftuep.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2qzzzoumr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2hrdlmouh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2csbheima.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mcjbixjo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oyamirhd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bgogpwoj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2phqoeavq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxyohxj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dtancmbq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2saxcwogv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2raixkwem.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2mkarukbo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2blpmmhbr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2bzxdgwai.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zfcchiqc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wlgrgnyb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfamtuef.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2whglgxlm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2inejidqx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzkejodl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ewgtcukl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fdgsurrm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2axytwrfh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vxtyqqaw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fjrncaub.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abqxyfjy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gtszluvr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2jgntmkjf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2onjyboak.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2hqcvyxbx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2bikbfixm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2alnksmqi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2quodhhia.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lkgixzet.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2pynbhgww.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2yhmmdxbm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pcemqsxx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hoqlzkbp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ceddgjgh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekdsvlsk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mmarcjzv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rdauvscr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2niqwslco.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2svkbfjff.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2gakyrcdo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ximhpmtl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ngxfbrlq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2gehqxpkj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fyrfnchn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2maiajsfm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2nhifozve.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ltbjjgfr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2irmcvhbh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2gzbupqit.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nwcbufrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmdeqpwe.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2blsvsojd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogeblhjw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vzzikxra.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wprnprfz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzyvnnfo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2emrxglxc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sthafdxw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ajxhegqx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2rfqdoxkg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2tikfdklw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2phxruset.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2dzzhtilv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2erykntsm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxlqroeo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bujmvsxy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nhcmklgo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2owxyufur.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dlnxeqqb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dpaufjug.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2heqbuopr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kynbhtxx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bitjdkuj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekyxwipt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2shcidoav.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oeysvhyu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ohhgsovy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mkalxcgb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2iwgxrbxo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ubvgwoud.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2phppwcro.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2kegvhhlp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vajmllgk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrwmttjj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rgzffmfi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kylrzton.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fhnhlzwb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fewmpfpl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2plnhwqhr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sbekvezi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2swfvcred.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ubokslbt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqytras.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nfeigodt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkxpuqgy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xtysvzus.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2olcymemm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xvnjickv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gjrlgyce.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bmucwkwc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkilvgka.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2anssdhsn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aemmypde.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ambetlmi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2svmvcbxa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ruahlioj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2urxamaxq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pukehzmo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ijfqylvl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzuxogjc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tgievaml.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2quzsyeeg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2belwqcjf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qpoeczpp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2evrpimfa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ythmuidn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hkiiimnb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mrljjwuy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mzeqfxer.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vbpszmsb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vewndpiy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hyqiozbc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gbekrbdy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ohkkuubb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2svaqkgaz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2yfwmfbaw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2zbojrqlp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpmzetgt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzirouva.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2auziaqia.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aszyetvr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mfxmkbjw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dilkhsjq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2onfdmvtz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hcfncrfa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rrizbada.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fikgpdvl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qnkobatc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zkzfcbcg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2onjmpnyv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pkdovjrp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2jmadlhdl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qsdkkcng.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2luxteqnu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wvnimepo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rvhodgyg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2edgzrafn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tjgylnrl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmreetiq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mqvcfzsa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2icbmbiwi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2flkauhbd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uvhwhemu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qngvqjrr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2aazxcuuw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cziwjyli.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ljkpwugo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sisadayf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bddicezv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lsbkvshi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jylhwfhc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xrvoxatv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rxubrbrg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2prcrmtpp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmphizy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifdcscjl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2toxlujnp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2verwmmpt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2kaglsuzi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2lqjepjel.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nourfujo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dotijrra.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vffvikhp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ivrmyzgq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2axnishwv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vbsbvguy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qbqfkxdn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2obtmzxta.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tlxqgmhy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2sbwtzzss.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kqwaamrc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cjvxlhcz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pfwoshph.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ynxvgnzi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zxbuqukq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wjdpvikd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qmsmvxig.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qrdoupso.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gukmqeey.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nwcbkcwt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rafmaagr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sxopujkk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2swffhmkn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qndoiyvu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gptdxiyw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xabtxenq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ypbubcuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kazfkfhz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uluhjlwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2betugrez.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2falzxacr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qunecnsg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vpxafhdz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xcxnpzjv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubijihin.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2toaoutys.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2khbzgljd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tbnhtcov.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dfgymfrj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xxkpexwl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qtelfczf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqglhvvr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drwrcaah.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2obwpwbdw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2kpsncgmv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rqocgyam.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kkiwgald.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wmqetugr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2hbwcqyrk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nowdzvgk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2cukqbjol.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcvwubbz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iotlbxeq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xubeehqt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mkasnlrf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cxpjxsdt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2axqbjmwu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rriacqod.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pupxptvj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2xhbaubkm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnpeolgg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ojpchotn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2gwikizyw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2guiexflm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gayycszu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lbbifhqa.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ehnkxqmj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2aphvhvbx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2udkhoead.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pivakalb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dttmstmw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nngvqeeo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ftoazbvu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ggyfvlmt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zphizfvy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vtxgtbbw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gqwogysr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xtgkuiuc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bjlhajux.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qwfiqgjx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xwmuktee.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2embvclbo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dtzpunhj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oexvzukc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zlycgmrb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ktxtfcoj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vqtancal.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mcntajbd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rcxzjkwz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arbknzet.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lvihyshd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nqwhlcdd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xgdwykie.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mwzmsail.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jfopafug.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nximcktg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2elixspbu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xbzwynix.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2urfzrrcn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2budtkoio.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ifajtmns.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gzidqged.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hpavmzab.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zayzexeh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkvulekn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vcfcpvwo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yylxlwtl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2clifftkv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kdgsqtif.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezrcmrxl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pgktnrir.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dwowyliw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2latdqmtt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ghdubqzx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2aotmgppk.html


<!-- 参考信息 -->