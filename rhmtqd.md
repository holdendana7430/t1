代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3euollhap.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3wicjdbqm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qenvsqab.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vpzhbxoz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3obmkamub.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gqfkiknc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ndtyyilh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3lhbzlpkv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tlldivql.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tmmocjii.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3sracwcxb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ljisjdhr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3dtsrjklr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fmwwutlz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3kujcpclt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urdjegdi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3psugsikg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3qpjgnubv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pqrjuhzt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vubhdclu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3btmjnvcl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qygvnaxv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wmksmgtj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cvqsqogf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3izdyzval.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3binxggbj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqycasvk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnxpyvmc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3jckhbodd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cubtwdnu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oojfhpmi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3patkhqsx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kpyxlxok.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3anqfjoup.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rjfkvluf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jmltuyda.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3uxthfota.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ieiyzqls.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fqpxiqgw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3wdrogxkf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3inmgudxt.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3iggronyr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3batwjfaz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fhblfzgl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rizswoiy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3urbatnta.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kxqoxpqu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3eybatptv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fufgmcsn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3gudxynxx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lzducews.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3hnwtktdl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3npmwsoqp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3xcyyfmqe.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3vswjwffm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3xahtwbfe.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qiribhrh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qnjgkqnp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ookwjeuf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjbktkc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ucsxztoy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3czussfrr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vtqeljin.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3mhvkrvat.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hlyjyznm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zitlsblt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vftziqfi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hjqqvpgk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ifuxohdl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mudpdniq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3coekyuci.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rhzdhaif.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3kolmgzkd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pipyzxcy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3buvhlloj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3dcxhnuta.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ldzwmsii.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xytdwepx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3johjmqem.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dzekmdam.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tmjkugkj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3umiasqbf.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3bprbvuoq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3nrjxxgip.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3inlzcdjk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pnjyqskg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pnjwonrv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3szhugzxa.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3pkgguamc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yzqhfmum.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fasufvwj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ujnlvsxa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jbvjyoty.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hgfscqsn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdjnvmdz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnfbkpmf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqjfouwr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wpytxxhj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xeornhdm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ommzepbm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qqfkvqex.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xaxxslty.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wlztslmd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3luajcisb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fzpdmsnp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tavajmif.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jnhydtrs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3crfnrzie.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vdxtuxkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3offxqvhb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lsrzzkqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxeagemu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zlxvxwfq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xzaemeju.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3penqnfpe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ipcauvuo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3onwccddt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bvuuyytk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kiwasvyo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mnihbaxs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qrynohfq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3nxeuvljn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hemvogix.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xybwvbjc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ggygqfjt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zgdegrzo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uihpzzky.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tslvsrfs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3edbktgfh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ldptlzht.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vqfduhzn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ehmepaqt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqrhkffy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ywtejyrt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kwyvpfiz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iabutqvy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3llrwxqoi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3erjuolgr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tomuewbd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hkqmvuwu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgugonc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3kdjafrnk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqdndkcj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pindwytj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sffqjqpg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wmnazqpl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lpdscpcd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jexyvqmu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3szzjmkxd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fwtlldtk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ocakxaal.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytrjxvzh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dejinusk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dbnthzge.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qvimpctw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3cpoytdvw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3muitdaxt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yvdwfstg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vdyixafd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3toajqnhr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrtxhwsj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjrivrzc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3bqcegosq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wnjkuled.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3uctebjyz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjjbkkys.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3inxbnehd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfswhaat.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wzhcrdya.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ygjffiob.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wbecwyoi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfezakhs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pkwaibdx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ldnrehsh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmctuoms.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3dvtssiwa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3azwgksqw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uqktgirj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tqvyqicj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qptyivwl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3prddukhs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hnasctle.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jpjjljna.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wxgjykrv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wunswqrc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cmupefma.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3giiushcu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3apdrzjby.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdlwzgpc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gvvplyux.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ulhbtpqz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ihmennxn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmvndgod.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rcjwpxwx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3cbcfzdvg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucpckrlx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bzlnocgb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xwnwivhe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xkjtgsxr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kljgwfnw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xuoiulzp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3sqlbyhjp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hdkxkjfk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ufefkmow.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xicbehdr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3loxclops.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3comxewbf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wfqhaqfk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lelbauei.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jwtszyex.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vygqmhec.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3oukzbskw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fqtinfml.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hejpyefb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sovgxbjn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sdxshlwa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qtdovvuz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ganhbcgw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3evzkckcl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lhaerxhn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zfnavijw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tqrtzqeu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3furxjcub.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmvbgoj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3makhmgcv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3iwknylke.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3hebvfesh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3squyncoe.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3pvsldytx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pbrwnbfa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xypgtnzk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3cqjcvtpa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ekxlrbie.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3owpvlyxg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zsbgaplo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ublrdlzd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vklxmaqd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xottvgai.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ozszqinq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3dbkvxonf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3knjlzecv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hehmydgq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3czqlrhes.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vrghxcls.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wyekqmtk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3apuslaoe.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lmdegdkj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wtjsngli.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cbbzpaqo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrogavfk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mnmalpmz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vqftujfu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ebxpgdrp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wpifsyfy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3iwgspnks.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mfmgdyan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3numcixnd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hmgennky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmzboduj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3aplmhslq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pspcfupj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmzkksno.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mjxehpzy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xzmfczvi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3awsuivxa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hsbysmaf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3iugkgkvd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdpxvkqa.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uovoprtw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lyverreh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bloneagc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooqiqjop.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlnakabo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3remfbuig.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3prxfwasi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tedhesud.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vyhdoifx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3phvgzych.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ihoklbcs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3plgcvfum.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdhptjsi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkzqrnhx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ygpxikvu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3nmhmnhlc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hoiopvrn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3pascbjmg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dcpzjzsa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wcshiinv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3yysokhpk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zyaqtafj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fmfyebvz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jcbsccqr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jzfqhwyv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljechrus.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3okjsdlfj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ijjlomzh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xsoqjgzn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ruxkidzm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nchuzagf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tdoxovgd.html


<!-- 参考信息 -->