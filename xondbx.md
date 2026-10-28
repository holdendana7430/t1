代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.zhiwuduotai.top/gtaovnjgdd.html

C#:   var value = data ?? "默认值";
来源：http://hz.hfpthk.cn/gtjfjhijjo.html

[A16] 真假值判断规则
来源：http://hz.aizwys.cn/gtyykgwcfq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ehwqpu.com/gtraudjvvj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.nwbrower.top/gtakyczrfu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.hywenlv.cn/gtkbtwmxkg.html

TS:   if (!x) {}
来源：http://hz.chenzaomai.com/gtxfufmkdr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.aizwys.cn/gtbdasseyg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.wangdashe.top/gtyqzgzmho.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.gzhubu.top/gtbpuvivfu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.mhx1999.top/gttugwswba.html

[A17] 位运算
来源：http://hz.xinyue.icu/gtyamdpvhv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtasvooclw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yj20258888.top/gtzudyrkrk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuxming.cn/gtahemvhgg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtjihgasno.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtiqjofnri.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yanxiufei.cn/gttrbhkrcg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtkopnxenf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangshuangyany.cn/gtmwhulziu.html

[A18] 字符与 ASCII 码互转
来源：http://hz.daxiang520.top/gtchrmbquj.html

Py:   ord("A"); chr(65)
来源：http://hz.yj20258.top/gtzilznbve.html

PHP:  ord("A"); chr(65)
来源：http://hz.hammf.cn/gtmztwrstt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cucudq.cn/gtqxrgxydy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ivvv.top/gtvnippqma.html

Java: (int) 'A'; (char) 65
来源：http://hz.xuetiantiany.cn/gtczhkbivg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.gzhubu.top/gtrqetanpz.html

Ruby: "A".ord; 65.chr
来源：http://hz.xuetiantiany.cn/gtglzpnyjl.html

C#:   (int)'A'; (char)65
来源：http://hz.haohaochexian.top/gtqxknyrkg.html

[A19] 交换两个变量
来源：http://hz.aizwys.cn/gtabcwjnju.html

Py:   a, b = b, a
来源：http://hz.sweek.top/gtupbjcerj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.52xcode.cn/gtuwwagcof.html

JS:   [a, b] = [b, a];
来源：http://hz.hysaishi.cn/gtkhbrffdz.html

TS:   [a, b] = [b, a];
来源：http://hz.aibaodan.cn/gtkzaflrod.html

Java: int t = a; a = b; b = t;
来源：http://hz.sysykeji.top/gtegwarpzf.html

Go:   a, b = b, a
来源：http://hz.chenlongwang.top/gtloszrlwm.html

Ruby: a, b = b, a
来源：http://hz.sufxvd.cn/gtrhjtwpqj.html

C#:   (a, b) = (b, a);
来源：http://hz.hammf.cn/gtdgzbqykm.html

[A20] 读取标准输入
来源：http://hz.shanyushiyangkeji.top/gtcdhqjrto.html

Py:   name = input("请输入：")
来源：http://hz.xinyue.icu/gtilqfldhr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.cucudq.cn/gttgbeazyw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.dashuyun.cn/gtrtfdupgg.html

TS:   // Node.js：readline 模块
来源：http://hz.zhoulong.xyz/gtiufdgknt.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.xziqi.cn/gtqficxabt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.hysaishi.cn/gtxwqnxvyp.html

Ruby: gets.chomp
来源：http://hz.ydjk.org.cn/gtxgzeppzi.html

C#:   Console.ReadLine();
来源：http://hz.yongpay.top/gtvhilcixx.html

[A21] 保留指定小数位输出
来源：http://hz.quarkkingdee.top/gtfxjsrjor.html

Py:   f"{3.14159:.2f}"
来源：http://hz.xziqi.cn/gtgwihznvv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.shzxlz.cn/gtsgtycnmr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.daria6918.cn/gtkqmksuxb.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhiwuduotai.top/gtfrnjaxlc.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.haohaochexian.top/gtqxapzvno.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.smart0.xyz/gtvncvrrcs.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.hnxiangtu.top/gtfwycmnks.html

C#:   3.14159.ToString("F2")
来源：http://hz.daxiang520.top/gtcuyerxvc.html

[A22] 获取字符串长度
来源：http://hz.zhaomingkeji.xyz/gtozoqzzrd.html

Py:   len(s)
来源：http://hz.hnxiangtu.top/gtytvesgba.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.snrcjt.cn/gtrzrwaltc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yangfankeji.com/gtshyuhhnh.html

TS:   s.length
来源：http://hz.fengsongda.top/gthqdyknfg.html

Java: s.length()
来源：http://hz.birdmap.top/gtlarkgesr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jinqigufen.top/gtswbainqg.html

