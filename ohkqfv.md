代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.xuetiantiany.cn/gtwlhibubr.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.sxryk.cn/gtdcfwrxws.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jinghuilouyu.cn/gtrmzimewb.html

[A17] 位运算
来源：http://hz.sufxvd.cn/gtbqgzusjx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.bjfxy.top/gtpcrrqnfu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yuanzhike.top/gtyitdfuij.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtzzwgggkw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtueyxsppw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtnanbwnsu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.iojbl.cn/gteqvbkshc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gtzwulpzzj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fengsongda.top/gtbaszvdcg.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jqgfzy.top/gtlwtelkub.html

Py:   ord("A"); chr(65)
来源：http://hz.xinyue.icu/gtyyfzunon.html

PHP:  ord("A"); chr(65)
来源：http://hz.mhx1999.top/gtpziwsolo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jqgfzy.top/gtxiqujofr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daxiang520.top/gthzchwpim.html

Java: (int) 'A'; (char) 65
来源：http://hz.gaohongyu789.top/gtvpwoofro.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.hywenlv.cn/gtqopdkskc.html

Ruby: "A".ord; 65.chr
来源：http://hz.ybcxt.top/gtggvwzskf.html

C#:   (int)'A'; (char)65
来源：http://hz.daxiang520.top/gtywakbnye.html

[A19] 交换两个变量
来源：http://hz.nwbrower.top/gtdiinhkcx.html

Py:   a, b = b, a
来源：http://hz.yangfankeji.com/gtyutqebpv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.ydjk.org.cn/gtwvgpedty.html

JS:   [a, b] = [b, a];
来源：http://hz.wangshuangyany.cn/gtyxrvfimw.html

TS:   [a, b] = [b, a];
来源：http://hz.zhengqikj.top/gtidolyosu.html

Java: int t = a; a = b; b = t;
来源：http://hz.xinyue.icu/gtnyqxsrgp.html

Go:   a, b = b, a
来源：http://hz.gzhubu.top/gtoihbxhmc.html

Ruby: a, b = b, a
来源：http://hz.yuanzhike.top/gtonysatcj.html

C#:   (a, b) = (b, a);
来源：http://hz.daxiang520.top/gtjzfblcny.html

[A20] 读取标准输入
来源：http://hz.birdmap.top/gtuddrnzou.html

Py:   name = input("请输入：")
来源：http://hz.mhx1999.top/gtogqbpnxn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.wangdashe.top/gtmluticqg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.havefunace.top/gtjzkdlktn.html

TS:   // Node.js：readline 模块
来源：http://hz.yanxiufei.cn/gtxxwmsegh.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.aibaodan.cn/gttomiqaxi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.cdnleiting.top/gtkqqumprt.html

Ruby: gets.chomp
来源：http://hz.gogol.net.cn/gtdyjnthos.html

C#:   Console.ReadLine();
来源：http://hz.zdqjudy.top/gtfdyzmwha.html

[A21] 保留指定小数位输出
来源：http://hz.ivvv.top/gtnpinlapt.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zhixingplan.top/gtrlpupjgq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.gzhubu.top/gtsulyqrnl.html

JS:   (3.14159).toFixed(2)
来源：http://hz.zhiwuduotai.top/gtupfzwupz.html

TS:   (3.14159).toFixed(2)
来源：http://hz.ydzc1.top/gtsgsjwapz.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yangfankeji.com/gtdeqognoq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.ybcxt.top/gtuxvbxsfx.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.sweek.top/gtkqxewbuc.html

C#:   3.14159.ToString("F2")
来源：http://hz.cheryme.top/gtmyyljjmj.html

[A22] 获取字符串长度
来源：http://hz.havefunace.top/gtsarslopw.html

Py:   len(s)
来源：http://hz.jinyuanbaomall.cn/gtfazubiwo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.sxryk.cn/gtuhruwouc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.hnxiangtu.top/gtjulwrlcq.html

TS:   s.length
来源：http://hz.hnxiangtu.top/gtgfzjtcnj.html

Java: s.length()
来源：http://hz.316326.xyz/gtchrwlkhp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zhongyouzk.top/gtrrvsefzw.html

Ruby: s.length
来源：http://hz.tianlin.xyz/gtnrbactnf.html

C#:   s.Length
来源：http://hz.sufxvd.cn/gtfmiazyag.html

[A23] 大小写转换
来源：http://hz.ydzc1.top/gtnrlvvrau.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.hnxiangtu.top/gtdcngasco.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.nanxinkj.top/gtvapdpcew.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuetiantiany.cn/gtitrkxoyw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhixingplan.top/gtqvgwkece.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shzxlz.cn/gtpsyfchlo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ybcxt.top/gtvkogpwjf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.tianlin.xyz/gtgxnzllwh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yanxiufei.cn/gthtelfkcx.html

