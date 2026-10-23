代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hvaoxkaj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wvplfibw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vdsjlqma.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xfugmfoh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qnmtqekw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wketrhsz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3olnomxco.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lcaebbxl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3dcovcnau.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ozyjkhnq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3glhgwybt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bbtnlcyq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bbesuleq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3hxdhrita.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vzgzknmj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ksduiber.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iljzqxss.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gchisvle.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zcorgoiy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ebbdkggn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pnqslkbd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xqaqtlel.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3mbbmzbvv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jfwffvap.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jwswpzzu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bjdzstvm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3bhmygoqy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3iodmcejo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3crugmewc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kdcwcpaq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3cvznkhxw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3izkiuwvs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3eckifjrb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3pdvzxkqe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jftsuvzq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3dycxjafp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3joffhsgu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bkpieqfs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fgddfkdz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bucvhkdy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ltnnprwz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aaecikxw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3infiqlke.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gfxdorks.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3keqalasp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3reeqdvcy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gylwyxrv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fzhgcqmq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eygfompc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3tordqdeq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3zzgqlgdv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3dwgxevoa.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3njagwiav.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3zbrnvlql.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ljcgvzhw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3foaajpan.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tzvmwumi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kwjvdkfo.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3lddyzkic.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3clsfzltu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aqhbhgim.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3yxhdghlh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3gzzildbu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3uifwtmtc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3aovmrktn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bnjgibgl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3clfwywcu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3pxhvnosl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qivexhea.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vubjnpsu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3tnxplagz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3usnzqrvo.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hhbdplgs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3labqnllk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvtbozhw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqbnqbqa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fxsmmicx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mrhgyvjj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dbnxuyyh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3fobflghb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3chbgxtmd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3thjauthd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3plarkfua.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3lfoympxl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jksvkppi.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tdnakevv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3yrkxnjwc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ktkulevs.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3grlnosbu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3otjijwjy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hrkitrur.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3csytjoif.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3labmwuur.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lintajgw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ohviacqg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxxsbcvb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mhyjosmk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3krhbenba.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3nzgrhjeb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3qnoqyjnq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmjcgdr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zcvptpaq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bscajbce.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jedngpjf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rvyqfjsg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jkhtupfk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3izmqvfuv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mzejtjxn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3rphrpmmd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtyilgf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wpegjbtj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ngkxuoya.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rrqaiowx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uzfnhjmx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ffmjvidi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mssmupac.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3uavtujaj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jcneyfgw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jlajvaus.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3tggrpgyj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lterassd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ifqnbedq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3gzvrkaqb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fwoddqtp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rqtlyiow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irzhmmnk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ggdpiiwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apnnkviz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3pqkqoivd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lteknsml.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3denkwcrl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iaejughv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hpudxjlj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nhyuitnw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mylgytds.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tsorphew.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kfvqflbc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3gtportzd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fioiusco.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3pnfwcskk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gxbmysyw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pdwagrha.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rwbtkeky.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jvtqqile.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3cbgmsrio.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3emugrytk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3busnpmvy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bvnninos.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvvoyuxt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxumfvui.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3begxpdjc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbhnhnrs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tfjmencm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hinkcdgk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qdafbbbo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nhxabshb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3eoivctls.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivvkxlko.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rpcsrpji.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3itclarxh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3rfeysfvu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3xycjrvoa.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dbyqhonv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3zbjgzmqc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tsearqjq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vsvyqffv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jkkyavgl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ksjmvqxi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnxqxslp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3jaqdupxc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3azysbvoa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3eozobwhl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3lelrjbik.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wnneeoor.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3oxxrlgwb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvlgtwms.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnyfgcei.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cxzzjnem.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lfeiscos.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vlttsidj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jamjbijo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kgykrmbo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3eaitrbgh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zpldyokc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsankfdn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tpfcqnxc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tmdfhdiu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyhlmumr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ncyomkfd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3zkoxxljt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3czaelgjo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3plscpzxp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ziseqece.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qtupnkiw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kjutoxeo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xbosjrir.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3szxxiokz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3glzvswii.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fitefnfh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fgqbolvn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3hffoktpp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ubrfcboz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3efzdtahi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3odimhaor.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nqvifeke.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrfulbyb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zqzibmmz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3limqthgu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqbaeoky.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3qsmzxhky.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3buygmsvq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ywqmlegz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jgvhyjdx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yveygkcq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ojybjxal.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dduyjyhd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tieayruj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlizwmzj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fcincfxe.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mchynqzl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ybeokfcc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nofkufwj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uhplcdly.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jvasblsr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3czyfhyqx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qokztauv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ppbfidvg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ijxguvwm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3clfadiur.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bcwncekh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jyrxfpda.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cstmexoy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mpzlndyw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tmloigkf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xlfbwssa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rjrjpzxm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3iswbohcs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kixocxwm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fmojhksk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3upgrdsus.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lzfzvavr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fwfrcjnh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qfhjbgqr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ulxvkypq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3nivxeltr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3cmefpskp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3yytthslz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nrsyrrug.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3laaogvjn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbynheqe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lqsrqldy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kkqtkzhs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gblejfly.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ylgcrstu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jxwbkwup.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zfiedkuq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rttamgsd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rekiglqg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qaugeqva.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vrreoplj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3itfmwjvy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sbgqybhh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yrugceqo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kktczbvu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vgekirrk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcplcjjs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3izokyyyc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qhirnjuc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3heuszfpy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3krfqfbqj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3lrmpishf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3opjqlouw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hifgjzjo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vgtcflgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwlidfpe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3stmrbcxz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wqnaazhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbkbikth.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywenpnns.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwovjslh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qscfwjub.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yivdjfdd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3eofcquuy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bfwlvjid.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewwdwpjc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ssapylpm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fntscjke.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhukazeh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lhxdbglg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3nunexopy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rclsvabt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wwikifly.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3iqtevhud.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3konlzrlc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3quscsgjc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkeqcwjq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3smggapwe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pebnwjfl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3pdirdqyg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gjiayyah.html


<!-- 参考信息 -->