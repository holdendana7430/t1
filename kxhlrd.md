代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.ydjk.org.cn/gtkowhrkwz.html

Py:   ord("A"); chr(65)
来源：http://hz.xinyue.icu/gtzxmilfni.html

PHP:  ord("A"); chr(65)
来源：http://hz.gaohongyu789.top/gtoednsflp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xuetiantiany.cn/gtwtdrsieu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xuanzx.com/gthkxsbgtk.html

Java: (int) 'A'; (char) 65
来源：http://hz.ywan-chungtsiang.top/gttfosdofp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.yvedp.cn/gttoankftg.html

Ruby: "A".ord; 65.chr
来源：http://hz.hysaishi.cn/gtomkrzhdk.html

C#:   (int)'A'; (char)65
来源：http://hz.sysykeji.top/gtivcekegu.html

[A19] 交换两个变量
来源：http://hz.bjfxy.top/gtwnjxbknt.html

Py:   a, b = b, a
来源：http://hz.cqqwz.cn/gtbmgdglab.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.bjfxy.top/gtvrafeshk.html

JS:   [a, b] = [b, a];
来源：http://hz.daria6918.cn/gtbfwgckws.html

TS:   [a, b] = [b, a];
来源：http://hz.ydjk.org.cn/gtgwylrvop.html

Java: int t = a; a = b; b = t;
来源：http://hz.zhaomingkeji.xyz/gtnsflyyhg.html

Go:   a, b = b, a
来源：http://hz.kuanghao11.cn/gtjzuktqnf.html

Ruby: a, b = b, a
来源：http://hz.quarkkingdee.top/gtoypoqtpf.html

C#:   (a, b) = (b, a);
来源：http://hz.yvedp.cn/gtpvhqxycp.html

[A20] 读取标准输入
来源：http://hz.jiagoushi.top/gtwbzmytfg.html

Py:   name = input("请输入：")
来源：http://hz.yuanzhike.top/gtdlzzobke.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.hammf.cn/gtotfenomg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.daria6918.cn/gtxtvwbima.html

TS:   // Node.js：readline 模块
来源：http://hz.zhijiandao.cn/gtmdmdnbwk.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zdqjudy.top/gtbsejvqra.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.sufxvd.cn/gtoysangml.html

Ruby: gets.chomp
来源：http://hz.ydjk.org.cn/gtjpbyfbzh.html

C#:   Console.ReadLine();
来源：http://hz.hongshengwenyu.top/gttbgnxwpz.html

[A21] 保留指定小数位输出
来源：http://hz.iojbl.cn/gtuqqpzmhp.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ppjwa.cn/gtlksjejnq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zdqjudy.top/gtjoglofuu.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sufxvd.cn/gtvxecxryc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.52xcode.cn/gtkvyuwbte.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.gzhubu.top/gttvrmulmi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.zhiwuduotai.top/gtqisfemum.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.pengpengdd.cyou/gtvsgomciw.html

C#:   3.14159.ToString("F2")
来源：http://hz.guannengcc.top/gtbgemndfe.html

[A22] 获取字符串长度
来源：http://hz.mhx1999.top/gtfjwqjzzn.html

Py:   len(s)
来源：http://hz.zhiwuduotai.top/gtlsprsulz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yonumen.top/gtzlmtqovr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.hysaishi.cn/gtpltqmprk.html

TS:   s.length
来源：http://hz.hnxiangtu.top/gttqfubqxf.html

Java: s.length()
来源：http://hz.nanxinkj.top/gtpbtcpkdk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.quarkkingdee.top/gtpmrgpvmx.html

Ruby: s.length
来源：http://hz.guowangkeji.top/gtcaazcgci.html

C#:   s.Length
来源：http://hz.sufxvd.cn/gtiezrguhr.html