[A24] 去除首尾空白
来源：http://hz.cashguo.top/gtnhdtguzv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shangyingyoupin.top/gtokqsqwmv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xuanzx.com/gthtpxahop.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ehwqpu.com/gtrzddnjky.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.smart0.xyz/gtifybtqco.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.gaohongyu789.top/gtehkbztps.html

Go:   strings.TrimSpace(s)
来源：http://hz.jinyuanbaomall.cn/gtniqelwxz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.0kj1m.cn/gtpjrzwztp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jiagoushi.top/gtggatrvpo.html

[A25] 字符串比较
来源：http://hz.hysaishi.cn/gtjgoacret.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ywan-chungtsiang.top/gtqwnifvhn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zhiwuduotai.top/gtlzjjypuo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenzaomai.com/gtvhfinyyd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xinyue.icu/gtkhqwbyce.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.nanxuanxn.top/gthbicavtc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.chenzaomai.com/gtzpiuylfd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xziqi.cn/gthwyojrfu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ppjwa.cn/gtbsgmdgsg.html

[A26] 类型转换总览
来源：http://hz.yj202588.top/gtsaytzayw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.guowangkeji.top/gtuoejhqhy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.haohaochexian.top/gttucuaoqe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.tianlin.xyz/gtghazbdaa.html

TS:   Number() String() Boolean() x as number
来源：http://hz.aibaodan.cn/gtjtjcclvt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hywenlv.cn/gtkcnmqwbc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.nwbrower.top/gthemngscz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhengqikj.top/gtouggnuko.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.gogol.net.cn/gtixoikkyz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtslhktbmo.html

B. 流程控制
来源：http://hz.ydzc1.top/gticrzlgow.html

================================================================================
来源：http://hz.gaohongyu789.top/gtydgzxdrl.html

[B01] 条件判断 if / else
来源：http://hz.ppjwa.cn/gttlcrckgy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.9152youxi.cn/gtftkpgafi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xingfuxueyuan.xyz/gtnxjevwhq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.feifeiyinyue.top/gttqjfagef.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xziqi.cn/gtigludchg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ydzc1.top/gtrzpwnbbt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.redwolf501.top/gtiqrndetv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.c1oappe.top/gtixzqmczh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtiuoqjzbk.html

[B02] 多分支 else if / elif
来源：http://hz.nanxinkj.top/gtmgsqntbg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hywenlv.cn/gtlbrrkkek.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.ppjwa.cn/gtlztnoipt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtnieszeuz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gthoykmnto.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sufxvd.cn/gtyomjmxqk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ywan-chungtsiang.top/gtyxjyhuks.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.meibo888.top/gtjpxhpdhv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shuidangran.top/gtvfpmyapi.html

[B03] switch / match / case
来源：http://hz.ehwqpu.com/gtuajnzjqv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.meibo888.top/gthvgthzdc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yangfankeji.com/gtrqkfvhhi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yvedp.cn/gtzkynoups.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.quarkkingdee.top/gtiurvmdmg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtahglhzsd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.sysykeji.top/gteeaoreuk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.sysykeji.top/gtsgfhmvoo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xziqi.cn/gtwwglurub.html

[B04] for 计数循环
来源：http://hz.gaohongyu789.top/gtmgucsbpe.html

Py:   for i in range(10): print(i)
来源：http://hz.jqgfzy.top/gtjwllrukn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shuidangran.top/gtpddfeaof.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ehwqpu.com/gtlrthabgh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yongpay.top/gtrywxxfez.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.9152youxi.cn/gtyvaeokqp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ydzc1.top/gtlyzztstm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shzxlz.cn/gtiidbbxda.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.chenjidiqi.icu/gtrerfmgby.html

[B05] 遍历数组 / 列表
来源：http://hz.52xcode.cn/gtdsoiesmd.html

Py:   for item in arr: print(item)
来源：http://hz.zhengqikj.top/gtvaqrrmsx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zycfv.cn/gtplsztnft.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.quarkkingdee.top/gthibpufmp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yongpay.top/gtaxdpqclb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gaohongyu789.top/gtavshevfq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinghuilouyu.cn/gtjdbhivph.html

Ruby: arr.each { |item| puts item }
来源：http://hz.xziqi.cn/gtfktsnold.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.nanxuanxn.top/gtcpknmzsm.html

[B06] 遍历字典 / 对象
来源：http://hz.jinqigufen.top/gtuzddahft.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hywenlv.cn/gtwmjgrvbu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.havefunace.top/gtmjrqtima.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.smart0.xyz/gtvwihkweq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.snrcjt.cn/gtxylxcdmn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zycfv.cn/gttxmjxbay.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.cdnleiting.top/gttmgzxzlf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hongshengwenyu.top/gtebuovadi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sysykeji.top/gtqzhpwmfr.html

