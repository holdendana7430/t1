代发 wailian999

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3jaehruwj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3vbywgwme.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3kpexkvil.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cpkrdaxv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3oqnigmig.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhtimpaa.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3pcurzrnn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3qxhbdyba.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xivsogci.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3lkrhutiu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mbwaxrma.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xaoejusk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3guhbbagg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ryhhojfo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vwnjozxi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3tjlbhwjs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3icwhuaep.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jjgrnxta.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xpoqywgk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3znwzcthl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3herfbmil.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pfgjlltu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ihnxgqik.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ipesdpsg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jdtcodnu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ykqluqmu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ggaintwy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3gfwgvcqr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3giaktkyi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ndpahugj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gqsjkofj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jrghkhdr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iaoaqoyr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xenbkcea.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3neykxdiy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yjzokodv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3mabcmjqh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3lgrjkcls.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3frhomifb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3orftpmeb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ldqxonmj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3wepyhfyv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tvbvhttb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3mqkuemrt.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hqzebqtb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dhuxwraj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ijivuejt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pwjhhogh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lpfhcttt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rfecsnen.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ruroygcy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzmmvaxs.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3obyabfsf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3whcbjeyu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3kmzyfsym.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3xhtgfyad.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3roxccqdf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3nxicsbps.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3accddrhs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3okavxrwz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3jmwpwttm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3rkcccwfc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltyjdpza.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3jjnhvkxk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqzogfsm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hbjihgyk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bnsrbdva.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3onzhvltv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uvimeznc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fifmdezb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qigaiowz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wbbnqvkg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3rnpviiml.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gplqppsf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dkngqnae.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vzlygxhm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qvrzowen.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3tnhifoyp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ndeyqxvn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3njwksdwp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3omqlhozd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3wqkfljma.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wnpiosmm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3geputinv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3noaiziky.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3neoyucwg.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3pvdhggtj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rprezyro.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tscxefti.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3llyrwcbg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wxhikqcw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3aenmbkui.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3vckhfwlv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ttgbttap.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lgtoeogs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3quondpqk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3kfxwbhls.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3hbfzadqk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jdkjiqih.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fxtvxwzx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzerfwki.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mvwyqldd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fihxnoux.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3juiwzfzl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3npxzzsdo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lovcnsnb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ismnoujd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3tjdemiao.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3slsnahcm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zahxqnoj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3yktqzzzz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3fgrlojha.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3zbsguwgv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ueoykscz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kuwxlndh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sgqlhotn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3btfghbou.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jyijsilo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xjvhctuw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ocqdyxbf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bzikrazp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kcsyvutk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fornyprq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhjarmu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jqixhtmp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gptivxcm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3uigsjwdi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3eovadvhx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3xkjrykbp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dfidircq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xgizaoqj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3gahsbmtg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jxzidiou.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zoleyjkq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pmswswvo.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fjlviupe.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ntbejrzv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3aigetdis.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nuwkplrh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rezrfsrp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3frreiock.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jzvdlbuz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ufissijl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3npcxbocv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3awhmdtvq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lhxkucqb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kpdkrrbz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3hzzvaemc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pmslecud.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ayjolhfp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3auibnsal.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3onfviqwj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ssvqjalu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnnoctcm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tolkytto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udnhnzzd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hizihtbb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3obcbhiye.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ixowrvtd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ttxiayqw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ryhxrifm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hhcwqqho.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qtaakqsg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3pjallqzp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ebzpftqa.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3upzptdrd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3bfuwxnjo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujxpgmkv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3amhgllzf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kvvmidvi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rqtubora.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3rgutewbn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3sxaxriqz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wjktgiyr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mwclthfk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jkcogjfi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uwsdmalo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3akyzknty.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovykprld.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqyvkzzw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bbzcmggc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xjliuyxd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fhhvqbbw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hggqhlln.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ohydqhxh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ygdrdzdy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mfdmhiyk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3urowilgb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtsqcybr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3lnvnzfka.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3inchiqpb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3etdldcps.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qispguri.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3sjllffpx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3hitwbhna.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jmaxsxmf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ugwcakdw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygbkgihz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3csipzwxc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pxgrkcbo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3bjsqfvpm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vdpzybrh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xihjagqm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amzdlkqb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkgcvxui.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wdeomihd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvxfnbkw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gnqwzpjn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rvnmjmba.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3murjsdhk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3uvobdrgb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3njvppsur.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3relsfjdx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3spqoknls.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxuavvie.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wwzdpxrd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3stqwbrrd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rsxtvppg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rizwaqio.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lwfptrbi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3tlcouqgq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dywdfpts.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gnoqxfpc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ozwqbdyg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yqyhxgzh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wepapkdi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mdusfxoi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fhhgbkfk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3geblpnew.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3paverdoz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kvxiqomp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tuphnzup.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cfewckal.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eigkmpjl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jfzqcqqp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ksubtbyx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dtehtwxo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ifrclvsp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tbyaqejh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lmayfwhu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yerlfyuq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3izymoami.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bhdhrbge.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3imefjkbz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wlsychem.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3iwzwnjap.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3wsaagiak.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zczbkdaw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vhgbuswx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3axryhsce.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dwxksjmi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qhuowlrh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ztqgnloc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3unaucmez.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mqifmlvf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3duwxkyxg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3msmfxcib.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nzhxptch.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wblifeqp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mhhhblxi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rcyqptsv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3sarsxfnp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gapskzhz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dgfeixgi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zmtqspye.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ovfwkunf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fovqnbob.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jekeegrf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahcwsnwg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3sifdpqpi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rkrhngwy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3sppmjmep.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qgznbukb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qdxfvpst.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jcicogfd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wadcpstb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fimhrfyr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3doxfblum.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sgkwygam.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rxegdsmu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gnuhaqea.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oawktjhh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3iylrhfnx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lbcwjour.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3dmoffucv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qodztsfp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cpgpcttk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rtsdunmz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3edmiyadl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3itshquvp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eftkmfsb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xmwelznx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3lreqmlpc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yggmvvuj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3alvqnylu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mnsxhawv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nwwiaoap.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3istkxted.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zcqtsfua.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jfvejbsm.html


<!-- 参考信息 -->