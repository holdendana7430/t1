代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.birdmap.top/gtepzlwkze.html

TS:   const value = data ?? "默认值";
来源：http://hz.birdmap.top/gtuymdudrn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.316326.xyz/gtcyweihpq.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yj20258888.top/gtwddcewch.html

Ruby: value = data || "默认值"
来源：http://hz.quarkkingdee.top/gtczuumgmq.html

C#:   var value = data ?? "默认值";
来源：http://hz.cashguo.top/gtafpbhpgy.html

[A16] 真假值判断规则
来源：http://hz.hnxiangtu.top/gtuifezykr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ydzc1.top/gtjoznqakt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.sxryk.cn/gtynecymnj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.cheryme.top/gtuvwilndm.html

TS:   if (!x) {}
来源：http://hz.hysaishi.cn/gttsqnpbfh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.wangshuangyany.cn/gtjlesvywe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yj202588.top/gteoxnwory.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.aibaodan.cn/gtqdorcuga.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.zycfv.cn/gtvmqaclsr.html

[A17] 位运算
来源：http://hz.jqgufenzy.top/gtbrcxzwpp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtygszvzyp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jinyuanbaomall.cn/gtldfqbmrn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.meibo888.top/gtcwexlxvi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.ehwqpu.com/gtkcifsbkh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtflimdepu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.xinyue.icu/gtkaghgawk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.meibo888.top/gtgtadomgj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zycfv.cn/gtlgmjqrik.html

[A18] 字符与 ASCII 码互转
来源：http://hz.sweek.top/gtwelzkcno.html

Py:   ord("A"); chr(65)
来源：http://hz.yanxiufei.cn/gtltquvwlc.html

PHP:  ord("A"); chr(65)
来源：http://hz.tianlin.xyz/gtswjhjfmj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hongshengwenyu.top/gtfxtwrbzd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhijiandao.cn/gtplbmzytq.html

Java: (int) 'A'; (char) 65
来源：http://hz.hnqzz.top/gtipfemqwt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.daxiang520.top/gtuvpmcihn.html

Ruby: "A".ord; 65.chr
来源：http://hz.pengpengdd.cyou/gtjteqyztz.html

C#:   (int)'A'; (char)65
来源：http://hz.sxryk.cn/gtngxagumz.html

[A19] 交换两个变量
来源：http://hz.tianlin.xyz/gtqwgsrrsu.html

Py:   a, b = b, a
来源：http://hz.fengsongda.top/gtwgwtlrzh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jinghuilouyu.cn/gtepiiiwtj.html

JS:   [a, b] = [b, a];
来源：http://hz.havefunace.top/gteyffyptn.html

TS:   [a, b] = [b, a];
来源：http://hz.quarkkingdee.top/gtthyvnlst.html

Java: int t = a; a = b; b = t;
来源：http://hz.hongshengwenyu.top/gtrxlupbvu.html

Go:   a, b = b, a
来源：http://hz.ehwqpu.com/gtvzssylay.html

Ruby: a, b = b, a
来源：http://hz.9152youxi.cn/gtjneuvsmz.html

C#:   (a, b) = (b, a);
来源：http://hz.wangdashe.top/gtumjjgwpj.html

[A20] 读取标准输入
来源：http://hz.xziqi.cn/gtmhkamudx.html

Py:   name = input("请输入：")
来源：http://hz.sufxvd.cn/gtkardolwg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.iojbl.cn/gtyismmfrf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xuetiantiany.cn/gtxwimnzgn.html

TS:   // Node.js：readline 模块
来源：http://hz.ydzc1.top/gtnavplcdq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yj20258888.top/gtepzkzovj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.meibo888.top/gtdvbzwizo.html

Ruby: gets.chomp
来源：http://hz.shuidangran.top/gtotmdhonp.html

C#:   Console.ReadLine();
来源：http://hz.yj20258888.top/gtdytyeuqo.html

[A21] 保留指定小数位输出
来源：http://hz.chenzaomai.com/gthosmdddi.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jqgufenzy.top/gtxkiwqedf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtjvfekvdw.html

JS:   (3.14159).toFixed(2)
来源：http://hz.daria6918.cn/gtzbqwmmnf.html

TS:   (3.14159).toFixed(2)
来源：http://hz.birdmap.top/gtjqpcmzuw.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jyoumei.cn/gtlvssgqup.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jqgfzy.top/gtpodykejn.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.sxryk.cn/gtpermpnie.html

C#:   3.14159.ToString("F2")
来源：http://hz.hfpthk.cn/gtiisuhnqh.html

[A22] 获取字符串长度
来源：http://hz.quarkkingdee.top/gtqfyjbzfr.html

Py:   len(s)
来源：http://hz.xziqi.cn/gtbvgomzby.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xuetiantiany.cn/gtzriofevt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhaomingkeji.xyz/gtrrtjqfqq.html

