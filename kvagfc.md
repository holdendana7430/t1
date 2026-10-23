代发 wailian999

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xxmjeoma.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3keygcyyd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3igfgvyms.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wfxkaagf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jqxwqzly.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3hxlomgpz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wbravvwl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ydbjdkpb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3adaosqiv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3vgflqmyb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eicojqjd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tvwwjnzm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mozxqiqj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3twfbeuue.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wsaajqvo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hfocaucc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jvztozet.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zgkbxqfn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3edosmhbm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ppeofcdn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gjdnwmsx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lmhcdvxm.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ekzioojz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hiytmygr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3gezvbvjd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tvmdfnsu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mbkiohtj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmfittek.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qwsvjmpc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3lrswkbvj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgtujlqq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3fphtgyto.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwuidiic.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qmahszwr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dkbuyzlo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3afxatdkl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3edgzihus.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rtjqpeym.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3szhsbeeb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3krmlqezo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3eanrjbvt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cshdgthh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cbceaqqa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qskayssc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vjwqcxbx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3mimipsmg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xikqbklw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3oyztffkt.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3uvbryjja.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3kjbanrkn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3avofnnen.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3udwdlwyn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qyxeqzrs.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kvhzknve.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ehhfaobq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ipmdkvgn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ownwdcxl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3oxjkfwsv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rvuarwxf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3alkzxpwz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3dmfurhtz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3juklhwqq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3opsswzkx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3fnuztdzt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3uptqgxmh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3riekfmpx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3utufowjy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3gwsjgxnx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3zmaplzro.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ckybgzch.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dnndfotm.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zwoilwyg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3idedmbpa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rdvmnwrs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hpdedxvc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3qnfdqecb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bbqrjxrn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3zfowxyjr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3tbtxrhbx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jyjbazqs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vhenpxen.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pnswzfup.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zgyahsfb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ntvnplqb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ktdkwdve.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bjfcczou.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3mgewbifi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lctscnig.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lwbqnzin.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wnlnuxjg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xwvjiwgi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gehdsqbq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ixvenkay.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3iodojjnk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3uwzdkzra.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3gpwktfkd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cmosakbw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nguikyjw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3unmplzys.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hlhnvdhg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qffrgwhb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ttnaaopn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jfsaedkq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tisvfbjn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3yaqahgyv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vhhidkuy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bvhkofsy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktutfsrg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3akvekxvk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3cngvohmq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3mwrkgnjp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrvulsxx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3zdkohlba.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3cmsqjiif.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3amtuvpft.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3dxuxybic.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rwadxrsh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pblxasqv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qfcetpml.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3rrqfiysn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kvangngk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iffwokqe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3hwkjheoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxjaptst.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ofohonxw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hmvlpqab.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejovplsl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tgcegnvu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fbiezyqi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yexnmmlg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3sbswxzxh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3lixxjevz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vrzvxvei.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qdhlpkkk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3kwomrsep.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imkxmfzu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sxjolnsq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3soandkfj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yblfsuzg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wycrgkpt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3flmvtjje.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3turhyzef.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3snqzhlyq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ddowzsms.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyvmheoi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mggkidge.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sgxuegyu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjgitpu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nynejqbo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ccmlrwnm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kwetxrqd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hkbpcbjd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ikjexzta.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxjrnxfq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jfrokesw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uasucuvn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dzntsqmo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gjhjadnn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3npzjiwzn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3oejvufuw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3egicmbni.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ayobhtdl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3sguaohpk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmwqfnwi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iisvouoj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3uwnvyhjc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pioiqinj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ihzxmqyk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3skmtglcn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qqdfcdhi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ecmiohvy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3soonqhwe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcejmngj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ldfkofcn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3rvhribfq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qzvuemga.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3bjfklprn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3psrzpxow.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3exrkqncw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yrpboxzq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jdstzxpw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwrgwsns.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjacyyw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3axqwwdrg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wcxtjsas.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3nrkhhtww.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sspabrfa.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zpylibyy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3aqfyjrhi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3egwrtgea.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3locgyksv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lhyturvd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cwcdroqs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tvtohuhr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3pylcwnyd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ylfxmnbx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3rxpgeqck.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvuabcwj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdofvorg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xosnkbjl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cvuwjopi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mchtcsuf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qiaydrna.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3kecxpgpa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iuvyytgb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3epjwydup.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wbvtytlq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wcborhnv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uhikxtse.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eyojemxb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3uafpkfjg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yqbaxasv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ldfyxzxe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3woudegnu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zgfjiijh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fbrzgren.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fmfxyavj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mdnstjgu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3liuawbdi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mxsqvjnl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3bhfmxyaa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jwrbygbf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnwdsko.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ybznoqir.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xloonfgs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tgrnynqo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gufeoxmx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3osnemvrm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hsttlyfg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3suegazbi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3pqrikgoh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3abmltwsi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3heuqwskq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pcphgxqt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkywywzg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wabnujwt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijzbyaeh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3zsbvdnzr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yhyesxkc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vaxjmnqd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3uiomvcsz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3evjpjwjg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3sjorkqea.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sstuzguc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hyftzdkp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mteyyess.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zhibqivz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mwyeozpd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkgchqcd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jwmgkzwr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3flrzeqhr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ceojtfya.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mtiidcen.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uqnptjdu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gxjgogvd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uuoexdps.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mxvkohin.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qmnocpqv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sackejds.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qlowckua.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3nocrbgsa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3keisfosr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cxabsfdx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3isvyzyhz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pkhhjjxt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3slrqdfrp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pcnhlhty.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wrioipyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmrbflwt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hlclroui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuaapwbp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kppfwqmg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3myybpukb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbbtenhs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zzblbjvk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mqzhworx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ycmwawjy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vdhpcaez.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3obdeveeo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ejxjjgug.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sgjgdsad.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rybnqluc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmoknlhe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyaketwa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kewluxqr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jcmghdnv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vmkhczxm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ibggsjca.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gnagszpj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3yufyoabp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qfemdlyo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3uufazhbc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pgtsxjar.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3csjvxyuo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwrjscbu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3joyccyiy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hzrcillx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kxhatqex.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3twdimsfo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zgrzwmuo.html


<!-- 参考信息 -->