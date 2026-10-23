代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bflzsjks.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wvxclcjh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ybidcxah.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlvaagtb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbdnajr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3qbtnmath.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zcqijabw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mnoknxph.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bqrgbkjo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lutfaosu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3wnrbssgi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kqyypmji.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqzissnn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3knqrearm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fsdqdmgr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3vulvwbed.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ltguwgav.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3nsbwefxz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kcmukmku.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xcvkinsy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3entatofb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rjgcjgay.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3enjjxvnb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wjegzykf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gtwambqb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3abwbiojr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3miawluzh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ybejdmia.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3nekgqbvt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mfhdwbft.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jgnilqik.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xlkqueeh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ghnhiclq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tlgflcgt.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bcqifiph.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3amhknubz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ixjlppfq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3touubqmd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qgvzhbcm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iyscxlez.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3apcvhvhc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gujebvav.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pmpbmpbf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eilvojyq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hxnqczck.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ncdrtmut.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wveuwrov.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hlmduacw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qpseafed.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3teisrlku.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mtbhrpml.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3zfevsvsk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3siynftnr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3outzhzqp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jqeorbvp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rcrkqyws.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3emlzsoap.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uwinkffk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3whmvguou.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ijrhktxn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pkpenhlx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xrpxzvjo.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ardudbfp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3uidsfyga.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3newzstfw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3smvlabpi.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hqrfsset.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfpspmbq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3hkzvdywp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3avntvpnu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ncimfcaj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ersfhqdl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lxratstf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vdavwvxv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dfzrwibh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hpbzipbh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fzqrpxzq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3miqnuuxa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vsjndlok.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ksrllaho.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gwapydcg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3itregdul.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3loyxnhtx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3suxwclzx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cemelpzl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3gjxsjoga.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3cdzbfyjp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wbaimmbn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3apualsvi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mdmrqumc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3sikucgcg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3wfjkasbf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gzybmanx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dgagnmmi.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ehgvxzie.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cuytxanu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ypuvrqyv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ejdiexlj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hsfqqcfz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3lbwcdphp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hgzrlnhq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jynnzhhc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3voncofwk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vnsamcpo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3bjyiumwx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ukefzgit.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3wwihphvo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3vwcygcbn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3pmwmwztq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pkibcvyo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkmkwofr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3litelxrq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pvvocrrk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3irxqyqis.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3phoqtxny.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3uxmfymmp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wjunites.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3lgjrgieh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ujsxdwyt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3gsexfmkx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ojxtvlcr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3iggpyckw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvfvngrc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eyohdcob.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bsgjvthf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wquwsxdm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3swzmnkyj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vytuclyu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ldbrxlco.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ymbbiusg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jfhzqdtk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jqtaotqw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zofgahgm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qqrntchs.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3nsagyiaa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3oeljxlpv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3aljdquut.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rbwzxdsf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bkwcprvn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3slfeppgd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dufxvohw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3oxklnykd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3llijsrtn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eafhehnq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gckvnkfw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvdypwjk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vcqylrsp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hvfrpdnj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3slfmvphg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wijrdxec.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3gzkzadin.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzuyasdr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qwvkcssz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nwtznxdr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3spghnvnl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gpomaska.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3brwzoeyq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ymytlucg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rvhysnzx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ilfjzvnl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xvqtdbmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eddvqlds.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3olzuxpxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjdvbpgb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ydytvqja.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uqbxdeyb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fbyfiugf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dxippclm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ubuzqqlb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dskytjoe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3bnbcqcvx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3domojkhq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fehpznad.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3oeeenzkc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zemvflrq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzxzayao.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zqoaahym.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3drlcuuvx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pwiohygl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3olikbcsd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3pnvwpbjp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qjiynfcw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3epnjbigs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3odpvjmtp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioheqruq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krnixvhx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvtsdycj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqthcdzm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ulamgcft.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3udsjjipi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dbnbxvxz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cuwbsohr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qgevzywm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gfwgljcr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gangkjyf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzciiulh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccphudyc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3cakfvlbm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hqylraoz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3jggxztcn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sqmgcgrr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xbswtagc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ntgjifme.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3srkbxlem.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tffjhenh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rzudlyso.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3stxpyyqe.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3oeusnxnj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzekjgmj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lbqbswrt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3njarraed.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyubwrwe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmcykeyc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnkgddur.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tcgrxtfd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fzfwocoj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rmkigdkq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvcihrjj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dvhtzvze.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tugtkrob.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziurmdbb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbfcmfaq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lzpnqsdq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zrdmbdhg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3pdvzvwvp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3krkvsxtz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oimsgdks.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3egmflgxs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gdycvavl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zhmjeiyc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dohthner.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xgtsxmlc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mxnaihvd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnzjssvh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3twouhpqz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ijmtfsof.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3hizqvokx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3axeohkcr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cdcxxaja.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gphuuodq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gznqzxii.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddkaenly.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tcwyhsbp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvypurc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yahackmc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3nhtuzkkl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3flmfuabx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lvubylui.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jisossqr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hdpldhwk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xjahbjcm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tcrfvrpz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rhrcvzdw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3idilsjqo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qgmakzap.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3irpkgdeq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lcqlnwkv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rsxcidlk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dljnaiby.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xbitotek.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rhfjcbqq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rgjrbdmv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uydsjsze.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pbflynzo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3umfpkbwc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ptnzwxoj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ixcjrtlu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oaqpkgvt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3riqtacud.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vopjwbvr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zishlxuy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3alpcqsti.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cglhwpqp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3htdmyysi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3sctiqkic.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3atwmlgwy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iaixlxzs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ejduuwcr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ffwuofsa.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3uzunziys.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3tpoztnkz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wgvsdvls.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ggdftsap.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jeonwcnb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bsphixuy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqdadazo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jxnwesul.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3oojbtvzb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrwieoeb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rilnoxhd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mbmgktrd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rztbqynq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gvizmsjj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wtzpknny.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xpnfafvx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xlpwcplx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cxlftbda.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gvhdfrtw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cznyncsb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ykleqtgf.html


<!-- 参考信息 -->