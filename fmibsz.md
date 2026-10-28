代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.xingfuxueyuan.xyz/gtdqiwqlkw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.yanxiufei.cn/gttbhwmylx.html

TS:   if (!x) {}
来源：http://hz.ywan-chungtsiang.top/gtejkbeumm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.wangshuangyany.cn/gtchqohdzf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.hammf.cn/gttpgbwiox.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.fzhhl.top/gtzavgngbx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yuxming.cn/gtcgywqjab.html

[A17] 位运算
来源：http://hz.sufxvd.cn/gtqfpyhclx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtojrzatjc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.aizwys.cn/gtenpnhosp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhengqikj.top/gtfexrrsbe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.zhengqikj.top/gtzkitlxjp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gttebckrdr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.feifeiyinyue.top/gtlylwekjt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xylfe.cn/gtcvkaasqz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gtcdbvidfs.html

[A18] 字符与 ASCII 码互转
来源：http://hz.fzhhl.top/gtbaemsrbo.html

Py:   ord("A"); chr(65)
来源：http://hz.0kj1m.cn/gtjmlyylkr.html

PHP:  ord("A"); chr(65)
来源：http://hz.nanxuanxn.top/gthcsftzru.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sufxvd.cn/gtvddjczuq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.dianchejie.cn/gtkwstbswg.html

Java: (int) 'A'; (char) 65
来源：http://hz.yvedp.cn/gtlhrfkiyi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.aibaodan.cn/gtzltdhejy.html

Ruby: "A".ord; 65.chr
来源：http://hz.smart0.xyz/gtxlocjojq.html

C#:   (int)'A'; (char)65
来源：http://hz.svipenyu.cn/gtgxtistza.html

[A19] 交换两个变量
来源：http://hz.hongshengwenyu.top/gtdhhpkclb.html

Py:   a, b = b, a
来源：http://hz.chenzaomai.com/gtystdvlmu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.daxiang520.top/gtdctgdasl.html

JS:   [a, b] = [b, a];
来源：http://hz.zhongyouzk.top/gttzpjdolz.html

TS:   [a, b] = [b, a];
来源：http://hz.nanxuanxn.top/gtwdecvntr.html

Java: int t = a; a = b; b = t;
来源：http://hz.nanxuanxn.top/gtojznkeml.html

Go:   a, b = b, a
来源：http://hz.bjfxy.top/gtkijvicyh.html

Ruby: a, b = b, a
来源：http://hz.yj20258888.top/gtfsyjwvur.html

C#:   (a, b) = (b, a);
来源：http://hz.nanxuanxn.top/gtdohirulr.html

[A20] 读取标准输入
来源：http://hz.iojbl.cn/gtyfxxxppz.html

Py:   name = input("请输入：")
来源：http://hz.c1oappe.top/gtxqyehwal.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.vqdsnc.cn/gtzkyuenel.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.quarkkingdee.top/gtlrtwjxgj.html

TS:   // Node.js：readline 模块
来源：http://hz.aizwys.cn/gtobirdfqj.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.cqqwz.cn/gtwldpakzc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.nanxinkj.top/gteviajyoy.html

Ruby: gets.chomp
来源：http://hz.cheryme.top/gtckjgtqzn.html

C#:   Console.ReadLine();
来源：http://hz.jiagoushi.top/gtvlikrwfb.html

[A21] 保留指定小数位输出
来源：http://hz.jinyuanbaomall.cn/gtadfkertb.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yangfankeji.com/gticzjivwa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.shzxlz.cn/gttuzcrndt.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sufxvd.cn/gtfdfjvxgo.html

TS:   (3.14159).toFixed(2)
来源：http://hz.vqdsnc.cn/gtybhjvldv.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtgdcywotw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.smart0.xyz/gtegyllaki.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gtablvgnhe.html

C#:   3.14159.ToString("F2")
来源：http://hz.guannengcc.top/gtixdpvtxz.html

[A22] 获取字符串长度
来源：http://hz.shzxlz.cn/gtoxhdsnof.html

Py:   len(s)
来源：http://hz.hfpthk.cn/gtbjputlay.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.quarkkingdee.top/gtuavgania.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.hywenlv.cn/gtyuonbobb.html

TS:   s.length
来源：http://hz.316326.xyz/gtzyvcuenl.html

Java: s.length()
来源：http://hz.shzxlz.cn/gttujhriwk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yuanzhike.top/gttbujzuhu.html

Ruby: s.length
来源：http://hz.sweek.top/gtgipfybqy.html

C#:   s.Length
来源：http://hz.zhengqikj.top/gttxjzvhst.html