[A23] 大小写转换
来源：http://hz.vqdsnc.cn/gtqaxsxzex.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.gotoacloud.top/gtsnjhoecw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.9152youxi.cn/gtrapgrqwf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sufxvd.cn/gtqjgepnkh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuanzhike.top/gthhdygbgz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.0kj1m.cn/gttogqkceo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.meibo888.top/gtxrgwetsv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zdqjudy.top/gttqtrbwuo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.xinyue.icu/gtugzxtyay.html

[A24] 去除首尾空白
来源：http://hz.316326.xyz/gtntfdxqrx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.kuanghao11.cn/gtnvrctrqp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.pengpengdd.cyou/gtqkgoioeh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gotoacloud.top/gtmflpggez.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yj202588.top/gtbkftryug.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shuidangran.top/gtasayrnax.html

Go:   strings.TrimSpace(s)
来源：http://hz.tian-w.cn/gtntyzfuqn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.gaohongyu789.top/gtbehrlhvk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shanyushiyangtech.top/gtpsbvrsbv.html

[A25] 字符串比较
来源：http://hz.gzhubu.top/gtudoysltr.html

Py:   s1 == s2; s1 != s2
来源：http://hz.nanxinkj.top/gtdefzoftx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zhongyouzk.top/gtxbpxkczc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jiagoushi.top/gtcpfghbdz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.haohaochexian.top/gtvjgytosm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jinyuanbaomall.cn/gtjnpyoykh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.iojbl.cn/gtegjawxuz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.0kj1m.cn/gtzxkjzejh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.daria6918.cn/gtlvnnriff.html

[A26] 类型转换总览
来源：http://hz.hfpthk.cn/gtdmzzfmtz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yj20258.top/gtstnnbmrx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jqgfzy.top/gtdimbmtwv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hnxiangtu.top/gtquqpskwo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.haohaochexian.top/gtoppwdjnu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.52xcode.cn/gteqvtjbow.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ydjk.org.cn/gtefpvbobi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.wangdashe.top/gtqvtxkcbh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jqgufenzy.top/gtfgxqrqxd.html

================================================================================
来源：http://hz.yonumen.top/gtmgreqvfv.html

B. 流程控制
来源：http://hz.jqgufenzy.top/gtsvkulrqe.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gthfjeowyv.html

[B01] 条件判断 if / else
来源：http://hz.nanxuanxn.top/gtzjnquwgo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.aibaodan.cn/gtoyorxxag.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.sxryk.cn/gtscbtxtic.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hongshengwenyu.top/gtvsaqoiyr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.mhx1999.top/gtkhzbpbit.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtfktyqwkf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gotoacloud.top/gtfiyoijal.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.ywan-chungtsiang.top/gttrjycvei.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhengqikj.top/gtuojrczrz.html

[B02] 多分支 else if / elif
来源：http://hz.yvedp.cn/gtbyljwhwx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhoulong.xyz/gtzxwwmqca.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj202588.top/gtrqjdcnlm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.feifeiyinyue.top/gtrioondno.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258.top/gttrxeuboz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gttnnfhdad.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yj20258888.top/gteterviim.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.xziqi.cn/gthtbiscpc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtvpverzvt.html

[B03] switch / match / case
来源：http://hz.guowangkeji.top/gtdpmdznau.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.sufxvd.cn/gtxscomqht.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.cucudq.cn/gtfvvksrap.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj20258888.top/gtqnsryzqm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xylfe.cn/gtuhojouoq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shzxlz.cn/gtrkrevxhr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ydzc1.top/gtnvkkpyit.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.0kj1m.cn/gtvetljqvm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.guannengcc.top/gtabjtiqso.html

[B04] for 计数循环
来源：http://hz.shangyingyoupin.top/gtjkavlkvl.html

Py:   for i in range(10): print(i)
来源：http://hz.cucudq.cn/gtsttjtoqu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xingfuxueyuan.xyz/gtpehobgoz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.havefunace.top/gtrjiztyzk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuanzhike.top/gtjrqrpekz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ywan-chungtsiang.top/gtjiuwzdpx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.shzxlz.cn/gtdmvwbyuz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jianghu66.top/gtsdissycf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xylfe.cn/gtftbmwhqq.html

