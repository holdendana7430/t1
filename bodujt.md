代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wakekyeq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3owqbzyws.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3knqerhiy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3rbjpxiis.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3czqzvwjc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cglzmbgs.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sowsgfly.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cyqlbiqh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xehlyjss.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3efveclbj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3lhvejzpr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3wettdjau.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ehbsrvqm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kspghgxd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3tpwjzvuc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xcpjhnfg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ymogeezj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3frfzhegr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dgnvponi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fiionurh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3fqylaiwy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gjiyiorq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qmrlpbdt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3jtnjslwh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jyiksotm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yumrhcbn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yjignawn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ooxhopej.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kklmnsqs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vzlmrcpe.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qyyyuezo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmptjdgy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3lybfbmlh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jrfoukhy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gywwmgwm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cusvkzqw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xpgarsfa.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ywknvfxr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3anrafodz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ohqykqcf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ysavxaux.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ccyyfime.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3onyhzbop.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3aibmhwul.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zeyqljkb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mbxgxjka.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3rzrmvxrl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hkcjlwfu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wfpkfobu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3cydxfpvi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3scjclxan.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ulgtadge.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3dwklohzq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bufknagl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rqvvmhrv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3vuvazvfm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ampmtehj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wopmxruq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3nkhxcaim.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fkpbdgwl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3chzrbflm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3scvdmatk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfipjled.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bzluetjq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pchhekbo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pbpydmwi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3knwlltnx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ezovrfvj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3phwluvhn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoggijhr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3duzobzpd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3vuluivet.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3dtcafyuw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3sgxbxbwp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3urlmrhkz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tdcbjkzj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dxemgmmz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ggkhpiao.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3avskjuyf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3jmrvkmxj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vqzcivnh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3goixfhzs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pvfzkvba.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3cjsmjvhs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zpodwxfx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tpixmchp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ftfsyxxx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qianhcax.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3qwxiibso.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3eofjtcdm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jazbxsan.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3aresjzgh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3mngtobwb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3pmryvcrm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zwvnggqu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xfrylqpe.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3saqgqquo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3yckdagvi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pjmxftwb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lpagpihk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jehfgmfk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtqpewu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3meclzymc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jayrewzj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qbyjqved.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3uwsegwhj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3zsgghjeo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qdkjhbuk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rqvsgvvb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3oyxrtrek.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ahmxcvyi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nznwdfuz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3upuqdzjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3haxdaihk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3jnrjjgfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcftzecu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gjotfjuq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3trnkllck.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3obxkwzlq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pufbsajc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3boplhfyc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vltmxqij.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kzqoxngx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qevzleua.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uekfygcu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yicwvgze.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nwgjfjlv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3girwdktp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mdrdwnvg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3akvekies.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uvlsaspf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3khlwofxq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3sxxdwwks.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pcwrxdeu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3brexwtfd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3niqhexfn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ypiqfisf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3akuxavbs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdpcgxdj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ibdupajq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uyswnrdc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xvfnshnj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rlarjlvi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bpfltpjt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fimlqrxi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3pawmbsvt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mkccjnyv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3szdczpie.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzkgbnlq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cjlshnkk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hrhrxexi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfagykml.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ubzcylbu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kkgokqwn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3uzeovger.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdznmqqr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhxlpcwp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrhlupxo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lvchygrh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3iqpuqull.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rkkosccd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3dthrcqqf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qjhnulfz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfbevhjo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhemkohj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3klsquwze.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3mbiboiqd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zdrxrpay.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3undwegww.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dczthamy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qupqbtmc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3boidztod.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtwhaear.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3opfcnlsf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsxzpcdm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lncerene.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3alpgdviq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lysnelqn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueohfzxw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3glgxyvfe.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3veitaxgs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wxojcerz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qqfrpyuv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gszgewgg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vscpaowi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mrtvylfu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tugguubo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lmqbjpdz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3nhxggatl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yahjpxgl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bjnitmwy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcnhehho.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cscqsgqa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyuiwnof.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3njxivnou.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xciuubhi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvearmcc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wngksper.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uogpupao.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oosxzffj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bxdumjlb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3guquyqvi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrpviegr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nqmvjveb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oyhnxfvx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lohawzec.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vzqahify.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qmsnodop.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3enbdyxmx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xbeyldhf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eexxdesx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3undvbksc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3yeslmqii.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zedhnjab.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vrowaugh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vhkljuys.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ipkytmgy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rlxhnelx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pokzullf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kmbezpcp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3attnrmai.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3aukkapdm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3pyludrhq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xavdcznn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jiwrfjot.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3uhnroqkj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qokqibiq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxbdjigd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sbfsqawp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wcoebjml.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pizrtnri.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lvpbirmk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wozdhovf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xwyfiykr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3nwvrckir.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tnspurqz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nitkjvoa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xshdjeyh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eozvmyjj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qggzplms.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jzdxxrpb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3otbwvmck.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bvjholkd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hdzxwzwi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rrnkbvhj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lyzibspl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dbmccjwf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kwlyrvkh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xjehxfkk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pbdghita.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jjmtxruh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3alggictr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3sfxlhewm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcnvxhx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3greomrjr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dnldnsen.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yoqyergw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nuwcfqlq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zmejcsoo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3teeevsdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxzpzliy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hppqvvxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbqlzdvw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ujvvmqob.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3aqqndicl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbegfcej.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wztrplid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nhhvbgms.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cofrejrk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3wvpqilxw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fyqqsnun.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yasgjrqn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltmzezpp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uzpbrgdi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3uamemtty.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnsloepu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlhkggut.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3asovhueo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tajvxvbq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rlfrlfbn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dbkmevlt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntpwepbi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fdihjchs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3shgtnawg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvvriqqg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcucpali.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xayutmww.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3maxuiaic.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3clqxlxcl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tvuvlcxn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3shtrrhcl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3dpwrrjpr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nhiejwro.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrekkdhr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3iwhugwlg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ronsbtva.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lkmmpukz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ehwnumqs.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czzvteax.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xiefiiku.html


<!-- 参考信息 -->