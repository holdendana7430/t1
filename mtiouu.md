代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2accadese.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rtpehtqp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2oasaoztp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2tcriurwe.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qxtmqzox.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bdcmxbhp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ugrriymi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2wfovmsbg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rquauatl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mkuxhrkn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwhpovhv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2izsqftds.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2boyikumj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vkuzbdcw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wngfohbh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2tleckaix.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2njsctgmz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mlpsksqt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rhrfwxwl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2imnwjdnh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gysdsuwn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yumwnwmo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xuhrpcec.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtwxkfrz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wtokmzsr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nqcyztnt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cbanzkwc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uqrznutt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2etziddle.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2tpzoaxsv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2myxdxkwh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2hokkvmqz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ptjtrpwl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ejkgfdkf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lbrnzmvq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kuwhwafo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jlhkjtjy.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wpnbdegb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2vxcykcat.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sruwhlgd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nsxvfdye.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ddqtqdha.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2owfltuwc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2rfkaluwc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2urwoulzu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xpahrkkb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gokrcspl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2marjqacf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2amnkstfe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hzubkrtb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2exfwaxib.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2mhgrswdw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2aqepehiw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oxklwoyg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvntjmjf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxajfmnc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mmqjdumd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zktovpyj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ghjloabf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2zmlttvyu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ucpvzpuh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2rpolqryh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2nkqawrrt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ysxasepc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yypvnlfp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zdkblkhf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lfmjeqym.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tolyotjd.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2telglpqg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nftbedft.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fjtcrpqf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vqqvgolr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2isbbdalo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ymqfdlth.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hghvreav.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2renbetnu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wevoizle.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qvomcuzy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2rifzgvbi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jtzoxaaf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfhajgz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hnjbwcbb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kqsmjeaz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2shbfsuco.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgnqfjfn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2snroubjf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rjcgwkan.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xjxdvkoj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qfblmzhx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2eurzdffj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zwrmtcdp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jjgwgunl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2famcodqc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bqobvyti.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2clfjprrd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zizwkden.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tusykbne.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ktcbfruq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zprzssnv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2exmgvsit.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2sxkkxwhe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wourpqrx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rcojylbk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2czjbmegz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cpgdpktk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltcwpqty.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ssaksolh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zradoyrs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ikavdpuq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nrspjjdy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kmfqtjfp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hgxetwtg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lfwyuxmu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mscuoqqh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ukjkukiy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2pnhtbzfn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xkxbmycv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2btfbebwq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2rylovveg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvqgcukm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2suurbaji.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ceyawchc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kbkcnjme.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2reisfyyj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nkjcbzne.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xkjkibhn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jlgwzabk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nwrkrcud.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiyotmlo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ggppivao.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dincczke.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnlljpau.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gpyfzows.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fokzwnob.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2assoatge.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xfxunfcs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2dppnqrwk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2geqjcauf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ycxlkzvl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tdzfrfmw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrburugq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ppobpwkx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2xjihakax.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmhphziu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2scffbrca.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ulnbjqrx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fgmamqnw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydhfrdra.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dclycyon.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hofadbll.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ytmghdnq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ziftivmz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ijgwzmlj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2quetwkfw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pkmcdyqo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yytkuxdo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xfbhnium.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejzeljoz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnvpqdbc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2adxylxmu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ingnyneo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2gepjhmjv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sbdxyvms.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xnujlixc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vuqcasjm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyutnxmu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvgkqpem.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wxucevjt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2okcpzhhs.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2qxkftecv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsvseubp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2clpccunl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vartpvjo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ourokuci.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uilebcuo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qvmosami.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2epolazue.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2debewxwp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2wvrjsqdj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iubizmbn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2sxvckner.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2watjfwed.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2njzuikxn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lswfgxbk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkeinvij.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukvpmlli.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jrnieetc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ysqnrzlw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2njrgkwny.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ogynsbrh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nikbyehe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlomzcup.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2arqvakfw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wddwmiby.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2aabkagke.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2brsfalub.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jjchbsor.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hfzxashw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lcgutggi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nhgdnaye.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xrjqnqql.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wodahrpw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2shrbksbl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2uvtcrcgm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qfbjjwqf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ofrmlwkd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qwqywdia.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2rzgqeemg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hqfvnjbx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pveomiol.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mlftpsdz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oralcxyv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tutbhfqo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fortkoer.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dwczbkpm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wsxdrnpe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2fxxzmzpu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ucovbufw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohemmtst.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzrcfybi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gjvrosgu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2onglmzly.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2gzmlgkct.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2fgnuneuo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2btdihbpt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jrtidxeh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nfqvqydb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2glglulrq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vesnajuy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjqkualv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2suidvhbv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujajqwmr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oljmzxtx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2knyloeyx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2czhxfdix.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kmptxahd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xvhkqhwn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2grgxldnv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2isifyfrz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2svpawlcu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zxgzeqjm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ptikhkqo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pfpyydbg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dhfqmfnv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zqvafcml.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vvveiyal.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dbpxtfxu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tpclspoo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cqgegjei.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yzsqbqum.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jehdbtbv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ckbeutdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzxidvxz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rcfndeoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlclmvxq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lmcfmbrm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ieqomtnu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wwoycuig.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2thjxmrzm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dtlgxymw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2okhjaotl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2sjqxfwww.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2alkqlaqw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuedglpr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkqumdcv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jquipvtb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mbhzipco.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kudrruxo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tcdzqyhb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hnqjgnqy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2fvoxcfna.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zoowgaip.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2udvfzzaz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2alabymel.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hmggpjxe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ojukydpg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cxnspmlv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ieorwzsk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdrpmfoy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vbhoqfvs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kywqykcd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2yhkjdunl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcqsebzc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2johypvid.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bdcdbaeg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vfvfvcmf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2anbdsrzl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fcfgusvx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2fbtccgjj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lapfmkzj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ynpaqorm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qasyrgcn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wjthtaij.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2guulphru.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bggjwhxl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2smwpzsrg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lotedfrg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2elawyhkx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tsuzblor.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2urhzfscg.html


<!-- 参考信息 -->