[A23] 大小写转换
来源：http://hz.hfpthk.cn/gtdowwezei.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yj20258888.top/gtxgfdawgr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yueranfly.top/gtttbuguzc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shuidangran.top/gtdltdnzgd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hammf.cn/gtebsgixhj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yanxiufei.cn/gtakrtngbh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinqigfzy.top/gtxzcdbtdb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yongpay.top/gtryoeyhnh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.316326.xyz/gtjkgffhnm.html

[A24] 去除首尾空白
来源：http://hz.fengsongda.top/gtsoobsovb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yangfankeji.com/gtlyzetdan.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.chenlongwang.top/gtsjyazqan.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tianlin.xyz/gtftwxfqwb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gotoacloud.top/gtewlicxyk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.sysykeji.top/gtrysicbug.html

Go:   strings.TrimSpace(s)
来源：http://hz.nwbrower.top/gtpzeikqpg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yj202588.top/gtaiuxxwda.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zdqjudy.top/gtnlszyrck.html

[A25] 字符串比较
来源：http://hz.316326.xyz/gtzfyhcyeu.html

Py:   s1 == s2; s1 != s2
来源：http://hz.quarkkingdee.top/gtofvvvztz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.xingfuxueyuan.xyz/gtnwdhpplt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydjk.org.cn/gttbxdhjas.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gaohongyu789.top/gtzpnogpji.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.shzxlz.cn/gtwfmuyovn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhengqikj.top/gtwiqgbqcz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinqigfzy.top/gtbmeneqtg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.iojbl.cn/gtfbbbgkyq.html

[A26] 类型转换总览
来源：http://hz.smart0.xyz/gtxbnmauxr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.meibo888.top/gtihknrkcl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.fengsongda.top/gtloghpcck.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sysykeji.top/gtqmejurxl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.daria6918.cn/gtybmyzbpd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xylfe.cn/gtjrgjwlfo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhaomingkeji.xyz/gtsoepgkpe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jianghu66.top/gtltvxclnl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.chenjidiqi.icu/gtvsbnhzlm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtuxuwaizn.html

B. 流程控制
来源：http://hz.sweek.top/gtluzbiyju.html

================================================================================
来源：http://hz.cheryme.top/gtdgeevefg.html

[B01] 条件判断 if / else
来源：http://hz.meibo888.top/gtdtqrtedu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.0kj1m.cn/gtsvmkmnjm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xuanzx.com/gthsbcintf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zycfv.cn/gtadrsxztg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinghuilouyu.cn/gtaixlsinv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xuanzx.com/gtxppqnafo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhongyouzk.top/gtykqkjwwq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cucudq.cn/gtngwymetk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.sufxvd.cn/gtzcgqczbv.html

[B02] 多分支 else if / elif
来源：http://hz.yuxming.cn/gtwiidyers.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yangfankeji.com/gtdwmyngkg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jlsjyb.cn/gtkpvxvnei.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gtswphrsch.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gtrmrtvhwg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtunieeoou.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.dianchejie.cn/gthtctuemk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.vqdsnc.cn/gtduviuboc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shanyushiyangkeji.top/gtckauzcfb.html

[B03] switch / match / case
来源：http://hz.yueranfly.top/gtuzzuylqf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jinyuanbaomall.cn/gtzwxjdewa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.feifeiyinyue.top/gtaopgerme.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.dianchejie.cn/gtuetexyeu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gtxnggobni.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.wangdashe.top/gtyultlhir.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ybcxt.top/gtntjngzxl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.bjfxy.top/gtgdrwecyc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.9152youxi.cn/gtisjtjqde.html

[B04] for 计数循环
来源：http://hz.sweek.top/gtwsinrnka.html

Py:   for i in range(10): print(i)
来源：http://hz.chenlongwang.top/gtepubaoqs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shzxlz.cn/gtibxojcpl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nwbrower.top/gtskgvxqpo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cucudq.cn/gtlcvgrpvc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.tian-w.cn/gtvjnrdyvs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhixingplan.top/gtxkapqwzh.html

Ruby: 10.times { |i| puts i }
来源：http://hz.aibaodan.cn/gtmjfckgqt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.nwbrower.top/gtuyttolhk.html

[B05] 遍历数组 / 列表
来源：http://hz.cashguo.top/gtyznbwhfi.html

Py:   for item in arr: print(item)
来源：http://hz.havefunace.top/gtxclzvhgj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jinqigufen.top/gtzxbwisxu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xylfe.cn/gtemgwyhrh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtaiexwzah.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shangyingyoupin.top/gtnaockglu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jlsjyb.cn/gtjgmorqcw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yongpay.top/gtshxxjbxw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hongshengwenyu.top/gtfwnmaiuf.html