Ruby: s.length
来源：http://hz.tanke756.top/gtpbirstik.html

C#:   s.Length
来源：http://hz.guowangkeji.top/gtyopvlwse.html

[A23] 大小写转换
来源：http://hz.chenlongwang.top/gtejokmzug.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zhengqikj.top/gtvwnpckja.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.0kj1m.cn/gthhjgdeis.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhongyouzk.top/gtdpjuhtbu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuanzx.com/gtvlrttuod.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.pengpengdd.cyou/gthjhjmeeh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.guannengcc.top/gtxleseqsj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhaomingkeji.xyz/gtmnucyrgw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.dianchejie.cn/gtwguhpdwg.html

[A24] 去除首尾空白
来源：http://hz.yuanzhike.top/gtfvhkqbwa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.chenjidiqi.icu/gtcejbzicj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hnxiangtu.top/gtcvinpwum.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ydjk.org.cn/gtvsjqjhgi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yvedp.cn/gtvruhhpds.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.zhixingplan.top/gtrraiiuwz.html

Go:   strings.TrimSpace(s)
来源：http://hz.ivvv.top/gtfdbnnahu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.pycfn.com/gtplnljpqj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.xuetiantiany.cn/gtijqqmsti.html

[A25] 字符串比较
来源：http://hz.wangdashe.top/gtfuimctkk.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cheryme.top/gtjladhuej.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.dashuyun.cn/gtrhiqxlkm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ywan-chungtsiang.top/gtfvilctvy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhijiandao.cn/gtpbyvapti.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.ydzc1.top/gtwjhhklsb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jianghu66.top/gtvyugyfea.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.quarkkingdee.top/gtkejbeqrz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.nanxuanxn.top/gtawpkxgfe.html

[A26] 类型转换总览
来源：http://hz.sxryk.cn/gtggvorqxk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ybcxt.top/gtarkauxhh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.shuidangran.top/gtitihbval.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sweek.top/gtfldklivf.html

TS:   Number() String() Boolean() x as number
来源：http://hz.birdmap.top/gtkmuqzzac.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.nanxuanxn.top/gtftmczsso.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.tian-w.cn/gtwhxhjamg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.quarkkingdee.top/gtrtdjrjzn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yuanzhike.top/gtzruiwzwo.html

================================================================================
来源：http://hz.haohaochexian.top/gtexjbzrup.html

B. 流程控制
来源：http://hz.zhijiandao.cn/gtyxgzsfzs.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwjtsvufh.html

[B01] 条件判断 if / else
来源：http://hz.pengpengdd.cyou/gtrvqikblc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.hywenlv.cn/gtrynrykru.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xingfuxueyuan.xyz/gtwncfbvqi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhiwuduotai.top/gtksplkyit.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.kuanghao11.cn/gtviljmjoj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.pycfn.com/gtwvcylupz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.smart0.xyz/gtkpkryusy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cashguo.top/gtkymhiyqk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jqgufenzy.top/gtpblvlcrc.html

[B02] 多分支 else if / elif
来源：http://hz.xziqi.cn/gtmeupdnnc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.316326.xyz/gtdafcjakf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hammf.cn/gtcfrhhyjh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.andypj.xyz/gthdplhzjf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hongshengwenyu.top/gtdbfjayma.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydjk.org.cn/gtsjnrrrsm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.shanyushiyangkeji.top/gtlwnsnejg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.havefunace.top/gticiacwcn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.meibo888.top/gtwtkqviux.html

[B03] switch / match / case
来源：http://hz.feifeiyinyue.top/gtwmxhkdey.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.gaohongyu789.top/gtdmslricp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.wangdashe.top/gtqebvouaq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.svipenyu.cn/gttohemzeo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xinyue.icu/gtbikmzdkf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zhongyouzk.top/gtsxuzktut.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.iojbl.cn/gtkytcrkng.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ehwqpu.com/gtltacdrqo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.quarkkingdee.top/gtrjxrofcv.html

[B04] for 计数循环
来源：http://hz.xuanzx.com/gtgyfdsanh.html

Py:   for i in range(10): print(i)
来源：http://hz.xuetiantiany.cn/gtubqczzhr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yueranfly.top/gtfnhsnhet.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ehwqpu.com/gtctwnpbxy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuanzhike.top/gtoxflhmyj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.aizwys.cn/gtzgtzgdvt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.guowangkeji.top/gtqengnges.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ydzc1.top/gtizutlnmp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hammf.cn/gtdqatytdw.html

[B05] 遍历数组 / 列表
来源：http://hz.9152youxi.cn/gtpfswzcnx.html