[B07] while 循环
来源：http://hz.ydjk.org.cn/gthxdwsidr.html

Py:   while i < 10: i += 1
来源：http://hz.jqgfzy.top/gtgkadzcyt.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xuanzx.com/gtglxrxqdy.html

JS:   while (i < 10) { i++; }
来源：http://hz.ppjwa.cn/gtbbjzkvrk.html

TS:   while (i < 10) { i++; }
来源：http://hz.hongshengwenyu.top/gtlhavducu.html

Java: while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gthytzbxyv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jyoumei.cn/gtphwserrt.html

Ruby: while i < 10; i += 1; end
来源：http://hz.chenzaomai.com/gtisucqqkm.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenzaomai.com/gtwwgtcghb.html

[B08] do-while（至少执行一次）
来源：http://hz.cqqwz.cn/gtigjctpwu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.tian-w.cn/gtbogvzzjh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hnqzz.top/gtpkfftxop.html

JS:   do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtwljqmvzi.html

TS:   do { i++; } while (i < 10);
来源：http://hz.nanxuanxn.top/gtkctmnvlg.html

Java: do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtulroajmh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.chenlongwang.top/gtutvxytlq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.birdmap.top/gtqzptcnhc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ivvv.top/gttpgmjwlm.html

[B09] break 与 continue
来源：http://hz.yueranfly.top/gtycjyobue.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ydzc1.top/gtbulxdpnp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cucudq.cn/gttnfwkxbc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtgznqklul.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtlqyrqpfs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtpbvwruhm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhongyouzk.top/gtatqsizhc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.haohaochexian.top/gtlneqeplf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtzhpoapys.html

[B10] 遍历同时拿索引
来源：http://hz.tian-w.cn/gttiqdqyrh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.0kj1m.cn/gtfhjuiqjv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yuanzhike.top/gtgaiezdxw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yuanzhike.top/gtnafokjwy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sufxvd.cn/gtmawmpaln.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.gzhubu.top/gtgdsxituz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ehwqpu.com/gtzhvqzgsp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tian-w.cn/gtvywtlkkw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yonumen.top/gtwsddawnb.html

[B11] 生成数字序列 / 区间
来源：http://hz.shangyingyoupin.top/gtgnshtunj.html

Py:   list(range(0, 10, 2))
来源：http://hz.hammf.cn/gthrqwrpma.html

PHP:  range(0, 10, 2);
来源：http://hz.ppjwa.cn/gtaufqqknu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daria6918.cn/gtuesyetfx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtopoihhkx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hfpthk.cn/gtjfaryefp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigfzy.top/gtzyfhhpky.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zycfv.cn/gtvorvwxsz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ywan-chungtsiang.top/gtuxurcmno.html

[B12] 跳出多层循环
来源：http://hz.jinyuanbaomall.cn/gtdizapqee.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yanxiufei.cn/gtchgepwxe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.dianchejie.cn/gtypsiqvsn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtqsuogrra.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtluxgrbfp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtvcdkokvo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yongpay.top/gtqdpfurwn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shuidangran.top/gtgwqtbrhu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.daxiang520.top/gtseylxuhr.html

[B13] 判断是否为数字
来源：http://hz.jinghuilouyu.cn/gtsnionvdo.html

Py:   isinstance(x, (int, float))
来源：http://hz.wangdashe.top/gtwuxqkisd.html

PHP:  is_numeric($x)
来源：http://hz.shuidangran.top/gtxbqwsgwt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gotoacloud.top/gtcrpctjhn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtzvfdcbyd.html

Java: x instanceof Number
来源：http://hz.yangfankeji.com/gtnipncpuy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cashguo.top/gtzxtczcfs.html

Ruby: x.is_a?(Numeric)
来源：http://hz.vqdsnc.cn/gtqejpokqv.html

C#:   x is int or double or decimal
来源：http://hz.jiagoushi.top/gtkpadgyfz.html

[B14] 判断值是否在集合内
来源：http://hz.yuxming.cn/gtiwhybqlv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinqigfzy.top/gtcwsqrwda.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.feifeiyinyue.top/gtneuchvss.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtzjwixqsm.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guowangkeji.top/gtxosayusr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuanzhike.top/gtkfqoducj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.9152youxi.cn/gtjsbeengm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yonumen.top/gtvddygqbf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinqigfzy.top/gtmzyozkqh.html

[B15] 布尔运算与取反
来源：http://hz.ivvv.top/gtvhmymowo.html

Py:   a and b or not c
来源：http://hz.nanxuanxn.top/gtqomjgwty.html

PHP:  $a && $b || !$c
来源：http://hz.gotoacloud.top/gtrhhbajrx.html

JS:   a && b || !c
来源：http://hz.aizwys.cn/gtkeajneii.html

TS:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtqtzctwpc.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gthshborea.html