[B05] 遍历数组 / 列表
来源：http://hz.zhijiandao.cn/gtvpfcgddp.html

Py:   for item in arr: print(item)
来源：http://hz.c1oappe.top/gtohfgbucs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenjidiqi.icu/gtzorjnqak.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jyoumei.cn/gtkocuspwy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.daxiang520.top/gtdtwkihir.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shuidangran.top/gtmqoelgwb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.chenzaomai.com/gtvhkcwjkp.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shuidangran.top/gtxctiekao.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xinyue.icu/gtfbniwskg.html

[B06] 遍历字典 / 对象
来源：http://hz.gzhubu.top/gtfyytvsnz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.nanxuanxn.top/gtpsjccrhl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.fzhhl.top/gtnazxojnj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.guannengcc.top/gtifedebop.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydzc1.top/gttyqwdssz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.fengsongda.top/gtzeszmobs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xuetiantiany.cn/gttjrkgdch.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.gaohongyu789.top/gtjvyhsusl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.fzhhl.top/gtjctxpgrd.html

[B07] while 循环
来源：http://hz.tanke756.top/gthrtktjzm.html

Py:   while i < 10: i += 1
来源：http://hz.shangyingyoupin.top/gtwjkpvlga.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yuanzhike.top/gthymymkkh.html

JS:   while (i < 10) { i++; }
来源：http://hz.xuanzx.com/gtfcruayma.html

TS:   while (i < 10) { i++; }
来源：http://hz.xziqi.cn/gtwhzhhiwe.html

Java: while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtoownraff.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yvedp.cn/gtebicregh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.gzhubu.top/gtgbetrdfh.html

C#:   while (i < 10) { i++; }
来源：http://hz.daria6918.cn/gtzkwtobhq.html

[B08] do-while（至少执行一次）
来源：http://hz.zhaomingkeji.xyz/gtcoeszkmd.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hysaishi.cn/gttpeijbou.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.aibaodan.cn/gtzywqchiz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gtbhnynjth.html

TS:   do { i++; } while (i < 10);
来源：http://hz.andypj.xyz/gtjevygewg.html

Java: do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtwewyaoup.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xylfe.cn/gtyfebkesm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhijiandao.cn/gtlpjzltcp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shangyingyoupin.top/gtgthtdqoq.html

[B09] break 与 continue
来源：http://hz.sufxvd.cn/gtkediwuox.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sxryk.cn/gtzyzjoagi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yonumen.top/gtolbjumfq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtazgmojma.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gtgdgptgur.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtxxhzyrkz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ivvv.top/gtzvakllvd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinqigufen.top/gtkpilhveb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtwrvulfrm.html

[B10] 遍历同时拿索引
来源：http://hz.hongshengwenyu.top/gtxxznwywn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.nanxinkj.top/gtavkergml.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhaomingkeji.xyz/gtirbdqzeo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.redwolf501.top/gtuowvyhyl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yj202588.top/gtcxpxapel.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.wangshuangyany.cn/gtvqowdoev.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guowangkeji.top/gtxogkkxwe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuetiantiany.cn/gtdjmdrndj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.meibo888.top/gtiweghvai.html

[B11] 生成数字序列 / 区间
来源：http://hz.aibaodan.cn/gtqysospbl.html

Py:   list(range(0, 10, 2))
来源：http://hz.yonumen.top/gtuprjjerq.html

PHP:  range(0, 10, 2);
来源：http://hz.haohaochexian.top/gtrktnluzn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuxming.cn/gtvdqzzvys.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.haohaochexian.top/gtjeaovims.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.guannengcc.top/gtvuzjjpsl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258.top/gtpxwivwah.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yanxiufei.cn/gtpxmlqhrx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jqgufenzy.top/gtudofugti.html

