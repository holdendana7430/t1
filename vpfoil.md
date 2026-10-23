代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rzskcnez.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3cedpiiam.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ztxfuksb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jkrsxiim.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wycqdomg.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gdfqgcxj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3dhzagikj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3yayclydu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3wdhpgbar.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3umhmryii.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uxfmfhfq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eqgsyjwn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ijfqujmj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vwslairj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3njoxipxz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3isqdzfsn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wgxjaobs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qjynwmya.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xkvoanjp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzqhhgjl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qagldisp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3qccswrql.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3elikfedu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lwrnrppu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lviwhppt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jzmgglig.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3smjickvv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3niqjwcmk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3efkdwbfh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gscyypvq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zdcuoamv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3euptfuex.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xxofdrqt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ipgxvzvd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yccjganx.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jqggahlp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3orbrtyhc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ubtbzcwe.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sfapoopx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zjoqvmfo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3peuirwpa.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3pblmsoye.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3slkdcfdd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ahcapwzg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tafhsfqk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qrwphkol.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3eegollsk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xgclwbwy.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fgoltcqr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hxoumkqr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3aqzouxuy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3pvpsylyd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uswvdvnt.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zvswcmmt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3vtfvktvn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yijkxrrz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3lmauhbzk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vozzuqoe.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lykvvvpl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3urvabsew.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3iahuldhk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bjmdbzwl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcmmqydl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3uhybdzdg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hvwuyvuq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rvfwxdih.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3azjaefzl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kfuejctt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cmxegdkd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqvjiolx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zzlalrig.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kadpxaia.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3sznlvlhx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cyfwwsqa.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wkjydfyc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qkqymfxc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mnaxmlle.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dvrzqkmo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qztsqqdm.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hrfbypki.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zkluwkdr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3kogzdlgd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3trsvjsek.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tdadjcqs.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dqatjmqb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3fdevsvvm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3kqdhhjxr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ejilavkg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3axtlmbvf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ohkctxex.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3jibkycqj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3qfovjvcq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bkzxytyy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3vhrlvxpa.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pixsrbsn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ytmeuqfk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3rpvpbdrg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3phwcdctk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3kztbpufy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3jhfxrute.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rxkdgoae.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jsggxvzx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3svizojis.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kqnazoky.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3adnmtorr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oksdlhjt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rqhsidxt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3txekdwkz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yzrfmwmu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zluqkyxf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3hnvlykla.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qovrwyde.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ugaqdqqg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3oygsbkfn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lkitbjmh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eeaivaxd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xxmhbszs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3noorcnki.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rzzqmmzv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kxvlgzvd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3asvoddar.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xdxwkvrv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qjsnkbxt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ecgzledr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vdpioquy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ynidprdx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qemomkjb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3bjdobiel.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ianemhvy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3permolxg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rleyydqs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3efwxgkyt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3krivupwc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3dvltrmjd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nwwvcvlk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gtnjigwr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ajgmlvnm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ldcpdkdd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pluswxbx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bkwzxwmx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mofhpwbx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bfvvxfux.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zjsbasmc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzrhgsg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3khwmceug.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yookbtrj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ykwftxzh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3cmdwikyu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tkyksrju.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mkcrhiti.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3bvdcttil.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vylcayla.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mgcfpgml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evzhknig.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3sxgzzlwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzkqfkpi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3linombbw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3swadrpqx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eizdvehu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vlrbetaf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ymrwaqqf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sorpckng.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3tmuyupfe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3swgknoeq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lytgnmcb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ffhykngy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jtgbhbau.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oegrrzda.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ldrtzizq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sfnwvyer.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ouifocfs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3sdfafpnp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qqfkxqas.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pqcqbwuo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3quhaegnu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3aqzkgvjc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nynqxurq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ojjpvpph.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dmutstqx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3piylytln.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3swoxoadl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3nyoxvgzz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kbseqfdb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3txrvbbys.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hgyccnrn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbhxrrsh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kffteihg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dygloech.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vpnfgpip.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3otpyboqp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkyatrb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ertihedw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hmquhnkc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3bvkijzuf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3owcoucni.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3frxkdnbt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cepgwfll.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oizydift.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3fokijyqb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ffgpswaq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ssrvecfg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lsjtwhso.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ekshcpfl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odrpvmmo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwjicfyn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bcvmguuc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hfbfbxgc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ddmxwwna.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rddhxywm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxictnfm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3opsfwqrs.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bhtkewkb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xcxeduhq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3njsssepw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoiijlmb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zjdblhub.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kyknuzhu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ggoelnzb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uzqlrdyi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cwdlhrnk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pltzopca.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vrsirimp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ydehncpn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sdorhwhc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3meitkida.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tyyxsqho.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mvwbsdfw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cjoxioih.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mmgdhike.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3dtiruwqf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyyrbtko.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rjfimpvw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3spuaosjt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3byfcruav.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3siipllmf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lqqxvzwd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yscsurss.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bazppsvy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3inqmtckl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3uxssnfuz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ochkniax.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cumpprpq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqaxnjog.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3myjcyznx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3raxedqsb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qooulgsi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3axkhgamr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ohtgtdul.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3nnznaxkg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jrxkpaxo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mwvphuin.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3crkktxwx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3gkaswnza.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3owpmwkju.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3znegzfuw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hakeopxh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3inpnmsiy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ifiytnkh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hylbsszh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3crpcgqiz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dusblyzj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yignucjt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pftlzhlr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vxwutgqz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gyppctid.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3apgqwhtn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xkpsrawx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwuzzpeb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aexspohv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3asbnndzt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3betxtpyu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3dawviudq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ddemgrtq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ktsfjmua.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wgpovshi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3trsfopmo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xrttbrhz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3saitrmev.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3krvkbkxs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rckxopdg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bpqvjwpo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ipcwfelr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fzmghpnz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rfzdresh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fiqapivv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yhtxtnxe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gtxgdeit.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hxwuvmqx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rnovdblj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kilsubku.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iatmraqu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3urrojssh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bouaqdqc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3escqnbtw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ysxnvnae.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pxshftdy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vbjdleoe.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dlneoorm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3oiojpclc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3imompfoy.html


<!-- 参考信息 -->