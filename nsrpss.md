代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.havefunace.top/gttyhdczjq.html

[A15] 空值判断与默认值
来源：http://hz.yuxming.cn/gtfjzjxqim.html

Py:   value = data or "默认值"
来源：http://hz.jinyuanbaomall.cn/gtajqufjuo.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.cdnleiting.top/gtrjnzcdve.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhiwuduotai.top/gtbkhqdblv.html

TS:   const value = data ?? "默认值";
来源：http://hz.yangfankeji.com/gtrjjrywlw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shanyushiyangtech.top/gtfcgprfit.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jiagoushi.top/gtxnyhylar.html

Ruby: value = data || "默认值"
来源：http://hz.chenzaomai.com/gtmwsgxsih.html

C#:   var value = data ?? "默认值";
来源：http://hz.sweek.top/gtroznwcrv.html

[A16] 真假值判断规则
来源：http://hz.zhengqikj.top/gtrcceyhtk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yongpay.top/gtfxcyhjtf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.shzxlz.cn/gtzvsrzlkf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zhongyouzk.top/gtmivpovpe.html

TS:   if (!x) {}
来源：http://hz.sxryk.cn/gtjsoryonb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.ydjk.org.cn/gthwzwvyrz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yanxiufei.cn/gtooaibmww.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.kuanghao11.cn/gtnmphnlnw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.ydjk.org.cn/gthhahsjek.html

[A17] 位运算
来源：http://hz.zhengqikj.top/gthghvebkc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangshuangyany.cn/gtplixolad.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.xinyue.icu/gtuszokimy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtxlfzrcri.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yongpay.top/gtvygfczoj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.mhx1999.top/gtjspseknl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtwxulfski.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shangyingyoupin.top/gtuyfbkhzj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cashguo.top/gtdprpzagv.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ehwqpu.com/gtatgtkvxl.html

Py:   ord("A"); chr(65)
来源：http://hz.shanyushiyangtech.top/gtrxcjkxiw.html

PHP:  ord("A"); chr(65)
来源：http://hz.jianghu66.top/gtmfcqiyku.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yuanzhike.top/gtonvupuik.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.chenjidiqi.icu/gtclfqsihq.html

Java: (int) 'A'; (char) 65
来源：http://hz.cheryme.top/gtmxziqyxs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.nwbrower.top/gtrxxdozct.html

Ruby: "A".ord; 65.chr
来源：http://hz.gzhubu.top/gtnnhgwqyb.html

C#:   (int)'A'; (char)65
来源：http://hz.hnqzz.top/gtztraizpy.html

[A19] 交换两个变量
来源：http://hz.jianghu66.top/gtvedncgfy.html

Py:   a, b = b, a
来源：http://hz.smart0.xyz/gtwkurhgqm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.ivvv.top/gtnnxelksi.html

JS:   [a, b] = [b, a];
来源：http://hz.zhiwuduotai.top/gtuqrbgzqx.html

TS:   [a, b] = [b, a];
来源：http://hz.svipenyu.cn/gtaoiwvgxi.html

Java: int t = a; a = b; b = t;
来源：http://hz.xuetiantiany.cn/gtbunohiaw.html

Go:   a, b = b, a
来源：http://hz.zhongyouzk.top/gtwpmrkdpr.html

Ruby: a, b = b, a
来源：http://hz.aizwys.cn/gtnimpfysv.html

C#:   (a, b) = (b, a);
来源：http://hz.shanyushiyangkeji.top/gtzodngfgu.html

[A20] 读取标准输入
来源：http://hz.pycfn.com/gtovsvppix.html

Py:   name = input("请输入：")
来源：http://hz.gotoacloud.top/gtatzbjege.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.haohaochexian.top/gtdnektwhr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zycfv.cn/gtfpmhoiqq.html

TS:   // Node.js：readline 模块
来源：http://hz.52xcode.cn/gtrngfhyjf.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.bjfxy.top/gtahmaaqtk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jinyuanbaomall.cn/gtapsspsgc.html

Ruby: gets.chomp
来源：http://hz.xuetiantiany.cn/gtqhyrxang.html

C#:   Console.ReadLine();
来源：http://hz.fengsongda.top/gtqagiunvq.html

[A21] 保留指定小数位输出
来源：http://hz.ywan-chungtsiang.top/gtzajsbjha.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ivvv.top/gtnzuaunsa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gtcoscdiya.html

JS:   (3.14159).toFixed(2)
来源：http://hz.pycfn.com/gtooxnnhsi.html

TS:   (3.14159).toFixed(2)
来源：http://hz.hnqzz.top/gthubqmdxt.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.kuanghao11.cn/gtgmmvqstu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.dashuyun.cn/gtfjdligkm.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zhijiandao.cn/gthhcjzjyy.html

