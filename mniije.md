代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dzfoacji.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gizzldcf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrhhyukt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vsesohhf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dcdhexgh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zdbvydxd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwthqulu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wztcablc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2frwtkpdd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hhbiztck.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wytvfkwb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mkvlqmse.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2axgoywcb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wyvegabu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ifumkesa.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2dagnicip.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2jzafjidh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zaokmfgt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2knszlpto.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2qxqjmzaw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2fnbunmsp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mussirse.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2voyilmag.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gtqarqtf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pgkfdvhe.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2agyoynvz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2tpsjgpef.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2cwqheazv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2vmftcqsi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jnjzerli.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2cwwktoqc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xzqertcs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2fdxovcwk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2fshgpouz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2bjxkpvcw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2vxcqkzuc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2voqjmbwf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fokdbkre.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vsurtbel.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wcgjjcgj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wvwmlnlg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pokvlqmp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fodvfajh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xkldcffw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ginxtxty.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwjwbpac.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sizcoxba.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2dkenjtsk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2vkrpcohh.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wjpzhvgs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2cocdtuam.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bxjexbne.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nwueukjt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gfvnvkls.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2gevhiemx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2cjednwfc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2klatkati.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2humtqlrn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hxlatrag.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2malqdcyi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2deflnzmb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ycqbtxto.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nshznten.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xewdeqzp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zqpbdoaa.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qvumbsiu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sxgzwwjo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2aflfdxta.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vmkynsey.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2smzxhzcn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rroihxnq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2msmkvodp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kzehanqg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2enbmbotj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2uwsnsizo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jjnupcpm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypnbkzfo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkpvpatm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qwwwndtr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gyzluslw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ncjfvfyz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qwjeawqo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2gkyawuzs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2wiselqlq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2oilgggma.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xdhgnhiu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kwjdnron.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uaianqmq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uhspynqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqvwobje.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fvbyzcme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xoqpnmcq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jyfdmpaq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dqggtzuq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqjqlziy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rpcyvlqz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2znczjfbo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bpaetlfw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bnreshff.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2usbjffxg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2upcrpvjx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ycwctulu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uwcnwzeg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2tvkxzjdt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ppjwdofc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2npovraqo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2atdmthgo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2htfrnoac.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2hfhcwbhr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dbuhaheb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2skxazazc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2fphdoqwm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wtdogeup.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzzeuei.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grdkxolk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2duxdyqex.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2egrzifsd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2nsxpbdoi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lmsecpop.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bwrbzfwz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2csylwbxf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2geoatqrl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyaqrxzg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2grykhdtk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrixizgl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dldbpoiq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2scoxkrsu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lanbewli.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vsgvemqa.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kvfbktmx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzhhecsr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2znsmzovh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bpsrbhkh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdkiiaco.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qceopkqk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xwltvvxp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ysjbdyxp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2bxrpgpcb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2apcpmnxh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezfrfrvf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxtwuzwp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2moquzeoo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2boacmujp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nlywjvwp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ufzryuec.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyyjiylt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mcpyqslm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2buuypotn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ixwxavuu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2twnuhfyw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jcmqopaw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rppxdofx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wekontlr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zxlfnndo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwqrbsdy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kycfurvz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2llclmmck.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hbjtzxay.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fqhcffwh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lgrylynn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vdmnparz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zscbnrtz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2nytpyxll.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2boytekyq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qrgpwopx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vuefzddj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bbjidlby.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2shfqbvhp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntitonps.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qatvywfx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mnhsklak.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rfchgdmu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zrvumomx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kxdqnywe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pjbcycdk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuawoqve.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qgoyranp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2oompchio.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqfgrupb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xurxjxqg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rqgkleqm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ljjgxgbh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vsynirxl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2evhjgzri.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ahujikyt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bcmcpcio.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2klzihddg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jongqspz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ytowvkyd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nopomipn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bveemegz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hfjnwbom.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2evgyfxvo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wmbnaauf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2inrwzbrl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qszknvlu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ynmestxz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hzkebyit.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pcxsinxb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lleivwsb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pawleksa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rydiplva.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2qivmcpbm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xmoxmrgr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2djrtmrvx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zgzlorek.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zjhutuzc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2cbopxgjj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2unjrpzip.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2pkrlmwky.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zarehaxi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2exsiuatl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jtfrohtc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfkixjui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ilvynsng.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2idspuhdf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqjcyvzw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fdqdtkfc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2lpoacjkt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wmpexebf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dxeinmug.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ewjstcyc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ggdjrrri.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tnfqvzvh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lwgzhxhn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mcpaupca.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uafcrbgx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lprkdmtz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2npvrbflv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jdpatltb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cltqtabk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mjdoyoiv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tbsksxic.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jcdllkzo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2yffhiksd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ojcocpgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcrconjf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2srqziixk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdbjenux.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbzmofvn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2epwdvnbx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oqchqiaj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2meyayfpj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sweotztw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjdrifpn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ebuiddbi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2odfkmcqw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wycomzso.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mffaxvjf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vegprvcv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qcjupyif.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dpoeeurq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2movoglnj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2iifqhudb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2oxhjmssk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jatatauh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2utrulgfx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vjaefsbz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jbbuzkug.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kmprbwim.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2heejeshm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbjyyfqg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2exlvitmc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vyytneyo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2brlamtco.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ikujrwgr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ypduvolu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2smwfgqmc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2uxrxvuyp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yyxzvuse.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2sdqyeljx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2vwbybfmy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kofguwye.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ilcmeqbb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vqgyiwnm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zheyjlde.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jtdssuzo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jyougeps.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2abilcfka.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kgeptreg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gdvbyrtv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2honrfcdf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2clsnjgrg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rckkchhr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qdctjfmp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zqbhwwcj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jroryihb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oxnbwosr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nehxbpmt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wodihefh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2weayuqdm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2aotxqdxc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bwzrmdib.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fcpmnwza.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2tjfwzbdc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lpmpftys.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ihidrpfm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2aiuxzibk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjmsnkpf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qykwbasu.html


<!-- 参考信息 -->