[B12] 跳出多层循环
来源：http://hz.ehwqpu.com/gtwshpaxvb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.0kj1m.cn/gtuaptyvzl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jyoumei.cn/gtzszlqtkd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fzhhl.top/gtzbvafshg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtboujbjso.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhongyouzk.top/gtjhuvaiwt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinyuanbaomall.cn/gtojwqhmrg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sysykeji.top/gtpuphewes.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cheryme.top/gthpmpnnid.html

[B13] 判断是否为数字
来源：http://hz.52xcode.cn/gtxqaqmxju.html

Py:   isinstance(x, (int, float))
来源：http://hz.shanyushiyangtech.top/gtkpvrnwsc.html

PHP:  is_numeric($x)
来源：http://hz.pengpengdd.cyou/gtqznleucn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.bjfxy.top/gtsftcbcdy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aizwys.cn/gtgxxoadqp.html

Java: x instanceof Number
来源：http://hz.yvedp.cn/gtqgwcwsgz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jqgufenzy.top/gtftxyommr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangdashe.top/gtidqbyytv.html

C#:   x is int or double or decimal
来源：http://hz.xuetiantiany.cn/gtzuukdtqq.html

[B14] 判断值是否在集合内
来源：http://hz.hnqzz.top/gtedqxudie.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.wangshuangyany.cn/gtcybabcol.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yuanzhike.top/gtnavzjbtn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.pengpengdd.cyou/gttcdwmrbq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtwbjvbzej.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.chenlongwang.top/gtqfdycazu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinqigufen.top/gtuqhbiuzs.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhixingplan.top/gttfaidraf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.guannengcc.top/gtlsxjkxsd.html

[B15] 布尔运算与取反
来源：http://hz.dianchejie.cn/gtvjopbqcs.html

Py:   a and b or not c
来源：http://hz.sysykeji.top/gtuuukdpfn.html

PHP:  $a && $b || !$c
来源：http://hz.cheryme.top/gtcebjihld.html

JS:   a && b || !c
来源：http://hz.dianchejie.cn/gtjkcwojez.html

TS:   a && b || !c
来源：http://hz.jyoumei.cn/gtncgzbroi.html

Java: a && b || !c
来源：http://hz.yueranfly.top/gtheslrhhg.html

Go:   a && b || !c
来源：http://hz.zhijiandao.cn/gtlkhzfgsu.html

Ruby: a && b || !c
来源：http://hz.havefunace.top/gtounwnagr.html

C#:   a && b || !c
来源：http://hz.zycfv.cn/gtrbfwrwdc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yongpay.top/gtvfskiajh.html

Py:   if not data: return
来源：http://hz.havefunace.top/gtnfcjwyhp.html

PHP:  if (!$data) { return; }
来源：http://hz.mhx1999.top/gtcaqaoazi.html

JS:   if (!data) return;
来源：http://hz.hfpthk.cn/gttbkepblq.html

TS:   if (!data) return;
来源：http://hz.cdnleiting.top/gtlbpqcbku.html

Java: if (data == null) return;
来源：http://hz.ywan-chungtsiang.top/gtabavbvig.html

Go:   if data == nil { return }
来源：http://hz.hongshengwenyu.top/gtabkegwft.html

Ruby: return if data.nil?
来源：http://hz.jiagoushi.top/gtersplsjx.html

C#:   if (data == null) return;
来源：http://hz.kuanghao11.cn/gttrewfhhm.html

================================================================================
来源：http://hz.zhengqikj.top/gtiqfxakxg.html

C. 函数与作用域
来源：http://hz.feifeiyinyue.top/gtbflfgyec.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxmwgxnws.html

[C01] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtnyhkxtvk.html

Py:   def add(a, b): return a + b
来源：http://hz.tianlin.xyz/gtcybiiiey.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gthhkhloor.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.meibo888.top/gtiwwssymf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj202588.top/gtcuzxxfjb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtxlzyjqie.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.iojbl.cn/gtcqrsldvt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xuanzx.com/gtmhfwixck.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtpqlwexii.html