C#:   3.14159.ToString("F2")
来源：http://hz.yanxiufei.cn/gtqyqpvwhx.html

[A22] 获取字符串长度
来源：http://hz.ppjwa.cn/gtnmeishas.html

Py:   len(s)
来源：http://hz.nanxuanxn.top/gtsciqfmrz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.shzxlz.cn/gtlwxysfct.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhaomingkeji.xyz/gtgeqwgmfc.html

TS:   s.length
来源：http://hz.hnxiangtu.top/gtncfsutfx.html

Java: s.length()
来源：http://hz.meibo888.top/gtliyyoqjv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.wangshuangyany.cn/gtighjpmjw.html

Ruby: s.length
来源：http://hz.gzhubu.top/gtqefqptvt.html

C#:   s.Length
来源：http://hz.jyoumei.cn/gtcyjsncez.html

[A23] 大小写转换
来源：http://hz.yuxming.cn/gtkorthqvd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.pycfn.com/gtmupicnrn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.birdmap.top/gtutlcefad.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ehwqpu.com/gttsiqazmq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj202588.top/gtvgvnfcjt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.sysykeji.top/gtqdzvfvje.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.hongshengwenyu.top/gtnhhydvkd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.cheryme.top/gttarfgqcm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.andypj.xyz/gtolrfessx.html

[A24] 去除首尾空白
来源：http://hz.feifeiyinyue.top/gtgrbsbeje.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shangyingyoupin.top/gtnsawqjgr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.sweek.top/gtcxuofcon.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.dianchejie.cn/gtuqigbdix.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.dashuyun.cn/gtfcuprbeb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shanyushiyangtech.top/gtqnrgbqej.html

Go:   strings.TrimSpace(s)
来源：http://hz.hfpthk.cn/gtaulyusdj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.c1oappe.top/gtqnsyjkfj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jinqigufen.top/gtqdvkwapt.html

[A25] 字符串比较
来源：http://hz.jiagoushi.top/gtyuzakvoq.html

Py:   s1 == s2; s1 != s2
来源：http://hz.tianlin.xyz/gtpqwkakki.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jyoumei.cn/gtmiehkwcu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daxiang520.top/gtzjqsifcs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jlsjyb.cn/gtajwuldtv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.nanxuanxn.top/gtnfxcjacv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jianghu66.top/gtgwhetyvi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jlsjyb.cn/gtrbhcugir.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.9152youxi.cn/gtrbljutzx.html

[A26] 类型转换总览
来源：http://hz.jinqigufen.top/gtlhrehetm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jinqigfzy.top/gtgoiuptva.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.iojbl.cn/gtbgftqotd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hfpthk.cn/gtsmwexacd.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xinyue.icu/gtwoljzmeq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhiwuduotai.top/gtlozbfjgy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhongyouzk.top/gthrrettyg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhaomingkeji.xyz/gtatxwdhdr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xingfuxueyuan.xyz/gtsgkjxvul.html

================================================================================
来源：http://hz.yongpay.top/gtdmocmywg.html

B. 流程控制
来源：http://hz.gogol.net.cn/gtnegzemur.html

================================================================================
来源：http://hz.xuanzx.com/gtabrgccrx.html

[B01] 条件判断 if / else
来源：http://hz.shuidangran.top/gtmxdmfctb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ydjk.org.cn/gttkzkroau.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ydzc1.top/gtgtlbnfio.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.wangdashe.top/gtlovplgwf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtrjmxsjxp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gzhubu.top/gtifkjfkma.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hywenlv.cn/gthdkrpqeo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yangfankeji.com/gtjluhvezn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hammf.cn/gtfogrbixe.html

[B02] 多分支 else if / elif
来源：http://hz.ehwqpu.com/gtaxazmxfh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yvedp.cn/gtqfihdral.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.smart0.xyz/gtfivzaoiz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinyuanbaomall.cn/gtemsmlpdr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydjk.org.cn/gtzcullhpa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtwnfuegzz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.wangdashe.top/gtidnxqfxv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.smart0.xyz/gtoaoyosnf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258.top/gtwiqqawuh.html

[B03] switch / match / case
来源：http://hz.yongpay.top/gtkufkqiya.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xinyue.icu/gtbodxkzdw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ppjwa.cn/gtlocmgemy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigfzy.top/gtsfznoybz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhixingplan.top/gtflqnmxsu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.316326.xyz/gttdmewaen.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jyoumei.cn/gtyxiifjoj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.gotoacloud.top/gtxxhwwggk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xinyue.icu/gtdizznvin.html

[B04] for 计数循环
来源：http://hz.xinyue.icu/gtiahhbdnt.html

