代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3uknahezl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sigsfhfd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3blhoggwn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3zxbwnbqd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3dpxinzxd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3fbdbqisj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ubrmtdvi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pfrswrgd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yoqpkwke.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zsskiayj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kjagbgbs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3sbidyeht.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hlinukht.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ruydrhdm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eflbwnim.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3gtepufeh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3atekpexv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3eeulxylb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wcgdbocx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xjuieeoj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cngwbwgr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ioieffpe.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3rfpeiyix.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3mxcwfquk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vmtuyppv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bndqmqei.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hlusbnqt.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fewhvxhp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cmrgrldc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pmiqjjpm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mkytkttu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ettmmuym.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3pqydmpkj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3boyjkltp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nvzdzxka.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iollaeom.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aaawzico.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3hpscgqfj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3auvtihqf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3cleqcrhm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3foyyejef.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3nnpugzrg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sgpgduhr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sqiaemkt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qnmezdvj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eobfipjw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3autwpkwu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3logdhlqy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ijedwvla.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vuvchroq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3tzhxexvq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3czqxzdnn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3cerehans.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3wtfnrgas.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3elrbpooz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3gspjawnq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nohhcuzx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3sxgbwdpe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3orujucgs.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3amkpbcia.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ztgwpmtv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lyyesvne.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wrswwwzq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qycgcycl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iusjjzwo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jceekryr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cifaksak.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rwoqodzq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3humkciht.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zwiibbgm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wrstjkxs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hgltzhaa.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zgnrdktg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3kghdzbok.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uytneucc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3wprgewwu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cicxvcsf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jhgdegkq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kgymnfup.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xhssdyvg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3grgpnlda.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rtukuuab.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ebpilwom.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ohsuezne.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3edlurkah.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3pekcmznw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3oxxjgogp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ewzadsgi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ounrtmkx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zxbxrwhv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3jqspyjfi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3nnhhdbxc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3kkjgadcx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ejipjvbg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fupxeaju.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3peugydgx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ypytzdbn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cwpepahq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3blsqmscq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tilzupma.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tumbhhqs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tawrcvco.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jmhlixnl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3yjcioqrs.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qnafuhpk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmcatstr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3sgzpnsmh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3lvgixqia.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bttjjzmn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cpptjgbn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otlvnmcg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3egxicdoz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sethgtjw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iupaxytn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3yrpkdhof.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdydjat.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lykazpni.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zchzjkcq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3snrswlwd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsgxaias.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fbpdxdif.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3nwqjznbo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ryjrftfa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3lqtubkdl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lkgxzead.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mijcefte.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eoqxynqf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3bdpfmnrr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbevbusc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3woicvoun.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bfilkpum.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xqfmfmih.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3nmgjhpbw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgtzzcjx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3outogphs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3njcuwkfa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3oohfjmux.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftkefmtv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3leprnqol.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3osdxjbox.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3owskiegy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tinaboss.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3xcfpymko.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3zqdtwphi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ptkajmeu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ykneslty.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3raluceix.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ysbvdwfl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pijpfmrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmztlovn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zkinnlbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjxrjhob.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3unznigbg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ctmayygo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwxitjel.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ynhdyzkb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zfnbuatm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jgjehvit.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ytamxpkm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3atkwcggc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qusrxvnk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yzudwgel.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yhmyibge.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggustoxy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iozrztze.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wcccwzgq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gtbnjnrl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3aefwtvuy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ifyxaplr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lqakaune.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ueutgvyo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qhmprfyx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zewoieyi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hbpsmwfe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nkpesnpj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfmnolvl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3umfiegxl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3qdxjbmbo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vthccnre.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rxjqcvnq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eanapfcu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3orfifwit.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojkmuomj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrvnzssb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vfebckam.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vwcshyvb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qiubqwtw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3stzpimhz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3emhqkmis.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jzbdfuob.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qmauoqia.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vmwmesvv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwbqffhk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ogajczem.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fnbpoxlu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3rwdbsvkj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywpcpbhf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3veazrnqa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3pzloogtn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3prkjtuti.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hremkvxm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gvjhmdoo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhcumjts.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wrtysxoq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3seuxpouj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgyvmrpc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ytzgszot.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fgssochq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3evjvdgwg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wgdjlyzs.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mxlqqaky.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nioojebv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pcqgncyt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3qkasobbl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnzmumwo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3liikzmyj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3oshfejmx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dycczmxh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dgoigefp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lwmaeohi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gpioxreh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ifqoborp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hemztaob.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3skncuith.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lrrcahil.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3tpsmcvpp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uutplmlx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nbwwdhmv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkkpaucs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3snjmsgbg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3sdcxtenm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3brtsmzfs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zmhhvdew.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3nojskgus.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3onrrozjc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyeuchqz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aduhkbut.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bmpvdyky.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3expfqweh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qgvjkcqw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tqtpnpjj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3aifdwsau.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dtdmsbie.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3cmxjzepl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3flstrhyw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tlmzzkri.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3spiuemod.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvnusyfv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pnjpgvxj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lslgcavg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3joofhgkq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wgnnuops.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bchdygfq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hlpxwdeu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aavzfwal.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fuhhogft.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iuzvtjyj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3qpskymsr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3sqshgdit.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3szkjgpft.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kxqckkcg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pfbvmdiv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvsshhuk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcmbjqe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkicxqcp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lgbttfci.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bfgytnpz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3quzlakuo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tsprmgrf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xucjqyax.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3uvabbthn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3llhgcszc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fnpmfzfp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xifjjvmd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zzfvtpfu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwgndtfb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iishohlw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdoomuoi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qcsyhpjs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zpjorvxy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zmtnclgl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hnodaaab.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jwbyhjhn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xpbmpltt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xvtwgxzf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tpyxzncv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jiwoohrg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3czquctnq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ckbpjddq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwgneszp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ezgmkuqd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hcylqfpn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vubzmjaa.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3twmnhwqw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3omxubbgi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aubqlcxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljnvxefj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3owgkmweh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxypozix.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgwghfis.html


<!-- 参考信息 -->