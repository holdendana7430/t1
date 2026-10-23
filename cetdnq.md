代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gyskqqnb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3biitunkn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brlngeqe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oauxnuss.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ujyttnyt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yfqaevqb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3tettuzpa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrxstipi.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3dkzwwetx.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3egbrdikm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ddwdlbxg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ylfxskai.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3eririjwj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pawxykjn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3zgasxhwq.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3umbwstjq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3umxjjwbb.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3hclwiang.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ovnvgaij.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ldkymywn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xngvvacw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vjpgbcpe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wmszhryu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wpmgxpio.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tajrgmdg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qribhjhf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3chcalayk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3rjuxhlad.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3loqculru.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3obxlwprj.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3yngudikd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3sywlkosp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3bbgpcblb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3knzbincc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tsibzlej.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3zawjzkyf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cfuolgrz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ayjueklt.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3smumrwov.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ovwwmorr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hokymlro.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bqhwumws.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lavcdfbv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gbhnxkjn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3zoazcdju.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3nktzunmx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rdtsrpnt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qwvrxmqx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3balyewmf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3gxavzkhe.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sejuipiw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3chfptkrq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3czxwwomg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3llaocetc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tcxlcrgx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3asfaacfn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yhzznpja.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wuayaykn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hynyhmvf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwseqyk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tailomnj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ccqyzmyi.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3rcmyjazf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hgsvoeai.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3iibycfto.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3lilheafs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqbuwjtj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygxymkwi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3gbazygrg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3pqjljoab.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgahzpbh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qjfdwpmy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kwhzzwwk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3engjwumn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jucncjfg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kgfdbuac.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wsxujycl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cevabfgx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3njuuaqqg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pyaqggxd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3yictoqgq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3uptrlmni.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3elvembpu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wpmxyaqo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jqizhhys.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3nmawfkra.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3tlorwcqm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hwzwtxdn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mpnefxvu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cjvuuqzb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ksdlvrit.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3qusqqaqt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3smcnqnxn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qqtrbkfp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3dstggjtu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3adotuesx.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3swoywzrr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3kzbmctbf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3riqyfrvt.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3fejficnm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3amympjub.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vhpjeolv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ketezvsm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3wmtbzlff.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tzmrbznj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wdrkotcq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3phxbbqcx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xzikhwed.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3goomuaob.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nhiswits.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zizalusp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vnliknum.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lgfaheak.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jxrbgrav.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yfocejdc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3qsafesfe.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oceqwwaf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3rwanmnik.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3pyoxpikf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ookgessh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jfemjgwc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lugucxuj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3mokekmcc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3dujupail.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3efntqkyc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bpscyeym.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ksjhafwl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3dvapumoj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gcjaoinj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mfbqlyad.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3suzrtfcb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jfgyibhu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hlydsuwp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3hzwtwepu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hbzcklnp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3baacqwrs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmyvnwcu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yshlzmyl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3psumiqpl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mikcbqtb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3daotxfus.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3smalcnoe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zrwmxefd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qibpdwxv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3nwwhzdfu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcnuvmgp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xictxnys.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ppjvcqbt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3esgtvxrw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aaczkzdh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3mozdmkpn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbocsjuh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3gzfaezfx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3fzfofizr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3vcmomdbe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3mfzrizug.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3obncgeeq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tqtoxkky.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3wbdhktoc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hpyfcrad.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3svkahvuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyjdkpvf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ywebrknv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slvclpjy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kpzhowfr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vdgeoaqf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3vyaahioe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ktwiflle.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gqzmdhjy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xemxcqig.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dvgxvtqf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3orrwfuoa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qfzmzonv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zdeqkboy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bspupcsb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3sdzftfmi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kgcubemb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xndujsuo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aruhizla.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lnxlgwbk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3udbdwnrk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vhmkppws.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3lfwfywis.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lsomzigt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xnjaazav.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3woxpktpr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dcsemlbs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wlgwdrhu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tocqnxkh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bynokpvd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jpixezzj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jwdaxmtf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3utgwjlwv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ldsfmmrz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3chjaalyn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eftnglss.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tugarbts.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3txchscis.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fejghizc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgodzutk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3juwylosb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gbjjupar.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbfmezzc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3erfmbutj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yuiuxkrv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3srpaghkq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bzlkfgfh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jfgkygvp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3imwnuzdz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tztynlpt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qwvenzrk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3sjapvuii.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xormcpil.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3exwtvtsf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3mhaymldx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3dnwpniyn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3juleisld.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3epycrzlm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3aompisdy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jqzmbcni.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqrzyldv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3goqlxpxj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nupfbvlm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3glnsiaec.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ozodqdip.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3dulgwxzf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rvgownri.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3smyftpow.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xzgfsijw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nisdyfwx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3guppejov.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dvpyhnmd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ngmzvbfv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wlbwvxzx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3yozmxiqf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uwcfnxgd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3racdgwmk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jpnpftcf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpbsftjb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjxynckc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyshvedz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyitxncv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wjrwysic.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zutyovsm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3grfzdoyr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mtvedejh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tcqmhmza.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvhxirfa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3uqboxakh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pveoscbu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kfmcbaum.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qevufmnd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vqbezaqd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3izrfxvrs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cecruawl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3icarfdyz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fhpchplo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gutbjzma.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kupyiypl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cyxgulot.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ccbytsoa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3saqbsvlr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nphguhgd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nlcvqxuv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vtcafywf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3aebikztp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vlhvokox.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vqrwrocs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xgkxmepi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3crbzqbpd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ketlddoy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vgrgiluh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xicumufr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qsbpfaxf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tnmdtkoh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udcnfawc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykfqdeez.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dxouqgjg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qagdrlyd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3guceommm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3habpcreg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lsgmlnsr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ojauccxc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3yneuhlfo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ewebkcsc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnypnhfb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iiotfkpr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bxiustxw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvxpvvlc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vasuxhog.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3lypznjcu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3iyzdacce.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3kawzfgoe.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3demeqeqp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zzuaaspd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ilvfnyed.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lcszfhdu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uclbvlqx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jpzqpnjq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iquzivzl.html


<!-- 参考信息 -->