Py:   for i in range(10): print(i)
来源：http://hz.hfpthk.cn/gthgtwarxd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shzxlz.cn/gtjspztlye.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinqigfzy.top/gthhcbafcy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.fzhhl.top/gtkyitzmcf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.nwbrower.top/gtkchcubpc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.0kj1m.cn/gtbsbfykyc.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xingfuxueyuan.xyz/gttbtcrozl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.smart0.xyz/gtzdkittgo.html

[B05] 遍历数组 / 列表
来源：http://hz.birdmap.top/gtbcrmahjm.html

Py:   for item in arr: print(item)
来源：http://hz.havefunace.top/gtnphbwosg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.smart0.xyz/gtkwtjlqeb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jianghu66.top/gtkwsyewup.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhiwuduotai.top/gtxjcbuhwu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.tanke756.top/gtthzbsfjy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ydjk.org.cn/gtamvivirp.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj20258.top/gtgbvzagix.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.quarkkingdee.top/gtecaprplu.html

[B06] 遍历字典 / 对象
来源：http://hz.0kj1m.cn/gtasigkxoq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hfpthk.cn/gtuikqfoft.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ppjwa.cn/gtafjmrafa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.tianlin.xyz/gtgmzbtjds.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yangfankeji.com/gtbflpcybq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.mhx1999.top/gtgjgghuvs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xuetiantiany.cn/gtoepofsjm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.feifeiyinyue.top/gtbuqhspsl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xingfuxueyuan.xyz/gtcjxlqdeo.html

[B07] while 循环
来源：http://hz.redwolf501.top/gtpcqgtcyv.html

Py:   while i < 10: i += 1
来源：http://hz.yvedp.cn/gtmcgoehuw.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.redwolf501.top/gtfivplpst.html

JS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangkeji.top/gtmnzkxdoe.html

TS:   while (i < 10) { i++; }
来源：http://hz.shangyingyoupin.top/gtvvmammas.html

Java: while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtbxffhnqk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xylfe.cn/gtcoknkdrz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.snrcjt.cn/gtawznrfha.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinqigfzy.top/gtvxwxffgy.html

[B08] do-while（至少执行一次）
来源：http://hz.zycfv.cn/gtvngcztph.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ydjk.org.cn/gtchllsfsc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhixingplan.top/gthrzidxwc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtozvlurrw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtkpjafhrz.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtilegypiy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.aibaodan.cn/gtzyvanglu.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zycfv.cn/gtypqyaqwn.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtlgsfgmug.html

[B09] break 与 continue
来源：http://hz.fengsongda.top/gtdletojeb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ydzc1.top/gtrodvacda.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yueranfly.top/gtpekaexfs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.kuanghao11.cn/gtoxhitlhf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtsjlnhsgq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtbhkdybnr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cqqwz.cn/gtzvsjirqn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nanxuanxn.top/gtgnshbquv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtusljwuyn.html

[B10] 遍历同时拿索引
来源：http://hz.aibaodan.cn/gtbkcwgidf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhongyouzk.top/gthobpbzyl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.0kj1m.cn/gtyjgzbkum.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.316326.xyz/gtklkggbrk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jyoumei.cn/gtgmbeiupp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shzxlz.cn/gtwneirxje.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guannengcc.top/gtxzieegsn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.dianchejie.cn/gtgouzdmzt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinghuilouyu.cn/gtkesffcbv.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgufenzy.top/gtikqgjyvp.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhiwuduotai.top/gtripjqdgw.html

PHP:  range(0, 10, 2);
来源：http://hz.nanxinkj.top/gtngiavyli.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtyltddesv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gtdirtuylv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ybcxt.top/gtwjkhxfzw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shanyushiyangkeji.top/gtovdteetu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hfpthk.cn/gtxysnkrbg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sufxvd.cn/gtouzgtnkk.html

[B12] 跳出多层循环
来源：http://hz.xziqi.cn/gtbhedjdxn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.meibo888.top/gtgrxbtzwr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guowangkeji.top/gtuqgnxnwl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhongyouzk.top/gtdhltjyma.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtipiuomnz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtpmnxdbvr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yuxming.cn/gtjkwfgynq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shanyushiyangkeji.top/gtouecygkk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tianlin.xyz/gtpjqnwxlf.html

[B13] 判断是否为数字
来源：http://hz.cucudq.cn/gtbuemncea.html

Py:   isinstance(x, (int, float))
来源：http://hz.jyoumei.cn/gtjpwikzfn.html

PHP:  is_numeric($x)
来源：http://hz.shanyushiyangkeji.top/gtnatxnzhr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yonumen.top/gtujctlfyt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.0kj1m.cn/gtprnpxzbo.html

Java: x instanceof Number
来源：http://hz.jiagoushi.top/gtwnuellgx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.andypj.xyz/gtxsahktny.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuanzhike.top/gtwercoxua.html

