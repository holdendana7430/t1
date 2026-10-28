代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xylfe.cn/gttffvpsoj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.mhx1999.top/gtecnypvlb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.daria6918.cn/gtfnmwjhxf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtwvfkhzvz.html

[A18] 字符与 ASCII 码互转
来源：http://hz.chenzaomai.com/gtnjlogkwc.html

Py:   ord("A"); chr(65)
来源：http://hz.hnxiangtu.top/gtyqbnjump.html

PHP:  ord("A"); chr(65)
来源：http://hz.hfpthk.cn/gtowsvchje.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sysykeji.top/gtvbvibxyu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.52xcode.cn/gtshrkegjr.html

Java: (int) 'A'; (char) 65
来源：http://hz.jqgfzy.top/gtuizkfaao.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.smart0.xyz/gtiwcxyjoy.html

Ruby: "A".ord; 65.chr
来源：http://hz.shangyingyoupin.top/gtorglqeig.html

C#:   (int)'A'; (char)65
来源：http://hz.jqgfzy.top/gttwgoexgk.html

[A19] 交换两个变量
来源：http://hz.yvedp.cn/gtkuyezyac.html

Py:   a, b = b, a
来源：http://hz.feifeiyinyue.top/gtbmlvsvgk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shzxlz.cn/gthezlbote.html

JS:   [a, b] = [b, a];
来源：http://hz.9152youxi.cn/gtmbdxjqtz.html

TS:   [a, b] = [b, a];
来源：http://hz.cqqwz.cn/gtedxtggeu.html

Java: int t = a; a = b; b = t;
来源：http://hz.daxiang520.top/gtztbepbhr.html

Go:   a, b = b, a
来源：http://hz.xylfe.cn/gtammlegla.html

Ruby: a, b = b, a
来源：http://hz.zdqjudy.top/gtbrghpyaq.html

C#:   (a, b) = (b, a);
来源：http://hz.jqgufenzy.top/gtqahcxqxs.html

[A20] 读取标准输入
来源：http://hz.sweek.top/gtlvvshdij.html

Py:   name = input("请输入：")
来源：http://hz.wangdashe.top/gtpelnyfzd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.dianchejie.cn/gtucfvpbiv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.nanxuanxn.top/gtcnzaknwx.html

TS:   // Node.js：readline 模块
来源：http://hz.haohaochexian.top/gtnnfnugox.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yj202588.top/gtiuyfyxxg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.hammf.cn/gteaqunvax.html

Ruby: gets.chomp
来源：http://hz.jinqigufen.top/gtlyzpidis.html

C#:   Console.ReadLine();
来源：http://hz.hfpthk.cn/gtyuizdtkq.html

[A21] 保留指定小数位输出
来源：http://hz.zhixingplan.top/gteyqakpho.html

Py:   f"{3.14159:.2f}"
来源：http://hz.shzxlz.cn/gthudvwjhf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yonumen.top/gtmlxizthk.html

JS:   (3.14159).toFixed(2)
来源：http://hz.xziqi.cn/gtlretqcid.html

TS:   (3.14159).toFixed(2)
来源：http://hz.c1oappe.top/gtruxzqelo.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yj20258888.top/gtnclypyai.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.aibaodan.cn/gtncuwmiyp.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zycfv.cn/gtcjwtglcn.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhixingplan.top/gtzxahdske.html

[A22] 获取字符串长度
来源：http://hz.haohaochexian.top/gtkezfalte.html

Py:   len(s)
来源：http://hz.316326.xyz/gtpbwlszxh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.0kj1m.cn/gtduqtdkde.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.nanxinkj.top/gtauowfelv.html

TS:   s.length
来源：http://hz.shuidangran.top/gtwtnfigil.html

Java: s.length()
来源：http://hz.jinghuilouyu.cn/gtfjqdtjyq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cqqwz.cn/gthvawqhpo.html

Ruby: s.length
来源：http://hz.dianchejie.cn/gterrtwpnj.html

C#:   s.Length
来源：http://hz.tianlin.xyz/gtgoqqtxje.html

[A23] 大小写转换
来源：http://hz.ydjk.org.cn/gtvvutguni.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.tian-w.cn/gtpsxdkzxv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cashguo.top/gtlijudaob.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xylfe.cn/gtjuanoktq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.birdmap.top/gtarkkseyj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.ivvv.top/gtbmrpmzmi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.cheryme.top/gteeqtyrus.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.meibo888.top/gtbkrbrgvl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.guowangkeji.top/gtkkuxxbgc.html

[A24] 去除首尾空白
来源：http://hz.dashuyun.cn/gtlbvczadv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yj20258888.top/gtrottxnbn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.kuanghao11.cn/gtkplbnxuo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhixingplan.top/gtvinsdhzf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangshuangyany.cn/gtusncnfgp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.zhengqikj.top/gtziwcfcng.html