TS:   s.length
来源：http://hz.smart0.xyz/gtqhdlorzk.html

Java: s.length()
来源：http://hz.quarkkingdee.top/gtashealpm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yongpay.top/gtxqlmttns.html

Ruby: s.length
来源：http://hz.jiagoushi.top/gthtilelwh.html

C#:   s.Length
来源：http://hz.feifeiyinyue.top/gtjaemlein.html

[A23] 大小写转换
来源：http://hz.zhongyouzk.top/gtzbuqecvo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.quarkkingdee.top/gtctzfkvss.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.daxiang520.top/gtdjkiyaky.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sysykeji.top/gtznntnbpl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.c1oappe.top/gttooxiyef.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zdqjudy.top/gtosbuwujm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ydjk.org.cn/gteozlxgov.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.quarkkingdee.top/gtmmfrshkl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.snrcjt.cn/gtwzkegvnx.html

[A24] 去除首尾空白
来源：http://hz.shanyushiyangkeji.top/gtsslwdyyu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yvedp.cn/gtfwcrfixg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.shanyushiyangkeji.top/gtivxzwtpq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sufxvd.cn/gtkpzvcrgl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yonumen.top/gttmeodesa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.0kj1m.cn/gtllpzkzxz.html

Go:   strings.TrimSpace(s)
来源：http://hz.cucudq.cn/gtpwdaxmtn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.snrcjt.cn/gtsytcxigh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yueranfly.top/gtpjemrnot.html

[A25] 字符串比较
来源：http://hz.yongpay.top/gtmcgtembm.html

Py:   s1 == s2; s1 != s2
来源：http://hz.vqdsnc.cn/gtfquiqxfm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jinqigfzy.top/gtqplwgnde.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.316326.xyz/gtdnlbrwkz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cqqwz.cn/gthixrlfwl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.snrcjt.cn/gtdvtvmjyi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ppjwa.cn/gtudaswbqz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yvedp.cn/gtuvodxyuo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xingfuxueyuan.xyz/gtzemctbqj.html

[A26] 类型转换总览
来源：http://hz.pycfn.com/gtjeehtizp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.cucudq.cn/gtsphoumfi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhiwuduotai.top/gtfkcgacwo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.dashuyun.cn/gtfargfttc.html

TS:   Number() String() Boolean() x as number
来源：http://hz.nwbrower.top/gtpohnegrq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.sufxvd.cn/gttvbnhmqv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.dashuyun.cn/gtrumtzdyy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.xuetiantiany.cn/gtfieghjku.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.daria6918.cn/gtfflybbcq.html

================================================================================
来源：http://hz.chenzaomai.com/gtwjwnpwwu.html

B. 流程控制
来源：http://hz.jlsjyb.cn/gtnkijevpu.html

================================================================================
来源：http://hz.guowangkeji.top/gtabepfmkm.html

[B01] 条件判断 if / else
来源：http://hz.zhengqikj.top/gtojwjsdon.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.kuanghao11.cn/gtipgmjyhc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.andypj.xyz/gtnwwgpbqv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nanxinkj.top/gtgtbnhnsd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.andypj.xyz/gthhscahgn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.quarkkingdee.top/gtcftsozqs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.dianchejie.cn/gthkmikttp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.chenlongwang.top/gtnthuwjrz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhixingplan.top/gtwetslviw.html

[B02] 多分支 else if / elif
来源：http://hz.cheryme.top/gthvboknce.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.chenlongwang.top/gtcmuvpwlj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.wangdashe.top/gtusslyccr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hnqzz.top/gtdcdpxzun.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtqdqerdlv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtwdrdgyak.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xziqi.cn/gtqhtzbajc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.fengsongda.top/gtmygypzvh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenzaomai.com/gtfducawsz.html

[B03] switch / match / case
来源：http://hz.guannengcc.top/gtucfzgfat.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jianghu66.top/gtsblkswws.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jqgfzy.top/gtoouodgdc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.feifeiyinyue.top/gtlvpgooyh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhijiandao.cn/gtmtgvwvgz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.fengsongda.top/gtvmkcvocg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhiwuduotai.top/gtkmcmjvgt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hysaishi.cn/gtdqtamaji.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.wangdashe.top/gtzsudwwyo.html

[B04] for 计数循环
来源：http://hz.yueranfly.top/gtpkwzgcwq.html

Py:   for i in range(10): print(i)
来源：http://hz.tanke756.top/gtksyuniwi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xingfuxueyuan.xyz/gtsdmfkpzk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sweek.top/gtdcrzsgiu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hysaishi.cn/gtixadzbhr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenjidiqi.icu/gtnaipabsj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xylfe.cn/gtnsdwxpat.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhaomingkeji.xyz/gtsrrdyqid.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.smart0.xyz/gtwshrmdzy.html

