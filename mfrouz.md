代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3qlhbxdby.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xfksrmvx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vlaotcnv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3setwyney.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpblcua.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nbljxzgm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ddkvtcbg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3nllrwxvp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xamluryz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zskszxiq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3icxtaieu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cywjsusq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lyreqoem.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pgxipvuu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3msypejec.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gtxveefk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hltowlya.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3nqpnmsov.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eiftmiup.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ricczgxs.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bqeqgoev.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3lciazhvq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3idxfxvqd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3kajcfzuu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fenrvmdi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sqwvrfbd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cxuccvww.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qfpgxanb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gavusvwp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pgddzifo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3yjqdbanz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ptldnswn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vganyfcq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3aezmblop.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3sdarnucr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3cglawrbx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3kkfanval.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3egwctmmm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3sbbkagup.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3bwlrbtvx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3njzivdtj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3jfypnemo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rmzgocjl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3fnmicdog.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3udjcrmvm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vjmbwkuj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xhzkddeb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fsnbmlcp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3esorjidv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwaopydf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnasptpc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3heifwtzh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3zrfzeknp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzekbti.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ceekafxu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqvcefk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3daketrhu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3fbirbrzj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ikkpkcji.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ychyfsdh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3nnxkiejy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3vwrzzyli.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wvzpxcee.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3tbmmlpmr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nlikggbj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zizzklre.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3wdefawcq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rhylebyf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fxtpzsxo.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3jhnrrfsa.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3gfgawhek.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3mxetvnut.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3whjnyodp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jdbibfzl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ujxzahfs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3piadmfsw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pdeuwohl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3nebqsvmc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3pigarzux.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lnampysd.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3wymecsvm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zwmrnabi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vyjiwkpo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nltppxfp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3drlsukmz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rqvpzppu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pihcwgis.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3dmqvrand.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yxkylqcw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3xkrbnrdx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3enpkcjfm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3suhjslcu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3imhdhwqr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3uvpjptfc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3reptxleb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cmfglspf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hzffflvk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nkigjmyo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3uwswbjsd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3binrzrst.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uzbkwaia.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ynfzvlyp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uvsiyrqi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kvshwfdg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dbifprem.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zjsywwwf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zunuyrvb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nnrbitvi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3reetqnkr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fftipdyl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3foeebmmw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3lqdkrkom.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jufwhidd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ndghwcdh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3aliojwyz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nvepnszh.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3odbjzwba.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ohuuofpt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbzquatk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbchjwyd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3uibthose.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kwkrzsnr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3prdggera.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfzhkbmu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3iklqomgr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3zfvslgil.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3iwnsoojd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ruagggyi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3dnitknmo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cldpgyeu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xueqzlzn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hglvakwc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vcdhjfzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gimdsxgy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fdmixpvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfmkfclg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3fkgmkujo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qmjhocuv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3irkzavxg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vchopitb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zzmysecg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3belrqgai.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gqquscon.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gtubrptx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gfdtfkhz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wlswctmw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fsjpqsqh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3esdmxprx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xrixzczg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3toamnuui.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mfmxqgcd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jwozepcn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ydfbndhi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ilgzeuyk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3lqvlppsb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zjiqopwx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cqkjgmnv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqolmpuh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnyuvluz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekuxetyq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3afeustih.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qhpedgtz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yewetuxy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3oyqxadwb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wprdishh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3tklnhenz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcoipajx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fkhnutha.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjxnzkit.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bkbzmeof.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3yovnigqq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhticgbi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wdqcubpe.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qtjilsxb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3csbnjeau.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wpxxlywk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cslnpuxs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3sceykurn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3antpzyvm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3avubmzlw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dohijxvr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wnxzxitz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lecrozgl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gowjvqvw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ruxrmlbh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ndavsuyz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcgnjhjl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zjwfrjxj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mrvtapfg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ktmswcdj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3csdsufos.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bwbstbpr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzdwuzqu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bliqkdbi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltlgxncj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mumtlkmf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rifjsngu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fhzqviwa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebtjzeks.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ifvrqoyx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rakwftre.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rjywwbtf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rkyzbdlb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dsojlrxr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fbhxgmel.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kxsgvspc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vcuunrcw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jxvqkafg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3hpstrtzg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekervwje.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gzspyvqk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubgwnuoe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qmnqacnc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqlfsqph.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtfiqmf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3oqmpbunw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwflimgs.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3kmojfird.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vytefxsk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3shxluydg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qngywrxh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ngxmmdlp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyolqlqg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yihaeqsy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mbvojkux.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbemuivf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3gzovtwwr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cuefzlfi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lhddieaw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3oayhanfl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3utmqbpod.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ajbffhsj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3imugukdn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sszmtsxd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3niejjiji.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lmnhwpix.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3lnoeuzln.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3huqugcuc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3icxswfsc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3azdjourr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pohrjazu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ffxopabq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ksgawdbb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ddmxgxjp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3pbxaucfu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dbctsubf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zxulthbp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dakreooy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qrtpsnbe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wiynlmew.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3urmnfqbd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3bscuyoaz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xzdanqlk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vutesjhw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tngxxktr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qlvsbmru.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3okowvvvb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3keukfzbt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sepbtkvt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3fsuohdnj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uoghlikf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hngsfenc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wbthvarx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3uqqtlfjm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jvyogicw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jgdzzako.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3szxlwezm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mkjmjdzq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jqrxgmet.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dhpsrhtq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3stuxrach.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rapqivtq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wkglmlet.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyddzeir.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cwvaqnbz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dkumnjqm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gzqzszsm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjskoow.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3aveuuomv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aharlihp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqxrkacx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cnplusxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtkziboq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yxhyvtlh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ykxfbkol.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqsxuawz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pnjllphp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajimssrc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3asucjmpv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bgekfvrp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3spaluwqk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqudjowz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dqhrxzqq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wjlkvyjg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htahtmzt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hdscxokl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crkjokdc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qhlkucpp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mndclidv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3pnosuqly.html


<!-- 参考信息 -->