Go:   strings.TrimSpace(s)
来源：http://hz.ehwqpu.com/gtpibtktjm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yongpay.top/gtxovdpbfd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hammf.cn/gtbvwpdync.html

[A25] 字符串比较
来源：http://hz.svipenyu.cn/gtrvuykhyb.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cdnleiting.top/gtxreflfqk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jyoumei.cn/gtfrgibhdi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shzxlz.cn/gtptfszyei.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.9152youxi.cn/gtsmqiqemy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jinqigufen.top/gtwmjwozcv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.xylfe.cn/gtzozmbigt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.9152youxi.cn/gtktynlnuu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.bjfxy.top/gtxwjjmyum.html

[A26] 类型转换总览
来源：http://hz.chenzaomai.com/gtapwexpsk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.gotoacloud.top/gtqhaoiosw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.pengpengdd.cyou/gtbnshlxzu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.nanxinkj.top/gtaaerqulb.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhixingplan.top/gtmgzrnfyz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.sysykeji.top/gtatxivexx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.sufxvd.cn/gttcomasgs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.feifeiyinyue.top/gtysbbinig.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hammf.cn/gtymbhdfiv.html

================================================================================
来源：http://hz.yuanzhike.top/gtuhedjtgm.html

B. 流程控制
来源：http://hz.sweek.top/gtpcbotdfb.html

================================================================================
来源：http://hz.xylfe.cn/gtbmhgxbwn.html

[B01] 条件判断 if / else
来源：http://hz.nwbrower.top/gtwwqvojbb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ehwqpu.com/gtgrnzfpoa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.gogol.net.cn/gtozqsolso.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.redwolf501.top/gtuhlvkuaj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jqgufenzy.top/gtfjrqrgca.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.vqdsnc.cn/gtjdftwhuz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yuanzhike.top/gtobglyyyg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.chenjidiqi.icu/gtelgdrdpq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gtwapqopxp.html

[B02] 多分支 else if / elif
来源：http://hz.jiagoushi.top/gtyijtcayz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhixingplan.top/gtohuexzew.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.cdnleiting.top/gtpsmdpewg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gtufklbyhn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhaomingkeji.xyz/gtseiueboo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.svipenyu.cn/gtmzlvvhtz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.316326.xyz/gtlwldoryh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zycfv.cn/gtseatwrdi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.feifeiyinyue.top/gtpzarxqbe.html

[B03] switch / match / case
来源：http://hz.daxiang520.top/gtoaiifhbl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.316326.xyz/gtfkewyeha.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.kuanghao11.cn/gtfawubemg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhaomingkeji.xyz/gtsrymgacz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gaohongyu789.top/gtqpigpvxa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.haohaochexian.top/gteeczvcxb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.sweek.top/gtjunsjjnm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shanyushiyangtech.top/gtyqdkvrni.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jqgfzy.top/gtcfjnsgpu.html

[B04] for 计数循环
来源：http://hz.nanxuanxn.top/gtvirvqgtt.html

Py:   for i in range(10): print(i)
来源：http://hz.shangyingyoupin.top/gtutihdfji.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.9152youxi.cn/gtxllxfgnj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pengpengdd.cyou/gtwwgloqai.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuanzx.com/gtwpolzadh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shangyingyoupin.top/gtykhxobao.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ybcxt.top/gtnxwftiko.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xingfuxueyuan.xyz/gtihbcmsgt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.guowangkeji.top/gtmtdrbfin.html

[B05] 遍历数组 / 列表
来源：http://hz.svipenyu.cn/gtsptomqom.html

Py:   for item in arr: print(item)
来源：http://hz.hysaishi.cn/gtijuzzmzz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gaohongyu789.top/gtjqiqnmjm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.kuanghao11.cn/gtpdzmiuvn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.havefunace.top/gtuatmsyxj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhiwuduotai.top/gtvkiftdez.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.sxryk.cn/gtbpctwqfq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ybcxt.top/gtbnimekfc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.52xcode.cn/gtdkofetxm.html

[B06] 遍历字典 / 对象
来源：http://hz.aibaodan.cn/gtnfuihiyb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhongyouzk.top/gtgzjigvta.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jlsjyb.cn/gtovcyetbt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fzhhl.top/gtbpruqkec.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fzhhl.top/gtzjsueqhh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hnqzz.top/gtjykujflu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xylfe.cn/gtfgerbcns.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.pycfn.com/gthodzhsro.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinqigfzy.top/gtbtvzhcwe.html

[B07] while 循环
来源：http://hz.zhixingplan.top/gttqklutwo.html

Py:   while i < 10: i += 1
来源：http://hz.cucudq.cn/gtejyejent.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.sufxvd.cn/gtxgkxqhne.html