Go:   a && b || !c
来源：http://hz.ydzc1.top/gtvqmdboac.html

Ruby: a && b || !c
来源：http://hz.sxryk.cn/gtubrocxqk.html

C#:   a && b || !c
来源：http://hz.daxiang520.top/gtrqraldra.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.aizwys.cn/gtfykgublq.html

Py:   if not data: return
来源：http://hz.sysykeji.top/gtwvfghlrt.html

PHP:  if (!$data) { return; }
来源：http://hz.cdnleiting.top/gtmufkgzcj.html

JS:   if (!data) return;
来源：http://hz.bjfxy.top/gtzgjtllzk.html

TS:   if (!data) return;
来源：http://hz.vqdsnc.cn/gttbpbscim.html

Java: if (data == null) return;
来源：http://hz.316326.xyz/gtmjcehxlj.html

Go:   if data == nil { return }
来源：http://hz.chenzaomai.com/gtdtqsoili.html

Ruby: return if data.nil?
来源：http://hz.feifeiyinyue.top/gtlaxndrmj.html

C#:   if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtwchixoly.html

================================================================================
来源：http://hz.cdnleiting.top/gtuiprtjiq.html

C. 函数与作用域
来源：http://hz.daxiang520.top/gtoqbzdkdj.html

================================================================================
来源：http://hz.52xcode.cn/gtelmrkkxs.html

[C01] 定义函数
来源：http://hz.jyoumei.cn/gtyqnzaomh.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxuanxn.top/gtfognsero.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.52xcode.cn/gtszbesypw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zycfv.cn/gtntjxahik.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gtceyateco.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtqfwiwuvi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.quarkkingdee.top/gtgloavgaz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shzxlz.cn/gtgqlgyngb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtbzofnaep.html

[C02] 默认参数
来源：http://hz.yonumen.top/gtbgadxqso.html

Py:   def greet(name="World"): return name
来源：http://hz.cqqwz.cn/gtyllgceky.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yueranfly.top/gtfmuuhwun.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.havefunace.top/gtdbvjevka.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuxming.cn/gtwwxanvoh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yangfankeji.com/gtnoufjxti.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cheryme.top/gtujnqjyhw.html

Ruby: def greet(name = "World") = name
来源：http://hz.ehwqpu.com/gtuljnjwvt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nwbrower.top/gtpxgkvuft.html

[C03] 可变参数
来源：http://hz.yonumen.top/gtcfdvqcsd.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenlongwang.top/gtdptymsdj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.vqdsnc.cn/gtozzbglzm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gtiyqinpnh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtdedzghid.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yvedp.cn/gtuvqvurrh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.snrcjt.cn/gtodqupnrx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ywan-chungtsiang.top/gtaiaehbfx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xinyue.icu/gthjcucixa.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hnxiangtu.top/gtutkkzeqo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jqgfzy.top/gthxmvaxxg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinyuanbaomall.cn/gtdlidfoab.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtronqatyl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gogol.net.cn/gtwvcouxjr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ydjk.org.cn/gtnjskukrr.html

Go:   // 无：用配置结构体参数
来源：http://hz.cashguo.top/gtmpjyjzkg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sweek.top/gtwqbacmuo.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtarmhdeee.html

[C05] 返回多个值
来源：http://hz.redwolf501.top/gtdhvmtzsp.html

Py:   return a, b
来源：http://hz.xziqi.cn/gtyphwnnpw.html

PHP:  return [$a, $b];
来源：http://hz.zhaomingkeji.xyz/gtuwaxrlmb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pengpengdd.cyou/gtewtgjham.html

TS:   return { a, b };
来源：http://hz.vqdsnc.cn/gtabinxixu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ivvv.top/gtvqbqiyxg.html

Go:   return a, b
来源：http://hz.chenlongwang.top/gtdzbcxvhy.html

Ruby: return a, b
来源：http://hz.nanxinkj.top/gtfloynlie.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.aizwys.cn/gtcwjfvrfg.html

[C06] 匿名函数 / lambda
来源：http://hz.bjfxy.top/gtvgtrbgmc.html

Py:   square = lambda x: x * x
来源：http://hz.hywenlv.cn/gtjamshfqp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhaomingkeji.xyz/gtqsbjuspc.html

JS:   const square = x => x * x;
来源：http://hz.zdqjudy.top/gtqjcpomuc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gaohongyu789.top/gtuhfkoswc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xuetiantiany.cn/gtcfyrehqw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aizwys.cn/gtgtxbvpvo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.vqdsnc.cn/gtylkqbdcj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.snrcjt.cn/gtyseqgaso.html

[C07] 把函数作为参数传入
来源：http://hz.sysykeji.top/gtcvesqdpg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj20258888.top/gtioyfhztc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhoulong.xyz/gtehdojkck.html


<!-- 参考信息 -->