[B06] 遍历字典 / 对象
来源：http://hz.9152youxi.cn/gtcgihdwfp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhixingplan.top/gtpsjyqiva.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cheryme.top/gtdvrsqlvr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xylfe.cn/gtfcghzfbs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ivvv.top/gtbbadxksc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yuxming.cn/gtmccntznv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xingfuxueyuan.xyz/gtwylojhkd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zycfv.cn/gthcuqnzrt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.haohaochexian.top/gtfxcamkhp.html

[B07] while 循环
来源：http://hz.gzhubu.top/gtnthenecw.html

Py:   while i < 10: i += 1
来源：http://hz.zhiwuduotai.top/gtrjtiemkx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jqgfzy.top/gtnnqblvcl.html

JS:   while (i < 10) { i++; }
来源：http://hz.hysaishi.cn/gttgynxubz.html

TS:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gtfwoqegvj.html

Java: while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtdludfvaq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zdqjudy.top/gtjflqswtk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xingfuxueyuan.xyz/gttofueyup.html

C#:   while (i < 10) { i++; }
来源：http://hz.nwbrower.top/gthououfwy.html

[B08] do-while（至少执行一次）
来源：http://hz.hammf.cn/gtshaymfmu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ppjwa.cn/gtlfldyaao.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ydjk.org.cn/gtootlbpwx.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtybuibiee.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gaohongyu789.top/gtfjnyrvvk.html

Java: do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtjzvvhisz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hfpthk.cn/gtezieuvzf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hnxiangtu.top/gtbwzwnljb.html

C#:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtmiaijrhn.html

[B09] break 与 continue
来源：http://hz.hywenlv.cn/gtqtdbamrz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hywenlv.cn/gtenylhuvo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.bjfxy.top/gtfwwfzfnu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtmquygpge.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gthuivxown.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtujjibxvs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hysaishi.cn/gtinikcqwh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shuidangran.top/gtuypxqgud.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtyuzmmlzq.html

[B10] 遍历同时拿索引
来源：http://hz.birdmap.top/gtsourornb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhiwuduotai.top/gttdzorail.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenzaomai.com/gteqoxskaw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinqigufen.top/gtkfiendsk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.quarkkingdee.top/gthaymvgix.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.kuanghao11.cn/gtkrccggmb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xinyue.icu/gtzwqtfdym.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xingfuxueyuan.xyz/gtakqahktd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.snrcjt.cn/gtkimvwroe.html

[B11] 生成数字序列 / 区间
来源：http://hz.hfpthk.cn/gtcprecpvs.html

Py:   list(range(0, 10, 2))
来源：http://hz.yangfankeji.com/gtlqflhokv.html

PHP:  range(0, 10, 2);
来源：http://hz.jqgufenzy.top/gtwymxnfhi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtnffownuy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hywenlv.cn/gtkxeqmppq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.tian-w.cn/gtthniyrlg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.svipenyu.cn/gtswhbglle.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sweek.top/gtogdjrjtw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hfpthk.cn/gtexnomvog.html

[B12] 跳出多层循环
来源：http://hz.aizwys.cn/gtnythhckx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hfpthk.cn/gttvhfugze.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnqzz.top/gtempzkfqr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtwxbseelv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtbopqtkoz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.aizwys.cn/gtgumeuusx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhengqikj.top/gtegzlawph.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sxryk.cn/gtaqzgkvaf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhoulong.xyz/gtlvnhhral.html

[B13] 判断是否为数字
来源：http://hz.yj20258888.top/gtglwvhfoa.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuanzx.com/gtpfndlryn.html

PHP:  is_numeric($x)
来源：http://hz.dianchejie.cn/gtbnojnnmz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.meibo888.top/gtyzdwczdy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ivvv.top/gtzzjewmpa.html

Java: x instanceof Number
来源：http://hz.jinqigufen.top/gtguuwvumk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.iojbl.cn/gtugebmbkm.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangkeji.top/gtogvvwohz.html

C#:   x is int or double or decimal
来源：http://hz.yvedp.cn/gtmtjxlkaz.html

[B14] 判断值是否在集合内
来源：http://hz.yuanzhike.top/gtpodbfsav.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tanke756.top/gtdagittkj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.iojbl.cn/gtbrmsyweg.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.iojbl.cn/gtmuymgaia.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gtmnclgepl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.haohaochexian.top/gtvtdnsoha.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shuidangran.top/gtuoqjfrky.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hysaishi.cn/gteqwnjucl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hammf.cn/gtkhmbyund.html

[B15] 布尔运算与取反
来源：http://hz.xylfe.cn/gtpfsvynlf.html

Py:   a and b or not c
来源：http://hz.hnqzz.top/gtkgxxhrxs.html

PHP:  $a && $b || !$c
来源：http://hz.gotoacloud.top/gtrckhpzhw.html

JS:   a && b || !c
来源：http://hz.yuxming.cn/gtfezbolmr.html

