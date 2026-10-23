代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dsvhchvp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nptphlzp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3zdtlnhxr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ykdhhfvy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jvsmcuhn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pzluveet.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3tingbsnh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zowbkmgq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3dppyzyeq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3kpfjncrz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3upzufvwy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eundmwod.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3anjygoow.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ugvsirkd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3axvfowge.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ciwfvpwc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bbztzysc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3khcwjavd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vfkewkoe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qnjitnig.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tjthlsik.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oszecium.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3olupcfin.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sabrksgp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3khorqhhd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcuujry.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xnfeveny.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hdhcsjhz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kysywcwn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3seidjvyx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rftidgfu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jchspqfx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3wqbhttrx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmkknlxr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yqczgplz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mfwevpxt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hthwwakr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fvpcffwb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3shfjjfav.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fejvctod.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mvozvrod.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3bopuxmtk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tygjeguu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3idpwoekc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gmifgnmn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ujddvjjg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jxfzzrbw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jfzjwxax.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3xyroeqeo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3nethyyuz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3tyaqcvop.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fzdfsgbv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3btaaojwl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xbrhdvhz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ksjhviwc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwrgjydj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ixlscezk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vgfkidvm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pfgagmww.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cquygpcz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uohyocdw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3epbdhrmi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vqrvxdbh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3uskyohhx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lqeutsep.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rgumqkkw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3rgckyrpn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ahlrshhj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lggwuctf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ymbqhudx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rcejdiqy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3qvvichnj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nepbbbmh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mcfchkms.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gylgjgng.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kuuqpuva.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lobokamj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3efoajubc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3duzwnuug.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nznepkoo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3edczuyrl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uyhhczhj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nokarkij.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dfmydkdy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3baoibsru.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3edfdhhbz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tyzhaesw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hhtmiqua.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3lzhxvxad.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ulwttndy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkygrftt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3guaftkzh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iwcbiirh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tyxkijga.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ufmoraio.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wjcntdwi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qipoberp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xhswxfnq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3brwifkfx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3lvlznyjg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fdfptdon.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pjmgemjg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3cjmqaofi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3mobjonvc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hodxvxzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnwbccxy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3mggshjzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmanegqz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3clkqxfqk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3heemjodu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uakoxtua.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ozrwsuyl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3asqflvrb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ipvmrihb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ahkygbkv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bcaifrxy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jypzsoft.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3spqgaipf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3dzahmjkd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfzwjrjf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yjdnxiue.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yghmkooa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aphscthu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xsxivmqu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3njvybiwj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hvnykuxi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wdpmzpie.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wxilktei.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yvjldcex.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ckryggsl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcpdbgrk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3inzpazgd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3giycdrio.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qwsskwqi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3humcfuqu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tfviqwui.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3cjcrwfvu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmlufflt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijrfiyrs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqcrpadv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gwffdboi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zrqmbiug.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nxwxvcfa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyggtdtc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gnqhfdsw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ajxqbfot.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3drbjpqej.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqjywmwj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sakcqjyt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3tgbydzuo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mtbdqsnl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pnoadngy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtrcyowd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tdjqkjta.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3puvuflxr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rzygmckv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3azhdzucv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vjoiabqq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkdbngle.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkcoljl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fsjqolkg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ahjeablc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3rjomisij.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3spzrhamu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjmhdkqy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbihackk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xevbwffx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uszylzru.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mszwydrh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ugwlcpme.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ghhsordd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gckqxmvd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ukbfhxdw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vrqdjups.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3seuggsww.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vvswneax.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wmrmmlpo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzjcgxtx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3jmazvksk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3huycxnco.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gsekaeqk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ktseuurg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hjscwybk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3smplivsp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3apnyikbp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lcbehoad.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uakffels.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3nnnxlqgi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uagrykkg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bavgkdej.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3flviwkdo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lohhbmaz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ixopdoir.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ilmpicij.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hehktgaa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tpbzbzis.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tqeiihwl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jntnvtdb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cdshognz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fdqctipw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3skwlxkar.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3varksobi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qndqwlbs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3blxpyyzp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3aiyqxbng.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hdyxijfp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pyyalrvp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmillcuj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jkzrnolw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3liiphktw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jtngfsmp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eqkukizo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ewfyesoa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3empkuwkm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pwjvcrxh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vyhlinaz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xidejssd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3csznojcl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3yahqanhj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3npcnbioy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xosfosrr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rdkwtmzr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jebzztni.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xwigkmdj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bqbixzyu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bdnqdslo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mnxkmjgh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3rzxllbnc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3njhxauxx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3coqojucc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3adsdysdf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iikddvel.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjbouzqb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qyefzzut.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3supujrnn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cijnsygv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tcdnncoq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rltxanbm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qsqvxglc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ceiemfbd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oxpplqbz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pdlbcobt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3onycliiu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dqxstskx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3lqtdrtmf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3alrxenzl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3duzxokso.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nghftzza.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3phhkkuap.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wgdilurd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qgnaqtpu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jgvwoxgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nepqwylb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cunwfkef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btggyiky.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrvqkfjg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3erapkllj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynbacbco.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjbyrksy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gwjsqziq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3akmwvric.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wovgjtpi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vlrcvfcw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qhmfzfix.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tolrpicn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ozushdch.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylzodccl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysbpmiaf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ryhmqepr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ekrifbkr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylxppmjs.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vgzcjfhd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vlbpyawg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jqxsocde.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3gkcvhoxb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hphmhale.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yeqsexef.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bmzmchps.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hkzzbsri.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3egsjsmgz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hzswzruj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yowsllvp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujduqlww.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3fzoqsadq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ytztpsiz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvnhegib.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gtxduxlq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3otsdmnke.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gsrkkmmk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wbhtebxh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nebneaez.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3tnyujvxe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yzbnnzoz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3zyuzugyy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eddzkmjx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3oduurtfv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3feniraed.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3atfxpucd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hsxlgtbq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3azlxxynu.html


<!-- 参考信息 -->