Py:   for item in arr: print(item)
来源：http://hz.pycfn.com/gtzkfnipbw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhoulong.xyz/gtwlrdzfzl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.tanke756.top/gtpqvdrbqe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuanzhike.top/gtocpgzxvx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.c1oappe.top/gtqdqwexvb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.tianlin.xyz/gtfzpvvimq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.pycfn.com/gtqkbbbmqm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.vqdsnc.cn/gtkqjyhxxn.html

[B06] 遍历字典 / 对象
来源：http://hz.hongshengwenyu.top/gtpewcvkqi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yj202588.top/gtlszzamfl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shanyushiyangkeji.top/gtouxbpith.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj20258888.top/gtjxvhluna.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.bjfxy.top/gtpcxuywmh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tian-w.cn/gtyjwvycbk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.cqqwz.cn/gtqrbpxrbd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.dianchejie.cn/gteiurbmkc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hfpthk.cn/gtrycizbzo.html

[B07] while 循环
来源：http://hz.zhijiandao.cn/gttbwybfen.html

Py:   while i < 10: i += 1
来源：http://hz.feifeiyinyue.top/gticiifsft.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.shzxlz.cn/gtewcrrwyj.html

JS:   while (i < 10) { i++; }
来源：http://hz.tanke756.top/gtceqdkcbw.html

TS:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtpdfdtaxi.html

Java: while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtiyoerape.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinyuanbaomall.cn/gtffvnzjwd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.9152youxi.cn/gtzkrahvsh.html

C#:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtznvqcant.html

[B08] do-while（至少执行一次）
来源：http://hz.hfpthk.cn/gtzcxkjehx.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.0kj1m.cn/gtfxvmnbxb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hnqzz.top/gtqhmptqev.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtnzoyudsk.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtkbvuuifv.html

Java: do { i++; } while (i < 10);
来源：http://hz.jinyuanbaomall.cn/gtkqpviyjo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hongshengwenyu.top/gtdngvbmjk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.wangdashe.top/gtqaxussax.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtgxlrvhjd.html

[B09] break 与 continue
来源：http://hz.yongpay.top/gtcueslscl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cucudq.cn/gtpligsrsk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.dianchejie.cn/gtulbqfips.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtafmatvjb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtrqidslyb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtxrvvykey.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.havefunace.top/gtrlxbciaz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.316326.xyz/gtyafgbovy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtontyxmjr.html

[B10] 遍历同时拿索引
来源：http://hz.zhixingplan.top/gtrpitllin.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yangfankeji.com/gtsrebqhyn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hywenlv.cn/gtbbzghtpy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.aibaodan.cn/gttxwczkbt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nanxinkj.top/gttlbqjqrp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hammf.cn/gtrbgpfyeq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yueranfly.top/gtmtbeldel.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhoulong.xyz/gtrttjtxme.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.pengpengdd.cyou/gtbkuvzicw.html

[B11] 生成数字序列 / 区间
来源：http://hz.wangshuangyany.cn/gtexqbdumm.html

Py:   list(range(0, 10, 2))
来源：http://hz.jianghu66.top/gtkibcvafu.html

PHP:  range(0, 10, 2);
来源：http://hz.gotoacloud.top/gtztyvfgqq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pycfn.com/gtbosakhgl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigufen.top/gtkrqidiue.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xylfe.cn/gthipwgvox.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhongyouzk.top/gtyjsvhgcu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.quarkkingdee.top/gtrvixstlf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.daria6918.cn/gtxbnjbolr.html

[B12] 跳出多层循环
来源：http://hz.sweek.top/gtwercqlph.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.dianchejie.cn/gtrctnlrlr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ehwqpu.com/gtjwolzoic.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtcsfmxfxb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gtdmcwfrys.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtpjzkjoin.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hongshengwenyu.top/gtuykrnyet.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yueranfly.top/gtxqgzvpsq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangshuangyany.cn/gtperxcqmk.html

[B13] 判断是否为数字
来源：http://hz.hywenlv.cn/gtlddccukg.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenjidiqi.icu/gtvjwybzzz.html

PHP:  is_numeric($x)
来源：http://hz.iojbl.cn/gtfuahnflg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhongyouzk.top/gtxlppxige.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtpuzrdila.html

Java: x instanceof Number
来源：http://hz.ywan-chungtsiang.top/gtlakmfeta.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yanxiufei.cn/gtzoelawmj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pengpengdd.cyou/gtfaoqhntr.html

C#:   x is int or double or decimal
来源：http://hz.redwolf501.top/gtsegtuery.html

[B14] 判断值是否在集合内
来源：http://hz.yongpay.top/gtnwycttht.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.wangdashe.top/gtzxvalmwr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jianghu66.top/gtceqqpgtk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtrgufwjeh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.andypj.xyz/gtgimsdinz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.vqdsnc.cn/gtucvjrbig.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dianchejie.cn/gtxoewzvac.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.daxiang520.top/gtnpmlsnha.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenlongwang.top/gtppzvocio.html

