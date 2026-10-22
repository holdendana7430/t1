代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ubibnsui.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nyazopuj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2rldknldn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhxgrcvj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2flpeczbv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2yabvjamc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2pungplkh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yestebvz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zkgcdukh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ewugwmqw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nwfwxbhb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ywnmdljr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2pobwmsph.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dakyokna.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kzxbkxaf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ripgjfpm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2snyzppgd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qjnvkvxg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eycbyqdu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2nzfafhsa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yoevbmfm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zyzycjaq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2zfhzinrt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rbujylfg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2mzllgomt.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vrdrapzb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gnxmuxmv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ppjttdsx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xzemplvm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2uuahunyd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2udawjtvk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ywlyosgw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ycldvyhp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nocjupmj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qvijvosq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ojgjlmns.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2anspxcrq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jxizwubx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2unpsktmj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2imnzzfsd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2yqcpyxxx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2lxhcgkvd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sdxftjqm.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bwlcjeay.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2skchuxzg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2kukomron.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qbvqbmdg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qghifwfd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wwjineze.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ppxsuwug.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kxpgmbub.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wurycdgh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2irwpyxwu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ctjbmixh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2cfperprf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2mchuspze.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sijwofmm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2oggdfbbz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2kdytekde.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vnvkuxdg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ljdwyvjt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2kxhgokkx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2eqvmphnv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgbuskav.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2egmyzzss.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xuwudmgu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxglcvvv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hmbktvgs.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bhydocro.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qpxdfhhl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zrxbqycp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nhiroget.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iwtxlzgl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2utpdficd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cvjhrlny.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqwicnlr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ymlhnnbf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xbswpzzt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2gietumhe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2regbdkng.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bvbjiwmb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2iflrwbdl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2trhcjida.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2pcmqhhzn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ginunxwg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2zbafzosm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eqfbluqb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2puotcfme.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xsmgabac.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jakwswpo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dvjffeap.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ngqkzgxh.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mxbfqmwo.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2nzxdgfdg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2votcrhyc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2qkworbbf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2aeenfljj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2dfqjdunq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2konximxy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2gluccwqr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xgtvfgqs.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2nxghkzcc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xhvhapkw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ykxhquhq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2kokfzwfl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nmtohobv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ezqkrldh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqbytkxl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ldgmymef.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2koevmzny.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nwvnijxi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rxelnoiu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2crijebjo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uyrbrtse.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2uznsmigl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2fxkkyhed.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2uckaqafu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hwigujcp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ujxexmmh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2thpktrai.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pvzvafkj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tbvceaqc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2coipcijt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zeirxgzt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tmwydqjo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dbinnqwd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sgglfgul.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmburorl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pkztfajx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ugciyelo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2pvjlakzg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gctmpsmn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2bpmelvdq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kskorryl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bpitrpjl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2bxaplhmu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqnokwys.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2sbspltwt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xzbmafow.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yjucqmsl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ydvwzokf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxpimesp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejofvmjq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2swpxfpft.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2axcreuro.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ozvxzeqg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2movdftyb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aroceofg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mpnwcmgm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2umqxbyzz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2jnaszluw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2wjwrrodp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2lofsqzkd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2krozphxk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ancevlbq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xlgaqrpj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nbutjlom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txhwekir.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2lwnelxxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdpupuyi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2umxrbegg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kudzykhc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aojlxewh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kxmgauec.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dpjfrcyl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fcgwflyr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2oxgpqccq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2himipalw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gbrowwnb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2aswdaywp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xvbutdjf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2yuexjsgm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vjuivxft.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nzvlpngy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2elbadebk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2deqyhsem.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2pysewajk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jqvfvyko.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hldkdiij.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2uysxtbkl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ectchmxo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eqxuxtgy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qmimyxom.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tezjtbkt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uoflxqkb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2lpmdlgyz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pkpruzzb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xvxlmgmn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rtuzozaz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljfxqvab.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbjnnfk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjeuiwnu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsnwcnsu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdmciwaq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2byvzvmyn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvohakvj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2naefmjrl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uszczllo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2oryivjub.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dwqtruva.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhafhaqh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkrtheoq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vordhsmx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mjxowhqt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaxuipjz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dzyyemmg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2sousupgz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eljaskvh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtjmcrxm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nalqjjin.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2lemdqdzv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wegdfipa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fnturjdl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtxgiwly.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dyrecbkf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2efdjaxrb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fphvvtjn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mjzrzaaa.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mcnemyzk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2khdwoxlb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mmdemnne.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtqpzckf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uncwsmwo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vsfukaet.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2auaxukgd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yeobjqyj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zzfhlcvv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aebhyxbe.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2anmqmxgq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqvinar.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jsjbwsto.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2esgeklsg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2phmkchya.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2nawzuywm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qgadzkio.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lgahrcrx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwabluvm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2valoagyp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fswmaxlo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2smtnhhuo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tizgqdrv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2qjxfwtsb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2obargtec.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lvxwvcin.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jmpaeaaw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tiqzlglf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnkyfazp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2knqtrsbt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2twdhhits.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wrcbpqid.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2arcvoqkp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2acwaeger.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oqclrogs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qpsouewu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2huailnyf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ibqdnonc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dekhlilg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hcfnexwh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wouklysm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wlydmoog.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ieewvgca.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2oomnmtbp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hibeqdoo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mivkurlv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lzdrympt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2mofhsyda.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2aslptpii.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2iwbpgsts.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jmzbhxpa.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ekidupae.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ymmgwmdx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gldruwdr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wsliyals.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ixgdndeh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2emfbxzun.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ptkawswd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2apbhbiny.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ntgqdwrv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2amkzbvzx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kxdmiuoo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckrlecqr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpbaxfrv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bnuwotde.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2clxhfbsj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fspxlefy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hkyebqys.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2skvmnsmy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ihsdlaml.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2higsseeh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cffntryw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qafgfgqw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zixmisra.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bffzhtgu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rfiprdvr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pvgphxqn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jihzgufv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wuxlsixd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjsqkwnp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xxklisgh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zsamcdms.html


<!-- 参考信息 -->