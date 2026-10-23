代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ohdzaylh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxikfwm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vieayhji.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gepzcntq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kdszarec.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3bplyujxp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3mtymoqjo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ukvbhwai.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3piuoldbg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3zttvowty.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bculqluu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vrijnyje.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rzdnpotl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3knruhasn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3viyfurjs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nwdtkovf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zlpvvrsr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3iydglhdb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3afeqonni.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3glaiwoen.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gzuulbib.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ugvaxuhv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lxusjlrg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kplnikui.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3iefqlsiy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3vkhjhhlj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3cewzuwis.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fmzjjoww.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rbddqpsv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ycyhpnms.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xywlpyiy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rlktekzl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vtfppqsg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uioouvbz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oczgdicm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3akvgwbea.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vkeidjis.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3moixtnkr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ktffjiiy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jlvsrmyd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nfyqnvcv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3xvrezfsb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3yitkuixm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vjfhzdry.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ammsaddm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jkjydubj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dlimlzcs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3inufsacx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pcbuntwy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3grzdoxgj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kjgyvpsy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3clcvybpj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ejpjijgj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3eyxjlqvk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3lwjflmgn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3cvvlqazm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wicpgolf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qmfhoeto.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tjaexcqj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3prvnqusr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlwsyhjf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3axzwoefy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gvkhwgtb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gxaeaipp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3aqlutkhi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxuawulu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vxautwym.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lmdhmvtz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ltgytbqm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rxpwdfls.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ixpddhbe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cliymovr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mtdpbmwh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ouzrktyz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vveixwrt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vbomigrd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3voxfdojw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zgunyrhx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jhgoukcy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3pxqumffq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3piuchwqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggflqhur.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3cpiykahh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vktvhjtq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xaaexnre.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gynuqfdl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lpnqbadu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zncnhwiv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3krrwyrhb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vdjylyup.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xpfgysns.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3fepntfop.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ogosbpew.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3gjthcgfn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nsgfqaja.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cvuvvsjr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dwobhnsi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ypbygykj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hqufjyck.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3jmnjnwbv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3gkuowaky.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rzqxuloi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3hwdchslc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3uomtbjlq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzawhiim.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lgbkqqib.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3znelmadp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mczlghbh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cnyivprh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vndnmzqk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nkmgedpv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rxkwdgta.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xvqtomrb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3rwcvejss.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pdqwvtbf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3asbrghzw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wkuynnko.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bwwvhqhn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3yinadttr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuimvapp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ruugwxcw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ivqguizf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wyjfawih.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojfsyfex.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgzgffhu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3upbelryg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cjgoczsz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3tqiuwipe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jznqjptk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lydsjdsh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bvhxphlx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3nhphiful.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hdmastcr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbfqsffx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tzevbfhi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jkhchmsw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hacovduc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3seoufnxx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bmakpaob.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3eohtzjli.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3liyjkhxx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lxcmmrct.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uogtfhil.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfklxowo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ouwkgcvh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yvocuvra.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ejrgcbyt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hhsnledt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3woqxrtac.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ofydszvj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sjtipwoy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vsdtgoea.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qiczceyd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kcnvbgwm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3cewhvlrm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mrsdlsei.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vtrgupbd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zycsovik.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tgmxdrdt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcdqhloq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpldvndl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jpfrknpb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xsoizwuz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gtqowtji.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mgomqyjz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3lvmuhndk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3efroaunx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugfkqbdf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pcoqerfe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cuyobjak.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fsuhnonr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bicblaqo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rheaugei.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ymqveapn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kaoxmfkj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wgoalbue.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3loranlmy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nytdjkuc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wnzkjnlk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wshpvskp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eyeeukaz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nzeayore.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hcvjvcdk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3srevngux.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pphtwtxg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sgngarrm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cjzxjeeb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wiwaivix.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3npzjioac.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmvtjptc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3eoaeknnt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rpqhnxtg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sfxupeuf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3snxwftwd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dbhrcopv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yztxzfkk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bazevgqc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hwpigxht.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jgregpcg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lunjuqof.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jitsporh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yilfuvtw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pjhholoj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xgjztpvf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tthdmvvi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zitgwyss.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3grgvrqsl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucvmznsk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shuddvgk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rntztouu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qlvxyeee.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3enekwiio.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mdfuymkp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dbfvbugs.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lcrcgeqy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3huydzdek.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lnocqvlb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3baiahcyp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uqnbmqef.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xxhqghzu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3lmmlucgc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vizihzfu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wqeeawbq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gworxtoc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wbhftoso.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hclgvmrr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3dmuhbhih.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pszrukym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elooksae.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3khzcvozr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juazylom.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ywtrbdrs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3emvvvkmd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lktixiyt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ogetjjfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hggywhhm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3knpgejyd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bwdqzdyp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3getyuvys.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ogyvbnnh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bfecfrrh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wejleewp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3usdtujts.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xgftqyiq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qnsjeaad.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3lkxcgrsi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3xseuanwp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yiztutql.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3edscnghn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ipkgwxnp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3oxpbxady.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdyltuwj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfumomsm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3olgauphm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gpdrrqri.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gpmdiuvy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3phjdfwra.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3rdrxouqr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ebqfhkvm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ygebkflq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3utakgkyo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3afzjkgap.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vqwmucuh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3chphukmh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xbzrczmc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3odszjeaq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3znvmzair.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ffscgfcf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cfnplrab.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ennwlsiq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ybgulcme.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ynymqrcf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fviacftm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3klvlrhit.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3pccgyidj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zlcvbxfm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3psqhnhbb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ktrqhqlm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mxqanpri.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hmcadvcc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dzgbohpy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dmwsizcl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3eykvwepl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rbmnyrte.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bjuhxslp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3elxkyjgk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gcsqksdm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3muxqaetj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3twwtcdcx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3vhcjqrxj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjmaaldw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3llaymvuc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3keeavvic.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3kxtirpem.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3swbfxodh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3shfvfbjh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xjgujdzf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lqiaypin.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qkraenxr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xykdvfqh.html


<!-- 参考信息 -->