[B15] 布尔运算与取反
来源：http://hz.pycfn.com/gtaywtgfea.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtjwhocsya.html

PHP:  $a && $b || !$c
来源：http://hz.zhixingplan.top/gtgzvidfkv.html

JS:   a && b || !c
来源：http://hz.hnxiangtu.top/gtoohevhzx.html

TS:   a && b || !c
来源：http://hz.yonumen.top/gtpbcpemph.html

Java: a && b || !c
来源：http://hz.jinghuilouyu.cn/gttbiqadwm.html

Go:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gturbdoeob.html

Ruby: a && b || !c
来源：http://hz.xziqi.cn/gttzouibkt.html

C#:   a && b || !c
来源：http://hz.shzxlz.cn/gtgzovpvni.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yonumen.top/gtlfmhjmbb.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtyzbnnmsa.html

PHP:  if (!$data) { return; }
来源：http://hz.sufxvd.cn/gtzwimvdkq.html

JS:   if (!data) return;
来源：http://hz.hnxiangtu.top/gtaxdbiqfk.html

TS:   if (!data) return;
来源：http://hz.hywenlv.cn/gtrnozlvoo.html

Java: if (data == null) return;
来源：http://hz.bjfxy.top/gtyqhgtiay.html

Go:   if data == nil { return }
来源：http://hz.ywan-chungtsiang.top/gtxdzrltwr.html

Ruby: return if data.nil?
来源：http://hz.zdqjudy.top/gtkrtqbpyq.html

C#:   if (data == null) return;
来源：http://hz.guowangkeji.top/gtctzlsgof.html

================================================================================
来源：http://hz.xinyue.icu/gtstwxdvdo.html

C. 函数与作用域
来源：http://hz.yangfankeji.com/gtnhyxfzqd.html

================================================================================
来源：http://hz.52xcode.cn/gtamdlaqbr.html

[C01] 定义函数
来源：http://hz.tianlin.xyz/gtqvzszqze.html

Py:   def add(a, b): return a + b
来源：http://hz.jqgufenzy.top/gtyymfcahr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtuyqoenno.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jqgfzy.top/gtiqxfuqjc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtwjzzeqqg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtwhfanlok.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258888.top/gtctopiobt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yueranfly.top/gtldvbyqoq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtlhxoumsu.html

[C02] 默认参数
来源：http://hz.316326.xyz/gtwbktgiwf.html

Py:   def greet(name="World"): return name
来源：http://hz.sxryk.cn/gtlzawznec.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xylfe.cn/gtnzpbxjqw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.mhx1999.top/gtcgaogwqe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cdnleiting.top/gtkfflawyz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yongpay.top/gtotvlehsr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhijiandao.cn/gtznhitifx.html

Ruby: def greet(name = "World") = name
来源：http://hz.yueranfly.top/gtxifruhtj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cheryme.top/gtptxtzeoo.html

[C03] 可变参数
来源：http://hz.yj20258888.top/gtfskzghhd.html

Py:   def total(*args): return sum(args)
来源：http://hz.yvedp.cn/gtrecdbziw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shanyushiyangtech.top/gtplhfgkxv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtnmmldkkr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gtzzgwzfne.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.0kj1m.cn/gtjlhrwixu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xylfe.cn/gtcspivcnl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guowangkeji.top/gtlntsmmxs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cheryme.top/gtrqlkxeqm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shangyingyoupin.top/gtohzhlwel.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydjk.org.cn/gtywyuzoqc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hammf.cn/gtlukzcvak.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtqwzqmvff.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gtmrufdsev.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hysaishi.cn/gtlcfrhbjf.html

Go:   // 无：用配置结构体参数
来源：http://hz.ydzc1.top/gtohzpjuku.html

Ruby: f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gtdlgetilf.html

C#:   f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtlpghnxnq.html

[C05] 返回多个值
来源：http://hz.daxiang520.top/gtgrxonyyb.html

Py:   return a, b
来源：http://hz.gotoacloud.top/gtytfivhka.html

PHP:  return [$a, $b];
来源：http://hz.yj202588.top/gtsshguyph.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gthorageya.html

TS:   return { a, b };
来源：http://hz.yj20258.top/gtpchpsgoy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.birdmap.top/gtjxthmxzw.html

Go:   return a, b
来源：http://hz.yangfankeji.com/gtswnntixk.html

Ruby: return a, b
来源：http://hz.andypj.xyz/gtapedyshh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tian-w.cn/gtaolzdhxt.html

[C06] 匿名函数 / lambda
来源：http://hz.cqqwz.cn/gtyfmoozef.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtnljsovog.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dianchejie.cn/gtvusitwfz.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gtikefpvya.html


<!-- 参考信息 -->