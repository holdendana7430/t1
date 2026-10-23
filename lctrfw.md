代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ldurncmf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvssktyv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qvuhotvf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3yeqygotq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3bcqtwiwa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3zsolrsvi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ybnyhdyr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qkgrxqqf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ewredsuw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wmxosuje.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aibnsdgq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ngtmykut.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jvhxkhvk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dktdzpez.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hfzzpvyh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3gawsergp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3juthqqnu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3mohvnxns.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zyuitnaq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ptvmnunt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3tpmspuvd.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wqqwcjhs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3alhfdldq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3wnbshaec.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3smcuiuxa.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zqzshcub.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jbahuvsr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qgyalgha.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cwsbvwos.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wstgtubq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kbiaznan.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tviwzuyx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3fccrqkql.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3yrvkygvx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rlsahipa.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3khtglzxp.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dkkoazjp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3cokndxln.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kofujizk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3rdjjfgpj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yrozmzxs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hlkcdgpm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rlsdtqwu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lkqmyyhk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tibjtnza.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yccpkorr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3bqebwvbb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3tykkvdod.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3lyvlcgtx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xkwqvxvs.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3aktqxbgt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ygsrotao.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3dxzcjgey.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ypuumudh.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xjawkgrb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwgaxrgu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nxflsogm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ercywaxv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qosakryh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qugqyxng.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qvwnsmhs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uxthlrcv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eogfyxkg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lkelovsx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wzfeykmw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtadyzrm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aymfurhm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvpkeqgs.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3omsbtdfy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fsbptkmt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxhnkud.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rnkfqzwl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rvmqtkua.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ofjulnfq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3vpmzxper.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3qgfwjlmy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3lfjnxmoz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cqtlsnhu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3whidfokx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pijlflpn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3trdqwlay.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3yzzmxkps.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3bfvldxhi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fxkyvkki.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3honmlhbx.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3xfteimqh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3qjmxylkl.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3mnicugja.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lwqzqmzl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3insnztws.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wufsiycb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zakwhgcr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3gxnmpahv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yqymccoj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3sfxroyfr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3gdxkubjj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3qxupzlof.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dnduptcl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zmnsuibn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3svwzmcqe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ytkcenta.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zpgymddv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3taczurkg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3sbqrecjj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iwhpuotq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3taiawqsc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ohfjgifk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jnliiniw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3wfeswmzt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uuurjzpx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djzsmlzf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3vgmeeylp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zivsahxg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3segzsxxo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xbqrnbme.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nudryees.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3iegcpdxs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cqzweirt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3brceksnw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3seghuarz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lpnkepko.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3uddrgqjp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3tghvlezt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3zlxewhhm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqbnvtw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rugowxdl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vpvnqamj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3eoosglra.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ipdengdy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3irwawbeh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wsuiwbcd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3estuulon.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jsdwsjdq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3iuqbbeve.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3htkjdmtb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wiriwruz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3puvlyvwy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssnncrgb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ddbkuewj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sorcxusf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3hiezoava.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3idxrtsmj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jwpdjkwk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3lakkmkrj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tjotremy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3timbugke.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3aavmkgds.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3znceyzta.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ncergfpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imrtuqtr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nyjalhtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpwpntri.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3uoledxln.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mbamjfiv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3eccnanev.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mrcrejqe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qprrmbky.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bbdjoagy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hslthqss.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dyksbupo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3enbuofjl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jqyokepi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zoeixrbq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cesqyhpr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3miufagto.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gnnlieud.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nbnokvgt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3pdrconvn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3igfwdtwv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uknszfkq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3klttfpgx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3maryrukw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qjfktxhm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mmivclnt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3crvarcnh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lbekxwwb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rbyvypua.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3njgqzyhb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gozwjfbj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xcijxtaa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bpbtffmn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ynsinmvs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uklfxcag.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ofcybtdq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwovakae.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nwuebkwn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zxfmvopk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3cehaqjsu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fhyqvgpo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hrfozvwe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbhnbfqd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ktvwowfa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rnwyfnhr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipzdjfif.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zoufgtlf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3kjlnxjbd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3lsoqaebh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ghihsgjr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3myqodalu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjcacjhm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tahznoya.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3sczwgvzm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ccowkqdh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gfwbivvq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yrxftqpd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hvzuxtew.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3obszodiw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmozqgvz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgrobepl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovjmidcf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3noezmivw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jedonecu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3jaijxodh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3nsuxxpnj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrqggsen.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3gzvgsudg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vdlqqmnj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mafmbmqm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3goooibnj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zpenxmyw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3civjnzuh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lgwqgowd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3afdwxygd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ynpicnej.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ehpgprgh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3evmkbeub.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wfsoqfaw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3swixkprw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcicvwgh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3isadwhzi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ymbjhwia.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tlfsdxth.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3enpmjypc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3guujynhy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jtwyjpfu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tditntlt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wtdkyjzk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vubseebu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbvmbyvk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bjsmkmhc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yysmxtvv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zkghwfpx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3sgosczyc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3vckillvh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3pdeymqkf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ylydwvpw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3riigouot.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ezmelhgb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kurxldae.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3viqzlljq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qjxxcfdr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rctjejzq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3trkfvwdu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wpsmrbsw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ryhxwcwh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ynesmkab.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uclocama.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bbjjmlns.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hyofvvgg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ogtmfnth.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wsyagpzu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fxumahcd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykhvmmjb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqbolbyn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3aqauntae.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3afdjaczc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3edilqbuc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jorwhhbm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3aytpowol.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3aexbkhwn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mwageblc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vhncybfu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwhfhrq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3blhgpmnc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajlntstm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3whsdqawk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qfooiakc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhylznck.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gfisvjek.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ozwvjjku.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3sclvipjs.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fyxtrbfc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dpmsirjh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cmldsrcg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dmaxmkzy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ybktbgaz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kgxtifyf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fvzzpfpd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yxozpmyt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kveuwizf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uwwmrczo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tlxtgoeg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3middaktc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3iprttpoq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zivyftid.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ltbumhlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcqwzzdv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mojkbrhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpukpree.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lfynlprp.html


<!-- 参考信息 -->