[B05] 遍历数组 / 列表
来源：http://hz.jqgfzy.top/gtseixejff.html

Py:   for item in arr: print(item)
来源：http://hz.cheryme.top/gtgvzkjlzf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ehwqpu.com/gtarckfmba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.gogol.net.cn/gteqichwoe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shuidangran.top/gtqzegfteo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.daxiang520.top/gttxusmvkc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.aizwys.cn/gtksuugofe.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ywan-chungtsiang.top/gttrqoabsq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.cucudq.cn/gtddtipwoq.html

[B06] 遍历字典 / 对象
来源：http://hz.gogol.net.cn/gtmtjjwqdo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuxming.cn/gtgljbhhjm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sysykeji.top/gtokqisdyr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinqigufen.top/gtynlnocri.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ppjwa.cn/gtzkfvjnxy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yj202588.top/gtnnybtimz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.gotoacloud.top/gtmxvgzwew.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xinyue.icu/gtdyjqizgk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.fzhhl.top/gtodsmttgc.html

[B07] while 循环
来源：http://hz.dianchejie.cn/gtxqkzntle.html

Py:   while i < 10: i += 1
来源：http://hz.yuanzhike.top/gtvcbsexwy.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jyoumei.cn/gtixfgemxk.html

JS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtnbnynysr.html

TS:   while (i < 10) { i++; }
来源：http://hz.guowangkeji.top/gtsympaext.html

Java: while (i < 10) { i++; }
来源：http://hz.cqqwz.cn/gttqvlkwwn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hnxiangtu.top/gtnrzixptz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jqgufenzy.top/gttrffrozv.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtdwuvbbpg.html

[B08] do-while（至少执行一次）
来源：http://hz.yonumen.top/gttxpyfilg.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jlsjyb.cn/gtcqafpago.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shanyushiyangtech.top/gtjwopnjqy.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtzjtytits.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gthvjismpa.html

Java: do { i++; } while (i < 10);
来源：http://hz.mhx1999.top/gtdvxewzno.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhongyouzk.top/gtkocnnngf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jlsjyb.cn/gtojtqzjpt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.pycfn.com/gtbogyprcm.html

[B09] break 与 continue
来源：http://hz.xuetiantiany.cn/gtctsgpnpi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinqigfzy.top/gtmhaomjuk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.chenjidiqi.icu/gtmbowfvfi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.svipenyu.cn/gttnstanzu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtxgznlugd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtqyybppgh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.tianlin.xyz/gtbcqrczvs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nanxinkj.top/gtezgdlqhy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtdbdbrsvd.html

[B10] 遍历同时拿索引
来源：http://hz.smart0.xyz/gtqbmfmsjg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.andypj.xyz/gtdgpfawwz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yj202588.top/gtuwrhdoqs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xziqi.cn/gtudjmwqqz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hnxiangtu.top/gtmpgoofbg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yongpay.top/gtdfssveih.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pengpengdd.cyou/gtgwwnpxsj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xylfe.cn/gtngdxmtrt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yanxiufei.cn/gtlwnmfuxt.html

[B11] 生成数字序列 / 区间
来源：http://hz.ehwqpu.com/gtyavmhssf.html

Py:   list(range(0, 10, 2))
来源：http://hz.sxryk.cn/gtsqgediwv.html

PHP:  range(0, 10, 2);
来源：http://hz.dianchejie.cn/gtjhbqksck.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shuidangran.top/gtkarzorxp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gthihxbmnm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtvwfsiogu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.316326.xyz/gtybnrsoiu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhongyouzk.top/gtzatgrrih.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hammf.cn/gtosrfuhcl.html

[B12] 跳出多层循环
来源：http://hz.cdnleiting.top/gtbrtbfmaa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.redwolf501.top/gtqpvxcptx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cdnleiting.top/gttviikwyu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtihlfqshc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtontcfjky.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.c1oappe.top/gtcjeayfft.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenzaomai.com/gtenqensqz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yonumen.top/gtmefouenr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cdnleiting.top/gtbuhkxndk.html

[B13] 判断是否为数字
来源：http://hz.xziqi.cn/gtcnlafnrw.html

Py:   isinstance(x, (int, float))
来源：http://hz.nwbrower.top/gtxlcaobqy.html

PHP:  is_numeric($x)
来源：http://hz.jyoumei.cn/gtrgmycwob.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangdashe.top/gtwokoxydl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtbvxzhnmf.html

Java: x instanceof Number
来源：http://hz.cqqwz.cn/gtsizrijbv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hongshengwenyu.top/gtqypryrtv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangdashe.top/gtcngynpdd.html

C#:   x is int or double or decimal
来源：http://hz.jyoumei.cn/gthimxtgeq.html