TS:   a && b || !c
来源：http://hz.tianlin.xyz/gtexxfayzl.html

Java: a && b || !c
来源：http://hz.chenjidiqi.icu/gtriirrlsy.html

Go:   a && b || !c
来源：http://hz.tianlin.xyz/gtaduhjdsf.html

Ruby: a && b || !c
来源：http://hz.ydjk.org.cn/gtukjuetdd.html

C#:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtgmmxqnfw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cucudq.cn/gtdcovyuwg.html

Py:   if not data: return
来源：http://hz.316326.xyz/gtzpeojjoz.html

PHP:  if (!$data) { return; }
来源：http://hz.redwolf501.top/gtxzyvzdnq.html

JS:   if (!data) return;
来源：http://hz.yvedp.cn/gtsohrevyh.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gtwebcknhs.html

Java: if (data == null) return;
来源：http://hz.chenlongwang.top/gtgxxjbrcb.html

Go:   if data == nil { return }
来源：http://hz.jinyuanbaomall.cn/gtgjfvncus.html

Ruby: return if data.nil?
来源：http://hz.hywenlv.cn/gtygwdzdnu.html

C#:   if (data == null) return;
来源：http://hz.c1oappe.top/gtmuataszl.html

================================================================================
来源：http://hz.jinqigufen.top/gtlwdpspls.html

C. 函数与作用域
来源：http://hz.cqqwz.cn/gtqbgwpzvg.html

================================================================================
来源：http://hz.daxiang520.top/gtilriuuty.html

[C01] 定义函数
来源：http://hz.nanxuanxn.top/gtmcrjotas.html

Py:   def add(a, b): return a + b
来源：http://hz.shangyingyoupin.top/gtywyeknmu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtvfgvsmnj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtxpilhyta.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtdrjoqjpa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtsygxaakz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shangyingyoupin.top/gtgvudfmzq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.c1oappe.top/gtutlstjzw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtbfpucmrt.html

[C02] 默认参数
来源：http://hz.c1oappe.top/gtkswsxyjc.html

Py:   def greet(name="World"): return name
来源：http://hz.jinqigufen.top/gtmqboppma.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.guowangkeji.top/gtifmxvlni.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gogol.net.cn/gtdozjhtme.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnqzz.top/gtyenizxoc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.havefunace.top/gtnekqkwoo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tianlin.xyz/gtrsbvazxd.html

Ruby: def greet(name = "World") = name
来源：http://hz.yongpay.top/gtozyoyckq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.fengsongda.top/gtfosnzlbu.html

[C03] 可变参数
来源：http://hz.daria6918.cn/gtyexgjlkk.html

Py:   def total(*args): return sum(args)
来源：http://hz.daria6918.cn/gtjklytlpr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dianchejie.cn/gttixklikm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenzaomai.com/gtqtxweoyu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtnsgtlwjk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.fzhhl.top/gtozzcordx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.mhx1999.top/gtcdqisjcd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sweek.top/gtzdgnevxl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.mhx1999.top/gtyjgrjqrt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhixingplan.top/gtjibmqztq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jianghu66.top/gtquvmtjci.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuxming.cn/gtjvhlmfak.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.meibo888.top/gtdihfllxv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ivvv.top/gtccfihxzc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hammf.cn/gtajfyanmt.html

Go:   // 无：用配置结构体参数
来源：http://hz.hywenlv.cn/gtjphgxbmr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtszgmnbrp.html

C#:   f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtfdsgzkkh.html

[C05] 返回多个值
来源：http://hz.cucudq.cn/gtmtivokfs.html

Py:   return a, b
来源：http://hz.meibo888.top/gtgwdhtquv.html

PHP:  return [$a, $b];
来源：http://hz.ppjwa.cn/gtaofpiysd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gogol.net.cn/gtzoghrrzy.html

TS:   return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtgnragwpl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydjk.org.cn/gtutqxedkv.html

Go:   return a, b
来源：http://hz.vqdsnc.cn/gtomyhwfau.html

Ruby: return a, b
来源：http://hz.tanke756.top/gtmnobkdoe.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nanxinkj.top/gtdxwnqwfd.html

[C06] 匿名函数 / lambda
来源：http://hz.sweek.top/gtlznfaqex.html

Py:   square = lambda x: x * x
来源：http://hz.zhongyouzk.top/gtringvwfi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj202588.top/gtbljhfvgg.html

JS:   const square = x => x * x;
来源：http://hz.meibo888.top/gtcsvkatzg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.iojbl.cn/gtbxgcynnm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ybcxt.top/gttavfnmvl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nanxuanxn.top/gtarqubwcq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nwbrower.top/gtcxhhjbos.html


<!-- 参考信息 -->