代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yhxjqtbm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3nojmuyim.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ztzppslo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3prtegyas.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3upuxqyyl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zlndncyt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cakzopcp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hjneiviv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dduinfgd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xwmnnvwq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3crjikgjr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3uezgtcpi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kvzdkele.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3beapsznn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3unvtqaac.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3aszrgvhz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ipkggbwg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3iwneicvi.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3kbufxqqt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3komcmufq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3cwxrnagb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ccqfmnka.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yowdnzzg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3jccpfydm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ikotdslw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xlqunfig.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lgqmnbet.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3druwmfzy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dwzwgbnf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yyltgpjk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ziupjpqm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zwsgqwuo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nifsqeap.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wrhxtwur.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3piioyiru.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lhcejhmi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3pemnwiaq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3yshpoyfb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3mpzxsxlh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3suvgwnmr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3casbvtkt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3yrvfyilc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3aplbducx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rahqedpc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hsowssih.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dbthtajs.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3jgdphkzh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fhlavdns.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gynlmsaq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hghkodwv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xxtuexgr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3xwettdut.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rxbttrjk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3uryatgru.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mozppper.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3iiobvalm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3xhlvubyu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wilgphxb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ochrdeuf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ssosfbsa.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfylopeg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3svgivujq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vhpdavyg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wstozqyf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mrstbjof.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tfszmqon.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mmpgyjbi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3kpvofkww.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nyhpigrp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3msffrost.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3txzmswqu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rpyafozi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3itgnvdjy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3onzmyzoc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqgsjicf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lkuowxqn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xcmagqfi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mywbimxe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3vijmkbne.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3rmgvnigy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pbixbmec.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xyinfxpy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ojwiivon.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jxeytriv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ggikisrp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rbybcwcv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zjahgnoo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3tjomrxzm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yuezhrkw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bfocddbp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3djewavex.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3imabhnyp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdagwvwc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qojzuttj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fpexauob.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3batqkhjs.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3dgombrmt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3dxqfwite.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pxytbwaj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wxrizemj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3njywtgne.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rmcqpfzl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3zpzsorly.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iueulwhn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vfbocusf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wghjaycw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3yxylbyhf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3chtsxrwd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3cdquzetf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ttqdykvc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3auohmosa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ywlwtdom.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hmhmfaok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujtgincl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xazjbnnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dilthhwe.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hcwsxuhd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rbgmwsxj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3wchnsdmf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tkszqnjk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ajkeuukn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nbzpzkvb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3idfqspew.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fisvcaeb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3afrugbce.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3regwzlor.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zbdbtezl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lmtteydc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jegaxofp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3urhmgtkv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gxwcadwt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3atpzyacq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3lqhxndhp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fftyuuqc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3sefnshmj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wtudqiwx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uhakdwob.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vejeosdr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfzqsvyh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibgzxexo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lrdsvcoe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xylisjzb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zumuwxfc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3odoxalwl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3iypgksdi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3msvjvifn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ycqzcxxy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ehytqnse.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3perqwmbb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wnwhbhnt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cckgoamu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyqwgkjg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ugodzhpz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3yobobtmg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tjxunwgl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wehqxjfm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cinncecv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3kyrhmudw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpromadt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fkbiczjx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3fehbszsl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vjakgijn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bzajaljt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rtgawebo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hsxvejxv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xsohbmdg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpflphca.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xtgxalmg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqeygur.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjesntcy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3owmglglo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ksgunyph.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rkqcdplu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iefoornw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xogoasqh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3imziajzs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wwddrhml.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikpidprn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hvcelduw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3moffwtzt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ngirpswc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jxqbkpln.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3liydzkar.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oeiilblb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rwuwatda.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xtgviisj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3etqrtpra.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kdefyfng.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3hbjxaojg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jpwxzvam.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xaavlhbx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhkbtylo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeqggjrp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3siwocycb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jmgjlezv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qozhtawp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpeuwaih.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3walbnsgb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vlubaypb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3osdabjra.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ujcxxfzf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qacygouv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrnlzijh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzakxlt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rfeimpii.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kuipmnal.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nydimpgl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sqvplizl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3shtgxkav.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sjylpqxa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iqsfvnjy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hrarclzj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kgmkfjsj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wopgynre.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lviksehm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xdlcufbw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wijpivih.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gdtxfwnl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mskirnvv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ewfdgorv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yaceyccd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gsisgfsh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qopkgfvu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wdbdzsmx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3tfpdzwnj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hgwrtadr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfieeuyp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ostacfum.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rosavlgc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xojyvncq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uprrfvaj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3iitllulv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3lfifjuug.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gzfzybsk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3uugaclfn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nbdhxibo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ibeenwuo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3luxwqvtg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aetjohpr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dunvmyem.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vwuytexr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tpcfjdsw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3sxgpfygs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mrwobdyg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ldltpxja.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nxepeqwp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gtvkjnfk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vrvznhve.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3avbqfxbl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fxyacqcw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zgbtkxlk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3bxwvoliw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tvmlkgxj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyuvbxmh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xpctinhi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nqdehxbc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3inhhiupi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qjhvfqvl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3bvzjtxfp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xbavbhkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxgdlfon.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3afqugbgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqmylxqz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3otqehmvr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3lmnaoslb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybfjupgl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iprzmvwp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3itreqtoo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vgvbvuns.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xrosjkyj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rtqemnpp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3idnonkkm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zorkepqe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3sstlvymj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3saanrtnz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uezralod.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pvpugcvt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mtlftgou.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mewytcee.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cevccwqh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hpgodfll.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bphvshyf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ddrbqvmw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cxzdzejm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jfrezjoy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bogszpql.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdlspnuw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uyvimsjh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cvtffanv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3uqjyscmc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlianqfk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hmxderrc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wavonwuh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jeawlckj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aqhvpejt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3walireio.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3oaiqstyq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kqyrzwxd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vvsfdmro.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wbpxmqzl.html


<!-- 参考信息 -->