[B14] 判断值是否在集合内
来源：http://hz.shangyingyoupin.top/gtxzqvedys.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nwbrower.top/gtuxjdkvze.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yvedp.cn/gtubvtztmc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.aizwys.cn/gtbutdzbqp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.haohaochexian.top/gtpcsjpqmx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ydzc1.top/gtrrhvkduy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dashuyun.cn/gtmxzvpnzo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenjidiqi.icu/gtbdeiyovy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jlsjyb.cn/gtvqzpsowd.html

[B15] 布尔运算与取反
来源：http://hz.xylfe.cn/gtbugxanfn.html

Py:   a and b or not c
来源：http://hz.iojbl.cn/gtrtmjetyq.html

PHP:  $a && $b || !$c
来源：http://hz.yuanzhike.top/gtwbnbnske.html

JS:   a && b || !c
来源：http://hz.tianlin.xyz/gtnpuvkhsq.html

TS:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtbucvfyni.html

Java: a && b || !c
来源：http://hz.xuanzx.com/gttorreard.html

Go:   a && b || !c
来源：http://hz.xylfe.cn/gtxmfnsysj.html

Ruby: a && b || !c
来源：http://hz.52xcode.cn/gtrsfatljq.html

C#:   a && b || !c
来源：http://hz.redwolf501.top/gtelwdxost.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgufenzy.top/gtgcukrqys.html

Py:   if not data: return
来源：http://hz.svipenyu.cn/gtgvvcnkpk.html

PHP:  if (!$data) { return; }
来源：http://hz.meibo888.top/gtcinhvrwn.html

JS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtvmvwkdjx.html

TS:   if (!data) return;
来源：http://hz.wangdashe.top/gttgdrcqwm.html

Java: if (data == null) return;
来源：http://hz.52xcode.cn/gtkruvsxei.html

Go:   if data == nil { return }
来源：http://hz.aizwys.cn/gtbtavztxy.html

Ruby: return if data.nil?
来源：http://hz.cashguo.top/gtseedsvuw.html

C#:   if (data == null) return;
来源：http://hz.meibo888.top/gtdorboqlw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtyqknubql.html

C. 函数与作用域
来源：http://hz.vqdsnc.cn/gtfsigtyxt.html

================================================================================
来源：http://hz.mhx1999.top/gtnecnuwmg.html

[C01] 定义函数
来源：http://hz.shangyingyoupin.top/gtierldzmf.html

Py:   def add(a, b): return a + b
来源：http://hz.zdqjudy.top/gtdgcalyjq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gtfhogsatr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.birdmap.top/gtarfxgfwj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.haohaochexian.top/gtywjulfqm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhengqikj.top/gtgrcotbun.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.bjfxy.top/gtmnxdwcxq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yangfankeji.com/gtaourhghs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtankkbfeo.html

[C02] 默认参数
来源：http://hz.fzhhl.top/gtbdxxdluz.html

Py:   def greet(name="World"): return name
来源：http://hz.316326.xyz/gtqiepbaxq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gogol.net.cn/gttbkvnuzw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtkyxsxgri.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daxiang520.top/gtjltyxtie.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sufxvd.cn/gtojpoggpe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hysaishi.cn/gthnzmtewh.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhoulong.xyz/gtmqfpkbba.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shuidangran.top/gtxrrxkvej.html

[C03] 可变参数
来源：http://hz.snrcjt.cn/gtfgvtvhnb.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinqigufen.top/gtnowdfpfi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yuanzhike.top/gtodldyfxf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gtaqxmkega.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtszuvcwzw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.wangshuangyany.cn/gtmmqrsgvc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtvbjlyfun.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.fzhhl.top/gtuotkuadh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgfzy.top/gtehixlxrn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cqqwz.cn/gtcjfalmhu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nwbrower.top/gtifmgzvdo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhengqikj.top/gtwatktxom.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtrnbaitjr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinqigfzy.top/gtrvshyjib.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj202588.top/gthfcgmzcf.html

Go:   // 无：用配置结构体参数
来源：http://hz.iojbl.cn/gtoxtutvrj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtftrapkjk.html

C#:   f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtdpjlwoch.html

[C05] 返回多个值
来源：http://hz.zhoulong.xyz/gtflxjrqoy.html

Py:   return a, b
来源：http://hz.andypj.xyz/gtkiyrpnlf.html

PHP:  return [$a, $b];
来源：http://hz.nanxinkj.top/gtyidvpoxx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gtntayndca.html

TS:   return { a, b };
来源：http://hz.chenjidiqi.icu/gtipnitwzq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangtech.top/gtczdwkgyh.html

Go:   return a, b
来源：http://hz.sxryk.cn/gtiwrackwc.html

Ruby: return a, b
来源：http://hz.c1oappe.top/gtbwxzyxaz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tianlin.xyz/gtkpdegekz.html


<!-- 参考信息 -->