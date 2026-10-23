代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nmmjytxo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hmvfmedr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lhrcftlk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bkmuiocy.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uikogokw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rxkfwbno.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wuerdvbz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cjydvans.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3fsdntazt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bstikltq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pgozlmow.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3moxlpluw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gpvdsomy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3tsurddez.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rvuhqulh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3osqfysnt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3edoqyowz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sxgfozew.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wfrjbgdu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qdmpxmwv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tlfgsmlc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nexfpvad.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3utscthto.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3bnyyuwab.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3uszgamhz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fnctkkcu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3otycvubj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mhnzrfyq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3tsnjtxtl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fvpqhnot.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ssruozud.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3vjeflsit.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3qkjcwwpn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3tlsqddem.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugemecby.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ubfiuyqi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ufkjmckk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ihumwexa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3headdkwz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iogrwvoo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gbjhtgjj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwstsfbi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3emrqyfvr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zdkwrbeb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3bzunmxfp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ptymimbz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dqzoqiob.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3llvhfghz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hiuxdggx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3cnfvzdwg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zpmfmfdo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3sdxusfkp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3depymfbi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jjjkufyy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ycjdumtw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3flarncea.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lqsjktbj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3bojiclbm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3wmjlpcnw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dbqzijpl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zsfpqicl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3remefese.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3lhwqqlzq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3izatabeh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ygbsjowf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fbbbpcoo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uhmqklqp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3fqjuwacf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3onlhmaxe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qcdismfy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fhgeiddt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3vdfmylbk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3soofuoan.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xjikxbyc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uwjrncxj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hjcvxoac.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbvwlgx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zkazyrbu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jbfaerdn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xunwpzzj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bvsinohr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3untuqzvl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3tasnezbd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3xbuwwroy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hexolngc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hruholpt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdovnwmj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3psptbttv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cshnwmaz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ewyussok.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3salakxey.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoabxhhv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ssfjgeiw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nbmgrubi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cjixxwfi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cocyfrgl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3aoiswmfa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3jyccbvuk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3vhszsurt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3zengqalq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlzwnebe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3naxirwga.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cjbygxde.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3lojtylcr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kggzsaur.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cihuxuwl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dvdovlst.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iowtvohg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3hafnmnev.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zgljlchs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3grzyoeey.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtvicdh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3iddtacgm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3phdwsjjq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ktrtswnb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dbqbmvqn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3pmxradwh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jgmsqpdl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3etjmhgmy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zitcxokg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3owsiueyk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ffwzjjes.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xdupztdb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mtllyfar.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xxcgqskj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjzbprsf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3nhcphelf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xnsfjnkv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3jghtmntv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ptnkkpnx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxzbftiu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3osiqtgyv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cpuyykno.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yxtriuvz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qpztjzrb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jubfhrra.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rqlymdtc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zinzfrsx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xbbmpqzw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycyfnkca.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hfotbpeh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ojaqizvr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qiokygwz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3yyvqompw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3lfffqbfq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fggvjnzi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3oktbemsj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ibqiydrp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wwgtpjso.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3omryqefr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ahokzsdu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gvidzlio.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ydsnlbba.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3zfbzmytt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bqqxivof.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3iivhlmab.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3kikvilha.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ugvrfjwe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vlimulbz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cwepejei.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xdzvtwqn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kjvxguoc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qbczmaos.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3slwsosnz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bdvzyzeb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3artcrvlo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3obshohme.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nmxinlze.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fkjzjohx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3aeevswqw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xqhtugik.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ibpxtxvg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ktjeftnt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mmnloaeb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3hfsirtqy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bqhvabgu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvkhtskb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijwohjno.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3bmxjycco.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rxkaqgqd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kfniyrjm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipsdffws.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3usbexlfk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3uwxfivud.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rinazeia.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aatvhczr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zbdpfxqx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rmhqmjtg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rtbkgdnp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pwiyqyev.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkukzmco.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3iiykoxsp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zbdhswvj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gxgxwkud.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ldwxvjjg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cqrjltor.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3glqcqkvw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xbtsnkvq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gfszbrfl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zbwbbqno.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3oflhkhxm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fcfnenvn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzfqmvxl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkebuklh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vozioxad.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zowakwum.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mocoioxk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3apzhecku.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfinanuv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zefuhfxu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqjxcdg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hpglzcmc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ouduutom.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qrdlwylk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3yiqzxpwa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vcuzoqnu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ylqjfaky.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktvhttzc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mrudmbvq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3oravznxy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sswjtkxx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qzhmlxsj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xwbuapdq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bknkphjx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qzpbughl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nfgyypfr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nzejuwnm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3oncggzrs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wgohpuya.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wszrytaz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pyayqlws.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hpfifgzd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sltmfjbz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vqakcqak.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xlafxoyb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dldkucpw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3azetbsys.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3whslszhe.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ormtqgjv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fzytqixn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ehauezdy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ipsuwwgy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mdxzcgka.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3atirlcuz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ualrtygo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3auanhjac.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3rsueckta.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qrqweoaq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3havuxcsa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpprsaec.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vpeuxojq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjepggdb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hazubrwc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hexucsjv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jcqxscdg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wftbgyla.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gdlnsrzu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fmwikpxg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lguggqkj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ywzwzbaw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ghccigws.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cbqcgshv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vcyldjoq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xxtlkprj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mghipxfa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jzqaugjv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3elfgyemk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hfruvryd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mygozxml.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3socmlpnl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lehblvhq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3znfaywak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpkulywj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3oqkwptkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvvsrgsf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cpmjyszr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3telmlijn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pmphqvsk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxdeibwp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3boujqocm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwvbnnxy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yvulcplt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dczvzcys.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cqckmqnw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pdoxbhld.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bzlilkit.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rswzikbf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxwxuydz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufijosfj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3todujpib.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmjxspsg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kfpniaur.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3apipfbsr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bosgdnnk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fjpaajhx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mavaedlz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3epgbaput.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggyhuhqn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3plmomawy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ilrxycdn.html


<!-- 参考信息 -->