C#:   x is int or double or decimal
来源：http://hz.yuanzhike.top/gtsksloeww.html

[B14] 判断值是否在集合内
来源：http://hz.redwolf501.top/gtmdtooexk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenlongwang.top/gtkmbhdoui.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yuxming.cn/gtudbszagl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.vqdsnc.cn/gtucbutbow.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gtpevfxrbd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.c1oappe.top/gtpjjxfhtv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jianghu66.top/gtipyzbgor.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.fengsongda.top/gtbldxmsvx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.meibo888.top/gtmqlmhxmg.html

[B15] 布尔运算与取反
来源：http://hz.sweek.top/gtwgtdjpht.html

Py:   a and b or not c
来源：http://hz.nanxinkj.top/gtkgdzkccc.html

PHP:  $a && $b || !$c
来源：http://hz.guowangkeji.top/gtfznqsvxb.html

JS:   a && b || !c
来源：http://hz.havefunace.top/gtettluwci.html

TS:   a && b || !c
来源：http://hz.shuidangran.top/gtywakudxy.html

Java: a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtwjczsolq.html

Go:   a && b || !c
来源：http://hz.zdqjudy.top/gttbcatgtb.html

Ruby: a && b || !c
来源：http://hz.nwbrower.top/gthphadaqq.html

C#:   a && b || !c
来源：http://hz.yonumen.top/gthumrjtki.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.c1oappe.top/gtsviixwyb.html

Py:   if not data: return
来源：http://hz.yj20258.top/gtfmbpyooe.html

PHP:  if (!$data) { return; }
来源：http://hz.c1oappe.top/gtvetuseel.html

JS:   if (!data) return;
来源：http://hz.gotoacloud.top/gtfcnguuyh.html

TS:   if (!data) return;
来源：http://hz.zdqjudy.top/gttcvqrzfo.html

Java: if (data == null) return;
来源：http://hz.zhoulong.xyz/gtwqcqvclc.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gtjorrnigc.html

Ruby: return if data.nil?
来源：http://hz.9152youxi.cn/gtrirwybzu.html

C#:   if (data == null) return;
来源：http://hz.sweek.top/gtzhezrqoi.html

================================================================================
来源：http://hz.cqqwz.cn/gtlerjeilv.html

C. 函数与作用域
来源：http://hz.hongshengwenyu.top/gtktmucsbi.html

================================================================================
来源：http://hz.meibo888.top/gtyhefqmce.html

[C01] 定义函数
来源：http://hz.shangyingyoupin.top/gtpeqijmpl.html

Py:   def add(a, b): return a + b
来源：http://hz.aizwys.cn/gtfdenhwov.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtqxbrxwaz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xinyue.icu/gtgfxqfgel.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yvedp.cn/gthtombhua.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtjcunobiy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hywenlv.cn/gtrzwasktp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yanxiufei.cn/gtunamoptt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gteglpwxuy.html

[C02] 默认参数
来源：http://hz.daxiang520.top/gtozlwxtwt.html

Py:   def greet(name="World"): return name
来源：http://hz.ydjk.org.cn/gtvcqbigsb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinyuanbaomall.cn/gtxjokbnha.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shangyingyoupin.top/gthgogjmqi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj20258.top/gtysfjswmd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cdnleiting.top/gtbjmfwjem.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ehwqpu.com/gtmkgzngti.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydzc1.top/gtgqxbcbpk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yuanzhike.top/gtmgwnqbog.html

[C03] 可变参数
来源：http://hz.jqgufenzy.top/gtynjejgvr.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenzaomai.com/gtkdnvdprc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gzhubu.top/gtjlvtffvt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.52xcode.cn/gtmlvsacnv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtmyfhrldo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guowangkeji.top/gtrbkqiahp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj202588.top/gtqifgowvs.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhiwuduotai.top/gtoqnqjvku.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnxiangtu.top/gtmyedmamm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gotoacloud.top/gttvcpplwu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.meibo888.top/gtutfvxkdy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.birdmap.top/gtxpeihrls.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtwjyhekds.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenlongwang.top/gtfndhzerg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xingfuxueyuan.xyz/gtrreenjdv.html

Go:   // 无：用配置结构体参数
来源：http://hz.kuanghao11.cn/gtkazbxorc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtqbsbmyzq.html

C#:   f(a: 1, b: 2)
来源：http://hz.cqqwz.cn/gtqhidynrp.html

[C05] 返回多个值
来源：http://hz.yonumen.top/gttgffuwao.html

Py:   return a, b
来源：http://hz.zhiwuduotai.top/gtkrkpfrcl.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtlqnejykf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.meibo888.top/gtuzmbkjug.html

TS:   return { a, b };
来源：http://hz.ybcxt.top/gtebpmajug.html


<!-- 参考信息 -->