JS:   while (i < 10) { i++; }
来源：http://hz.hysaishi.cn/gtqjdewlyy.html

TS:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtosbqgikf.html

Java: while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtkahcegkk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jqgfzy.top/gtalwdcrnz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.chenlongwang.top/gtxjlfykko.html

C#:   while (i < 10) { i++; }
来源：http://hz.ybcxt.top/gtarfgxlpp.html

[B08] do-while（至少执行一次）
来源：http://hz.nanxinkj.top/gtljuuxlql.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hammf.cn/gtqxnresbh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hfpthk.cn/gtogssrskz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.aizwys.cn/gtadtbbbkq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtjzmhrhnj.html

Java: do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtklfymbqq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shangyingyoupin.top/gtxvneatqw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.dashuyun.cn/gttsqywgrq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gttuccbwnw.html

[B09] break 与 continue
来源：http://hz.fzhhl.top/gttxnlqtur.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xuetiantiany.cn/gtbiqoujfs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ybcxt.top/gtkpntgjlt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtrzzboesb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tian-w.cn/gttxnzzlbz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtnhoknvkf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xylfe.cn/gtwfiiygsk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yj20258.top/gtrfihkpdk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtcekpylfh.html

[B10] 遍历同时拿索引
来源：http://hz.cqqwz.cn/gtfmokyqkx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhoulong.xyz/gtcswkxrkg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zdqjudy.top/gtvoqgcjkf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.52xcode.cn/gtoxchhdko.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jqgfzy.top/gtbupkufxi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cucudq.cn/gtcqjuyxow.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shanyushiyangtech.top/gtcbahlbgo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gaohongyu789.top/gtbfdbemsr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xinyue.icu/gtgeckizzm.html

[B11] 生成数字序列 / 区间
来源：http://hz.ivvv.top/gtktxkzjjr.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuanzx.com/gtkxkqcdiq.html

PHP:  range(0, 10, 2);
来源：http://hz.dianchejie.cn/gtpnthtgwu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.mhx1999.top/gtmdsvrdyv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnxiangtu.top/gtpzqsmyui.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zdqjudy.top/gttihmpnwd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xinyue.icu/gthfhpdxbw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.redwolf501.top/gtdqxouxyn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shangyingyoupin.top/gtwwurmdfd.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangtech.top/gtstzcqswx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gtuatqemqw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.pycfn.com/gthyfbtnpe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtajckvomf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtdtioxsum.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtcpiihrmc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nanxinkj.top/gtwnnwcidw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj202588.top/gtsuqqvhgc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ydjk.org.cn/gtjaxabdey.html

[B13] 判断是否为数字
来源：http://hz.jianghu66.top/gtmydkusyc.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenlongwang.top/gtkiooayes.html

PHP:  is_numeric($x)
来源：http://hz.hywenlv.cn/gteoqrughl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ehwqpu.com/gtwezsdluo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gtyrfinmoa.html

Java: x instanceof Number
来源：http://hz.yangfankeji.com/gtbpnpxyhz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sxryk.cn/gthjaefbrp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.9152youxi.cn/gtuttnjvuq.html

C#:   x is int or double or decimal
来源：http://hz.jqgfzy.top/gtlvvrhheo.html

[B14] 判断值是否在集合内
来源：http://hz.jqgufenzy.top/gtbeexotnp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.snrcjt.cn/gtvsengpaw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hnxiangtu.top/gthyvgcmyu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.wangdashe.top/gtxeamzcnj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yj202588.top/gtjgdvcxxa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hysaishi.cn/gtvcnrmykg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenlongwang.top/gtlnrjiipr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuanzhike.top/gtfixqzeaw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aibaodan.cn/gtokdpxgqa.html

[B15] 布尔运算与取反
来源：http://hz.fzhhl.top/gtsvyvsrda.html

Py:   a and b or not c
来源：http://hz.zdqjudy.top/gtxdczudfp.html

PHP:  $a && $b || !$c
来源：http://hz.chenzaomai.com/gtogwwljbn.html

JS:   a && b || !c
来源：http://hz.cqqwz.cn/gtcnjpcloz.html

TS:   a && b || !c
来源：http://hz.guowangkeji.top/gtqhcgmuce.html

Java: a && b || !c
来源：http://hz.dashuyun.cn/gtzdskfqhm.html

Go:   a && b || !c
来源：http://hz.tanke756.top/gtswiarzsu.html

Ruby: a && b || !c
来源：http://hz.jiagoushi.top/gtedqrudnb.html

C#:   a && b || !c
来源：http://hz.xziqi.cn/gtxwbufsif.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.vqdsnc.cn/gtjokwvpep.html

Py:   if not data: return
来源：http://hz.yvedp.cn/gthsapxffw.html