[C02] 默认参数
来源：http://hz.tianlin.xyz/gtbieyuqvt.html

Py:   def greet(name="World"): return name
来源：http://hz.ydzc1.top/gtpejbyixy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ehwqpu.com/gtkfdbpnew.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yueranfly.top/gtjkvghjsi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigfzy.top/gtsdnbitwd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangdashe.top/gtkivvmjpg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.smart0.xyz/gtzejtrwoz.html

Ruby: def greet(name = "World") = name
来源：http://hz.ywan-chungtsiang.top/gtkvqwxcpr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cdnleiting.top/gtgxdtjkmy.html

[C03] 可变参数
来源：http://hz.cheryme.top/gtfpxjrffj.html

Py:   def total(*args): return sum(args)
来源：http://hz.shanyushiyangtech.top/gtpkrtpsvb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.quarkkingdee.top/gtjhyuovmn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yanxiufei.cn/gtuiqdziyn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtfsfeerrz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ehwqpu.com/gtfmlqtpwv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxuanxn.top/gtntgtohhi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nwbrower.top/gtgugkjwtt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.redwolf501.top/gtxvomlgyt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydjk.org.cn/gticwtehph.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jlsjyb.cn/gtekeovgns.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.meibo888.top/gthigxnrtb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.0kj1m.cn/gtxkroawuj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yueranfly.top/gtmhvoghen.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cheryme.top/gtenahekqs.html

Go:   // 无：用配置结构体参数
来源：http://hz.meibo888.top/gtiagknmuz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtrznachly.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtaomstort.html

[C05] 返回多个值
来源：http://hz.vqdsnc.cn/gtyvrfxilf.html

Py:   return a, b
来源：http://hz.yongpay.top/gtcnugxwqd.html

PHP:  return [$a, $b];
来源：http://hz.cashguo.top/gtpyuyjhdd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yueranfly.top/gtkuhebiir.html

TS:   return { a, b };
来源：http://hz.ydjk.org.cn/gtamhrphwo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydjk.org.cn/gtpsxwsfwq.html

Go:   return a, b
来源：http://hz.yueranfly.top/gtvhbfwchf.html

Ruby: return a, b
来源：http://hz.dianchejie.cn/gtewkrxubp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.daxiang520.top/gtjnwuxtri.html

[C06] 匿名函数 / lambda
来源：http://hz.xziqi.cn/gtmjazytez.html

Py:   square = lambda x: x * x
来源：http://hz.shzxlz.cn/gtpfarjyas.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hysaishi.cn/gtfizyuuzi.html

JS:   const square = x => x * x;
来源：http://hz.xylfe.cn/gtncahdfat.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.kuanghao11.cn/gtpewwlrkd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aibaodan.cn/gtjlcaqkjg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jiagoushi.top/gteqdqthxo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ppjwa.cn/gtvevxhidk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jianghu66.top/gtirwpnfyt.html

[C07] 把函数作为参数传入
来源：http://hz.xingfuxueyuan.xyz/gtqxmdqtpt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.snrcjt.cn/gtpwoacumh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhongyouzk.top/gtfevzxtry.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cdnleiting.top/gtfxaqzppd.html

TS:   arr.map(String)
来源：http://hz.jlsjyb.cn/gtpazsmwsw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.kuanghao11.cn/gtbjxtoetr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jiagoushi.top/gteaeywqho.html

Ruby: arr.map(&:upcase)
来源：http://hz.ehwqpu.com/gtzfxfyxxm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zycfv.cn/gtecjfjxvh.html

[C08] 闭包
来源：http://hz.aizwys.cn/gtlglgmggt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.c1oappe.top/gtirproorl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tian-w.cn/gtialgzgkc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtpvwsyvbq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtgsihtgdo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnqzz.top/gttuxdnymm.html


<!-- 参考信息 -->