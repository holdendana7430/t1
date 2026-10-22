代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zifblbsk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2harfssyx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xvwvyiwj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vezoyzrt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2duaaewbu.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mizovfin.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zrqkebys.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qbabxgyu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2iowgtbli.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zouegyqe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2uxhzgmtd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpevsbi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uoylviuz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2avoefzkw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2dfjzofgs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2imslrzhr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vxqvyqkv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qyaljbkv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcxunsoa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tngfusqw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2gwcqfect.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2bejgtnnh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odzdlqiq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qmmodzjj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2naugzlcg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ewufhonp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2camdbici.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qirptilh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xpybtame.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ivfuufep.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kxbeougc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pkxqayow.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2taygpphk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2steoojhf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ugolafih.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ttjqmrsu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rzxrlrns.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ueazmmbt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2fzoiffeh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ccpwpbnj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cgjubicv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ncyfvjpo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2abwfwpbf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2znlaisjx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ebohvyke.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pmgafvgx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dxibheks.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gemnntat.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fszcikoq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2mutqbeoe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2rouxwyzy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2drsrykth.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2bxohvruo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jmbfzsuy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2pzuepdfo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ppwsvocc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2vienuedf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2chncrrdb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2uuanttsc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zynedpye.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2tffscuqk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wxrwtsla.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2piugzmtf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ramzruxj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ompkwyce.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzpdamw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mromhpdt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qgqnhvyf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gauqgtlr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpaclpdj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2pohsiawg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ilxaezje.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2uvtnmvmt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2oxfnvakn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fergtjll.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2kntvfoze.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hcbnplsb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zzhwrjiv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jeleqxsw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzxalzc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ijazksrq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gazkosml.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ixekkngf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2tptfovfq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2twycfhdm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2mzcyqdpl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2exblfwme.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fucnplks.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkqwspkn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dzfnipll.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vzspjgyc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ockprpne.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qoczgpnh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rfdwssck.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rqrqbohk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2srkfxfcf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ofgaeutx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gacsczis.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bymmsmxx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqsugech.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qiiyjidl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsgpllyi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2flfacvxl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fsulbhdx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hcmhxfdo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2guwslsbn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2bhaotrjr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yhhdxdbb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2llhghxoc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yqudbzcm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bkluqszv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pqvqztfn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hqnuumle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyqahdze.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wpzgtdbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yecyfhni.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ytnhwhqr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2eefwbdgm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hctsprfq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nvazqljs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bnxyksrn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rhemmsht.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2kfkzjxtr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2plfqmtoj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2whgqkfwg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kdljzlix.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uuaaxllg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gthxrjeu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xhnvgfdv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wakepaog.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2stcinupv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vukzfggw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2pmeanbnr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xffrivtv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ttghooxv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2fjrnnkwn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrzmtzle.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zfhoceto.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qxnymmef.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2amnqjzrl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2etrgkuht.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2lwrsmnoo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2uauxjbdh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfmnyffr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2soajtwvn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zgyeuwhn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yohxdycx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgjddxtr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vapyaowy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2bvagnzua.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fvwppjnu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hweutyrn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2obvwtnvi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gxhfwywg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lxaegrqh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ldxmunqx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gjxdzxjz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2brfypopb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2yrkkfqox.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2maagoasz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2slikghtk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2qpiozinu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ivnpazgu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mjogtqlj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2alaewfgd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rbzgbtko.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jafxfxbp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2sgfwbikm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2cyvmrmgt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wsfwcooe.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2zavltoft.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cayuooeh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2guipaqal.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqbklwoy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqjcnuyq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksrscvlh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2myckmdbs.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvkluktx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uxidtaki.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rrigzzqy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ghhbfzux.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cnieoqus.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pukyzjmy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gjrtysoc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lwachzga.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lkyyujjw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2myaczfio.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mchogovb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bhmqnpba.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2njjjoxmq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vexjauml.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2blbcvvep.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjsklbmn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ylumgdew.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2glquguuu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dkqcvvyp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpllholu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2krgaxgps.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2sjckzkyd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuroermt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dprydbea.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gnzpkgxx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2nyhlmkwe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jbaijotd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yudfhpkq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2duyuwxrx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2twtxrfnt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ugepwged.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sswqvbpn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kcwbuyjq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nwrlsryf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oyeavget.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2sjowaxzb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qaiwzjei.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mmydpmbe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2txtpufdz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2miaamfed.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hgkfbune.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2muagarsz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zunqcglg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fvyebgzt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nbcfbyek.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ejxrnvdm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ozqurtid.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2yhtjxonu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zundsxna.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2oztzubsp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2irsvyjns.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vszblnvj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2riekywzu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xjigugok.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lrmoujck.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2chmceepv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xvrthhka.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2sauywhxa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2msgimzhz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxgmnnum.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2trjgpyjf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enqbqkzj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rprvahlq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uxioexcn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2erzmcftm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2lkdwbwfb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bqfrgusp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tfljweki.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dshfycpk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xgvskfpo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ndldbvgv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aizujajb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vzzmidmy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uhipdlza.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2irpsddxw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lfmbwbcp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwzhhqvd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ygwafmdh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gofabvvw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fztgzqno.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tbudxneu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qzgrmxjl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zkiuujbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbnefphd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lvcqjtxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smrfpvbh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dwcdnbvj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sealootf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oivgrbls.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uvensjrf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyxtrzmf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2monyhewv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ganfzhqk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jwrdpymp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vqpnxmtn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rnhmmxup.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vgqfvjfx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxdrqjkk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pjyqpzst.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rrrjipdl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tqwmcuba.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kssdjsko.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2oenyhwvr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qznpjoeh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kewuoekr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2azvetpss.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdcesizj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pmqizyeq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fzrqfkwp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2selvddax.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2lunqnfyj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tyknypyf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jcnsqldd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hczyisto.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nncbkcsr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2smyhkdsq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xewcajkh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fgtmfwyb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wpwhmwtq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bbysvadl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2idaauepl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvntakpo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hofyzuic.html


<!-- 参考信息 -->