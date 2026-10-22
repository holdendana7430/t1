代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2jqutlpnl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wdxthlxw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2reiudgwj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kopaexzc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jdkibery.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2gzojmbwz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ifdzsfbk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2sqdatgza.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qcsyfmmj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2igpugncb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gnvyabzy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2pvoubiih.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2joytgsom.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dxgkbole.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2squivezs.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2daewfwpa.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tgcpkrbb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pszcutvk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wlncvdmu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2apcswzxv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2evszwywh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ggaevijg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ddospgjd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2dyhyiizu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ngloovmb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2iizxcdrk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2hkrbzicz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2hppvvrjl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rsqwqwxs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jzqbjhos.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xqltkuif.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wadoqhan.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2frsuvihp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cecrmwls.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vmtgrotq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2fpizrspp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dzolpikw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozhlcltg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2pinsmipw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2lbcqclsk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rjgzebhm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uijdfvgb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojmlizvp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2virpnhtn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bmbvdtsf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kotgzfvv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2nijdbxne.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2rljwsbiu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lpzjojbe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qncxguvl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vjrfdzju.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vzplywte.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pfnpdqro.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2sfegstyc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2kxmdaiec.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2uahdklua.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2wvkekqjb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fkvxcdvb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ezuzwxqr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ywifdwvd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nemhpvgx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2yyrqbobk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tyglzmxk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mjzintqe.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ozaiizcq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdddxww.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2revucnhc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yaxepkgc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jhlioutq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgmdunxd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vgiyjnri.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bznvjzum.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wxbtmrzm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qibuwxby.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hxpcmqjs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2nqczewnq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cerbowvj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zlvtbeql.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2snubjygj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pzbhcfff.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xwyqmaqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghqwybcr.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2amjqgflh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nllujfbb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2aqinzsli.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2fvyemfob.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2zbqzyvfa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2znookeod.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kecjhlse.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ddksowlq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2movwftrp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lvhkfyhx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hzrrlega.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wcobybzr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2kfnkdsdk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2svqyhemz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dqiekeel.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2axwegfau.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nrrattjf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ilqquofa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2goaoymhb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dgoqujdt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ffmjeblx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2uxhbgdlo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ylntjqqv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctvnjsvw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eayunarg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opdtnhal.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tafhipwb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ipdjbifc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pounhmrb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2eiwpddlw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2iknvhmnx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2apzwhfgv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fzbpwrqv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgslrdoz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhgbnzqg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ayvfxxwv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ibwrncpr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mkmgjkmp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ykrgxkky.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2bnrvzzyq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jhhzbccz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2joidnmwq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryswaafg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2nubvasjg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zbfljelz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wxkjqylt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2sunbaacg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ybbussxq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ccfvclxh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssebyxcr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vavlfclk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gxsoszyn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnncozcj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2opwygofb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dilkibnx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2tatpuacy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2owyfkydj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xwnkrinx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2gzphneex.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuklfemr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mevdzljz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljpdcxfe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tkvjndbv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zrywmkym.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2splcecwx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xyuxuopu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2fwlhqkpo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2afaebrgn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mounntjx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2flmgjksw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2shzvqqzb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mfhmmoiv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2shnyxbaj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2owyxaduy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2dgqjgcsx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2mgyvlgec.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dcdohqjj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gugekrss.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pghmznuy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nupunhph.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2viredbcv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2evgkwrtp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oshlcuib.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hvymjndx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gkphcojy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqzuewpu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qsjfinef.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qbmkpohg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2igkppuji.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kbyodmea.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kbxmybpy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nnclktun.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tpztkeil.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2judgcoxy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jhziznna.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2luageabi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dzzrnfta.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybbbhwus.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2djjxvgrw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hclnxrmp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hwxvlkry.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zjxvhcky.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ugtinwgm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2klenzoux.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ytfkfyxy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yisoezil.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yrtsedjs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hoycsrtq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bzsxmxym.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hxfwaboy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xszbumqv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zruwofsc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcljzxbt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rijrfvxt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2debgdyno.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2avfgiinr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tyypljze.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nlamejka.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gskaiqks.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lzhkwpmn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2moelequi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mmdlnhdy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mzrxwvwp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wzargops.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qkxrdypt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dunzhwkc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrxaaca.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikehbipp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2hnqdntps.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ezdtrgnt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jexddthf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cwjkfrrg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lqxduvmu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tlonquvp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2agoduqix.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yfiocvyj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2klcvpjze.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2uljokntj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2cchpqvlv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiahsvqf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bksqdzxe.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vfpjeyyz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wganiwww.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jgozafnv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2thpfdeqo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ayztoowq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfewujmh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2deugwtir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzbzdfxl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wnntdcam.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yhkrnzor.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wqrxujji.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pzzvspcx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zijgmbes.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqlemuqb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mlyyrout.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hywdhrzb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crqdlcfn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2uydvhkzy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2taegasmf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ppmxptbe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2diwctxtm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydrktnix.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2bacjcjuz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2mvjyoncc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xtakdkom.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dyhbvyyo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2klxhmbwg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yyvamzmu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2tdrbkxvw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fbzbsipp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfwhgauw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbasxvrc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2nzthwpod.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2anugzzhl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fvwaejsf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2gyvszdzr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2swhdigri.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mypgfedx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2piwxnqgf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pwrfdiss.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cgdwcpjr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uqdqyvys.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ewxmtajm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnhmdvcs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lgcpudfu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yverlkbx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2btioqeal.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2thtgqvby.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tdvjrwku.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ovmyslfp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jlqwczkl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2idvmbkjm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ljymnhub.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hxmcczzh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2apkfugcr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wufnpbgg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kwshkfrr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2phjyzqum.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jhpmvvsd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nddhkcdl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hpzrcwzs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cyltflhx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wedllbxc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2jbvtullw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqonvjau.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zvyrwpoq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vmdlzsag.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2eetriqsp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2lnocvqvz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2olntoftu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rnihehgf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pzuomaqp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ncyfooth.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfsoboet.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lklruwxo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jixegbzh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kplqxmxh.html


<!-- 参考信息 -->