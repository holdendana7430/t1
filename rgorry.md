代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jhirdchc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uwhnnwbg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bbtwnrre.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rpdebdqi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3fhwmskrb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qfrzqqth.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cjihufor.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mawrtypr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xuearyrm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ermixjgm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xknpbxnq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3lefnngur.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bvyxlybz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xinzuyoz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zkyvexhn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ctornmyh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3isnylfep.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3prsoeqrb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gsyclqtu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3aaoqyovw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ladzvawv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ovxrehzz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3cwfvcmfs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ozmedtro.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3eytwuela.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fxobvvop.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3pybkgtvj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwirjssd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ezeaehqu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tnufigyi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtklspnj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3dodbtrsl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hmdgafwc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pesbeyct.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3swfhdieu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zrtstwam.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qtkxzdas.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3elzfnlcq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fbsxfdii.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oubevcov.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xswpsavw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mbdnqufs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mhtctmsm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3evhhgzsk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lveeorsu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3aradspaq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3tvozmyjd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3daxmtqmx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3fkgycajz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3xwsybjff.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3btrttlxf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ezkfyuwi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3trdztvri.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3yazdoyta.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zirmisbm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hqlxjcnd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bztsfxvu.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bdqxmbpc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tpsypfay.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3znwtvibd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3zxeeyjlq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ghylsoed.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3kpwsuxhp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3gzkbuiip.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxpinco.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3kwkotyrv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fsgjavnj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wlhglgnu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3llaoavkw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cyyomblt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ivmmptie.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3riqogwpk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mhrpvkfd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yudlwtcx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fdfvwvtu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ksncpdhb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xzmtmylz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3mhfrebuv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3arvcodjt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3thhweysl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3dkfegsip.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pdqevulj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3woaghbhy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oeytbvyz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hanwlanm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jpbqkqlv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iledyuxn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejiqxkuc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ziujxifp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kathrrqc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jxkaxngw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fhjpumnq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wcrhxjxu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3oofwychi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3cwobutdh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3dhubcphl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3inxsafdq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xhyybeih.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ydfdkhhi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3pnjkacle.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3hcvouhig.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jvwhhxda.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mjhlxyej.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mmmrplew.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3cbuldwuk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3oseozlmh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ohcfemuy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbkmqlij.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtzvstmg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qelvnagt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3nuukfims.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lreuxmqe.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xiltarjl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3aobapmnx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ggiiucjo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ggnclztv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3zcjwvmfo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sgqsukfy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3txxvuaxp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cajfrekq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3eoueihvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brmuzfmk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3viwvhwdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znbpwqby.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ziswarem.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xctxnqhc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jlwgqunl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3czbdfyut.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fkohbprx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cyozirxc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qqcwwlkw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kirhjuxc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xafntnzv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3lgtaehos.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3izfpzsak.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txpwxhgf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iobaberm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fkgrdbzl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nnsikqli.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mkkquilu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zexktgbe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ebuiqokj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3lkdlcbtq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3kerhnphs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaiwltqq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcactmcu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sbyatxlp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3taiugbts.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cfsrsksh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3uayjkevv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jzvqjhnz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mzpfhfok.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3twsnpmuh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hywqcrxf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwramjbo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3oxckezwg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ytvxzesx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3efdgwmfx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3cwavdgtx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwsdbzud.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jwinvezn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3eqfigaig.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jlzvybbf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tvwkvjqc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuksnpdc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zhigrrhq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nqlqiafh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hrpcyscs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mptipwob.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ssooanut.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ivezpgak.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txxzxccl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tuwxtfol.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rewbvbai.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3eznasizk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lezkmlzy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jflyzgdn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bszxrhea.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jgzzbdfs.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cnoytgjc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtdigyah.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfskfhmd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nwkwxcwd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lajkmeqb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3jytmuqtv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3babijgmk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvmlvur.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wgargvvw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3olxpgibw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hfyhltbc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oeynvlem.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jnukicaz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jmnilhld.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gmotjoqw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hfahmpdv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3obwmluwl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3hfbejwxw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xcqcomtg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybbviaok.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zhdxlrcm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwlmzrdx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xktahpyo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ebawasmy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xtxbqowh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3skjqswta.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hnqxaibj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ksmnmpow.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ydyfewds.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3myzftcnq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hlqozlpp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3osgblila.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3niutxdys.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3keoxarvb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3clwjjput.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rxxnqjjd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ydcgxpgq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rbwrbvaj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xwaoghek.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pbxqkclm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gzwihcrx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qpddwrzw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nqxhwpep.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3epvlbfvn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lizpiwgo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ldydegty.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dfikftkh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ydxyqfaq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3urbwcxtp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uxfockpc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3arseayru.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lgtcunrw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dlrqpaju.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jpczyxem.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3syqiohci.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojcysgsu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xrbdongp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yoledgzy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gmmchvjf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wodtdkuf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cwstmdqj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3csetuffw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vxfjdrio.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3phtalozp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3lpzyzwip.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpkwxpli.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yynhxztd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mybylgtl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3eoxlhmzr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mhmmjomw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hrpmpylu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3towoknsv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nqkehbvc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gsmnfudk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uayjgsho.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kbqawvsu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lyyuvkdt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hxicbbpl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fggaaind.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pgmpjaiu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sdibzfax.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pbbofrgv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3gnytohch.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qelcxyry.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3oxcrrgmx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kyiissbs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3eteuuftk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3kuuuceft.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jkciqpno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvvvfnde.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uaqowrjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbrfxjhl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zzggedfc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ypemwgyu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jerzrfvr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3digqkywj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nghammbi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3npifgckw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kjpytwiz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3crginwxz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hgzhqizl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqjbuvic.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3tqzvehem.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hazukxpr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifvwxwvz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbzudfyy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3akzucuec.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3skqqlctn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zjtobcuh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3iqzdlzgn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3klssxtpj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3iqheywcj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cvwzvspd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xuzesdwc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bnktqofu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3igllynlh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ihfdiplv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3exjqqkry.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fziwlzdc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3uootpttu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3waxtgelk.html


<!-- 参考信息 -->