PHP:  if (!$data) { return; }
来源：http://hz.dianchejie.cn/gtztdbciqd.html

JS:   if (!data) return;
来源：http://hz.yvedp.cn/gtyxhnfofc.html

TS:   if (!data) return;
来源：http://hz.cucudq.cn/gtifcvcsji.html

Java: if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtmwxxkfpd.html

Go:   if data == nil { return }
来源：http://hz.xylfe.cn/gtdrpepfvj.html

Ruby: return if data.nil?
来源：http://hz.jqgufenzy.top/gtxkftcbnf.html

C#:   if (data == null) return;
来源：http://hz.meibo888.top/gtblmguyqi.html

================================================================================
来源：http://hz.daria6918.cn/gtmkzdpmrg.html

C. 函数与作用域
来源：http://hz.yj20258.top/gtiqyrgrwc.html

================================================================================
来源：http://hz.jiagoushi.top/gtfspimphg.html

[C01] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtmmcekoej.html

Py:   def add(a, b): return a + b
来源：http://hz.chenzaomai.com/gtgkbyeqif.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtnbmjrhyh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.svipenyu.cn/gtismrzkbd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.birdmap.top/gtbuzgbolo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtyzlwccqa.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gzhubu.top/gtzqkpywfk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hfpthk.cn/gtadskxctf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtwrwzstit.html

[C02] 默认参数
来源：http://hz.sufxvd.cn/gtdqfbcbmo.html

Py:   def greet(name="World"): return name
来源：http://hz.sxryk.cn/gtmlukzvef.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.9152youxi.cn/gtdzssivla.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nwbrower.top/gtphtnntlc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sweek.top/gtumfygyvx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nwbrower.top/gtqmlkjspp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.52xcode.cn/gtkgomjfcs.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gtpbmbxfgd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.aibaodan.cn/gtzmeyrven.html

[C03] 可变参数
来源：http://hz.bjfxy.top/gtwpzgessg.html

Py:   def total(*args): return sum(args)
来源：http://hz.bjfxy.top/gtwfvovyva.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.9152youxi.cn/gtkvmhlaxv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258.top/gtqddyqnnq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hywenlv.cn/gtywyshcha.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhaomingkeji.xyz/gtzbujztex.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuetiantiany.cn/gtncbvfrna.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guowangkeji.top/gtrmacxqdh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fzhhl.top/gtgzhicpcn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jyoumei.cn/gtisujedma.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hywenlv.cn/gtvchouvsz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.aibaodan.cn/gtzdxjjeaa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtmcbmvyby.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jiagoushi.top/gtsldvhthw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guowangkeji.top/gtmtihiwoi.html

Go:   // 无：用配置结构体参数
来源：http://hz.c1oappe.top/gtgijdclcv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtgpaarsse.html

C#:   f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtpqojaqtm.html

[C05] 返回多个值
来源：http://hz.fengsongda.top/gtdtfuxswl.html

Py:   return a, b
来源：http://hz.shuidangran.top/gtfbxxlbtn.html

PHP:  return [$a, $b];
来源：http://hz.jqgfzy.top/gthyheokfa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jianghu66.top/gtgxofecnn.html

TS:   return { a, b };
来源：http://hz.sysykeji.top/gtfmdcojlz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gaohongyu789.top/gtkegbwcfh.html

Go:   return a, b
来源：http://hz.zhiwuduotai.top/gtdnnftdiq.html

Ruby: return a, b
来源：http://hz.hfpthk.cn/gtabdydaao.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sweek.top/gtkxkivcyk.html

[C06] 匿名函数 / lambda
来源：http://hz.yanxiufei.cn/gtxxlttshv.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangtech.top/gthidwbpqh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gaohongyu789.top/gtcfzjauet.html

JS:   const square = x => x * x;
来源：http://hz.zycfv.cn/gtejsgsnem.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.andypj.xyz/gtzkfiflty.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.andypj.xyz/gtndeellbj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.9152youxi.cn/gtfrdnrimk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhengqikj.top/gtunysqjkv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dianchejie.cn/gtuvkrmzsa.html

[C07] 把函数作为参数传入
来源：http://hz.ydjk.org.cn/gtisvuszgm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dashuyun.cn/gtuuimpxzk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gzhubu.top/gtqvyfbpet.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xuetiantiany.cn/gtseorpadr.html

TS:   arr.map(String)
来源：http://hz.yangfankeji.com/gtpnztdbcc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ywan-chungtsiang.top/gtkmaqvkak.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zdqjudy.top/gtpnmqlrez.html

Ruby: arr.map(&:upcase)
来源：http://hz.jlsjyb.cn/gtykakphhr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtbclyzpur.html

[C08] 闭包
来源：http://hz.shanyushiyangkeji.top/gtxrbliesm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gthjxdksxe.html


<!-- 参考信息 -->