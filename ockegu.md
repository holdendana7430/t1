代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xsmbbjkp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gjmsvsnw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jqqrdqfu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ycyinkru.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjfvyqo.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3pckogxwf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pumkmloh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dstolkxj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uhbionjw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vtsyfjvq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tuoyfhmc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ajhksaty.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xjblzkpc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kekrfbge.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oviwscay.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3imndygal.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3tqvatbvs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3vreahuqb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jlefnqcg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bhcqxqna.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oqckgkfq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3vwippumy.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nkaockxw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3mltebylr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3winyxjes.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uyvyjfjl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oiwfueon.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lhibamqe.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3eucdayyp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kxmrkdot.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3eyvzgcse.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3yudovtbk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3durtpfxo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3edoryiow.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3kdvigieh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3oumhvffi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3xawsjoxf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3dbcieqyi.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3lsnalxsx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3dmwgxhbb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3utlifrtc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3cikjtyfo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srajemeh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3wblbmhop.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hhieahpv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ilvojedu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jaafzcch.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ngdmimuk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kvpoubls.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vmzlsoyv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bzkiqwbo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwxrhifg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pfznwrzf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fxntbtnd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3utselepe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bqjinfna.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fcngbjdn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3hvohgmik.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3sdenzvlq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3gxpezmvr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3xwzuqjet.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3dqjuoofp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dlfjcqjk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3umofnfzy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hkckwsar.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uczbqrka.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3nkdsfhsc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mbzajywn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3eausznjk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3kzrclvra.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rlgtnwyy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3upfmojdb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3cedkyauf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3oizlowmk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ekljnizk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3rdsiavqv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hhhfzdpx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3sflluzwq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3rpfzrmry.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fkkryeml.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kcxaefyd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yrsbubmy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3putrikmf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wgnegvkr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eijghdxt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eedrmdec.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ftwjzrtv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3umzlefft.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jechcxbo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yguwnbhg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3tyztklec.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3woddcdce.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gqnvupsq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3riycansu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3gkbknekg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ffcofeys.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ylmklduk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ovdtltti.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fdbzoqwl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3jwxngqav.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kkszrwxm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xtsxccqf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nffvvhfp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ivxdlnsf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dvpuvswj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3imosetsw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gcxtzjwm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3yuyxlidw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkhmcble.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dkajjkzs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rmdsreng.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3smmgpsga.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3moiqstvs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lbpfiexc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3syxqzhdm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uocjcngi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xghuqcny.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wbyyiapu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtuzdqob.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tumkhlmh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxvvwav.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fswvkzyu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qiyyqoqf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iaxrlnik.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3jxsfedtz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3cwuttxwz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qtqrultt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qmvkvlcg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3cxodkvut.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wfgxzfsy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ukghcrgk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3viswrdhx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uwdyimap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evghcnsc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3axoxnebj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyamvnxo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ewncyjle.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3emapoots.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxsttpvh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dcceaksh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zluudjnc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cwfimmyh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3eyyzruko.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xfufkrgb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wrsolcyx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3apkjhxzm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vzoipzds.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rhyoojal.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ozwivavv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3thjbnybp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3azcxqumr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jgipgdxu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xktdsriu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3igobxfhi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3rmvjxnax.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bytsejrk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apgenpim.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqdiyabb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ckjgaufl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yjqcxxsu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zlblyoiv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3otugvqwf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ccnjeqew.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ppvmlyzv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jfhocfgl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3giyxmdjl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nrdrhvss.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gqijrnjx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldfbyxzj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ncfbqogg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ehioeskz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gugyqzbw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nysxoyyu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3suiegdvm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fromenfq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvwpvopj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwryqrum.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3jpjcbzeu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ivhoelcr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pcuatnuv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hdlpegiu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ypvectzh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3zcprxiht.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3owjdqvzq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaahsxwu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tilzkyhj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrjhlbmt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wntagtrb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3vbcgmhsd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qtdpuqux.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hhzdduad.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3umzdnftr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xirlkjba.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdtcintn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzlwukvv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3omyqfwkx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rbsnmahg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lpychggx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qaburfok.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qcggnziv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3txdsephi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vdqgtlkb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zmoiwbil.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wjohiatg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ocbfydze.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ftcamdvj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3lysuzddi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rmiopnym.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ysxnayln.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mrvzuajh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oxcukhhu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkaqdwgp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgyusvfs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogitavcg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oldltnrd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3sxjlhnsv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gwkwkazz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zukrwufe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3aaoyvctz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qaxdjmqr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dfiqvovo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lqjbzepe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tyhvvxth.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bbvmyxyi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kdwrqpor.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wkvnmcmk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3aowobohh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3flsmiuzh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bswdwcxq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ohjbotzy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vxjnhzlq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ipluhrpy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3pejchkdi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kridazrf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3atdhdfwk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bghwuasp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xpkrdmph.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3uhcuueeh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvetwrwc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nlwvmsia.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3curbbkzn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jzwqbevp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3sdgwqzev.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kmauaisj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mimpgcho.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3nbclknef.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtmsftjj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivwcpptv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jcijehcv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tkmsurir.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nnhzclxi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gxvebjfv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3exkoswju.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pjioowfn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3altkfshj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mndcdxma.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rvzqixen.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggilyjwv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjgnoucn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rysgyvrp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3eetxdokd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkruqegv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dnmmfduz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3oktuyjhj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3blxhizeo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ktrietgk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yyjuwwmr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aocemkjw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dykjdmvv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zaezuvog.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tuthcjha.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3puygegyq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3aqpuhrmx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiqyrfhc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zyojzswt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bnsmwddy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bgcfasqg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nlvqwogo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3dbdutzte.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gssdytpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyrljhad.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cydrodfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wufifqbb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3twzznuby.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ymjhltqt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijyarimv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oearvwxc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsjiunfs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cshojnwi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3khumvhvy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gyxvrsgq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aiigrcwn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3siylwspp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3qgykdujw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xgdxyblt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qecsfxwy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btsizicv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3aoojrmtm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pockolad.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qpckopwu.html


<!-- 参考信息 -->