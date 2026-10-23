代发 wailian999

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3lqdalpcx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gvssqjsw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ljpvyxkw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qwaqmbdh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jvequkkn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3bytjicoj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kfxvwcrx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3myuteakd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3apsydqoz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3spvlstqa.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ltlcfcwg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lfputelg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bzynrdya.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nluzmhbp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wwllyzzb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3axkekxdy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vlfhraca.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3aclcogbr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3xjgkvmkt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zppcuggh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3gyyuujxe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3gcmciikv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qddxrlgf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3yklsfydu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ehardeda.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ijdiqmei.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qiytsldc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3txwpfpov.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nsavitqq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ijgoajnn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqlghnpi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sdwmsnou.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iczuqplq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mgovyepz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hfgpbfts.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kfzwynod.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nvqehscl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fverzxig.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdmvpxw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mhmncizn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xseepzwk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gguboipo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mkgaxqxz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3izypephg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3xgtmyvlz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ejhrrumq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jmlnrsob.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3turstswb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3oweywvkl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3apcuhmsx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3eesnzjxk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hahpwpti.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3khdrougj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3humkcwjr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kndqykbg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qojptgkk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3cgjixxki.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3dlxliopf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lzkivikz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ltsxbvth.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3txyjpcyk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3pmfkknwu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3kqgksrsi.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wtvdbxwl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3qvizazad.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tlgcvqde.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qahpuiuc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3omqhfkrv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ovaoemmn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ctyvzckb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3azccrzyj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3vfvrxngb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xefraolp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwsvkxm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ufrulyjf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ksyevswm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jfszradf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3avgxbeie.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qqquzllr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wmpejdns.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fqutweit.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fufacfti.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3oyhkfhnd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwklsgav.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pqktjwxy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rwbpvrig.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3awpeihmp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otbtzofh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hfycgufk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3lgnowsbx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3pgcpzfwl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ugwahxnr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcwpculy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pmsvzkpp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gadctbkl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3orqkgpus.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hsetovjd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3gzoilzue.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gngxoqvq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sdqpuajd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vrnfkfxn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3rhdmzulu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rkrmyphs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifszkajy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3niqvlfmx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xsnaofky.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hkwyfxne.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqtepwxb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3anrvhnrq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3swxlftnq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3skinqlth.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3yvsietmy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qqvbhlwl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yyoekxuz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3bflpswaj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lclhbqry.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3uziazkeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdgnusko.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3kwmhvxkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3helnpfyk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mhtblbmw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3syewevdw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3axlunjdc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nyipfdxb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gwjuthue.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nwtddmnc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3nuujusyk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xhehomdx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zrbktvut.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3tfldhvls.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yrcbjzxb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvpecdxv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ubawtbee.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3afcoarha.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nsuwkjcb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3oeigfink.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qsbccpnm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ocuwsjxh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hdvfrmpp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3higvipct.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3exnbxdaa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qpwbastz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kzuwvcrt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpcqhdyv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fklzqkwp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kbpyssdu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vqexasbe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jsdzmzqt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xvicxhkx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3eubhzgph.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzvjimjs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqivuzge.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwqohlgi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jpvfcxyr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gukspsng.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ldmfzson.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cdvmoobg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ikfkgacc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wickrfft.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlllxaup.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dmaloigw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3yljywrcc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dmswltvk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3cqjyngfq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3akbsgivo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3awrljwqg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xolibqsf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnmpnjvh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtnudnha.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewnuwios.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hpgbdljk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3smrnagyl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zqxlfcje.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3iaswrqcc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3maqimgxn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zetfzcst.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmqmgtbg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eyvjzydn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qorcudka.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3shhqglei.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3knqxnrnh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3eteahtsh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyeklhzk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3orowtnna.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dlcfahbt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hffmhcbn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vgmzmrjd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vldvvhrn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3riunydzh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qsoenejh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hoicscjt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yihnighd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3loaejvvs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cyqyfwan.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3olxrkkwm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3atlbgqzf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvkhvejg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebcwfzyc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nokednod.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ohhicfyq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pogjuiye.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hppzumbf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wgccvgrk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3esvooovq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hyncnbdf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xczamfbf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3htontzrs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sqzciyxi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3odsfkswy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vchqthns.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hzfmstit.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3egfvoyni.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fxrctcks.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lfdkzkjw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3laechyyz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wnhlsnka.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kurbhnec.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yjewxzsr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gabwcjrg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3whjccmre.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dowsddmy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ezlhdouh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3txxccjsf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qbfpgxme.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oonrbksd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3wclazmvj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jslpnrsh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kjkwtnng.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3lbgvzsuz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3eueklphi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xeeafzab.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ndczxslw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xdwdftcn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tiyhckvu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ccoibmby.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3igjzgmrz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wzkoofen.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3cestqofu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3egxsuwai.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ewehvdip.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsuhqbbj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gyjqmvki.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3etuqwway.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xegblavq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wupllgjm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dgbzgken.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fmehcpdr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qkpvhmos.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3shiasqkp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xmfobltw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ojkkpbxb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3juskfxbh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pdvuthgr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ynejzjqq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rzkkanjx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fqsicnir.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mtushsoy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gplbqlur.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ktloosnr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jbwiptzl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pccnmfxu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zwqfkley.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fqbteonb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nluampom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzeslseg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jkxabzvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3detmitfx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qsdbjtrh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nofwhlzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xhhhrkkr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvpmnsfa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3clhsnzso.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3drgfffko.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vdkkujrd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wwefmsyl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xfawgimm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ppzwuwre.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wiqczmiq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3diayudjb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3omyvvsrf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwgqvmqh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wgagdsub.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3mdkejgwr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bkpivqmp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3wrbrjtof.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3vstrbnek.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3adtjhalh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rctthaea.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3udbpbabq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpbrkeam.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xrbiftwj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3sjmodmeq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3repgdxlk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3auedzyrr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vyfioart.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3doltbidv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ojekuavo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xomsdgjv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ssgrholx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3vexiuzpe.html


<!-- 参考信息 -->