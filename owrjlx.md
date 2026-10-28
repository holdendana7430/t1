代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.yuanzhike.top/gtisjktbcb.html

Py:   ord("A"); chr(65)
来源：http://hz.hongshengwenyu.top/gtgjgiwhex.html

PHP:  ord("A"); chr(65)
来源：http://hz.xuetiantiany.cn/gtvkiyrqnn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.fzhhl.top/gtclsonokl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shuidangran.top/gtfvansitt.html

Java: (int) 'A'; (char) 65
来源：http://hz.nwbrower.top/gtnqzpxkea.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.iojbl.cn/gtawnmvdro.html

Ruby: "A".ord; 65.chr
来源：http://hz.svipenyu.cn/gtzdwipbdq.html

C#:   (int)'A'; (char)65
来源：http://hz.xingfuxueyuan.xyz/gtquvoxsmw.html

[A19] 交换两个变量
来源：http://hz.iojbl.cn/gtcjotnrhn.html

Py:   a, b = b, a
来源：http://hz.meibo888.top/gtzumgpknz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.cheryme.top/gtncdhszeb.html

JS:   [a, b] = [b, a];
来源：http://hz.ywan-chungtsiang.top/gtwpgyktbm.html

TS:   [a, b] = [b, a];
来源：http://hz.wangshuangyany.cn/gtpsusmrvc.html

Java: int t = a; a = b; b = t;
来源：http://hz.jinqigufen.top/gthwecvlst.html

Go:   a, b = b, a
来源：http://hz.fengsongda.top/gtmbcmwznk.html

Ruby: a, b = b, a
来源：http://hz.jyoumei.cn/gtgzteyvvi.html

C#:   (a, b) = (b, a);
来源：http://hz.jlsjyb.cn/gtgztzcnjv.html

[A20] 读取标准输入
来源：http://hz.gzhubu.top/gtbbyhkfaz.html

Py:   name = input("请输入：")
来源：http://hz.nanxuanxn.top/gtipziqkas.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.guowangkeji.top/gtetoyvxkl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.chenzaomai.com/gtcvnksych.html

TS:   // Node.js：readline 模块
来源：http://hz.zhijiandao.cn/gthtftjaly.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yuxming.cn/gtllhqutay.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.bjfxy.top/gtwdkyzqno.html

Ruby: gets.chomp
来源：http://hz.zhoulong.xyz/gtxpfwupxt.html

C#:   Console.ReadLine();
来源：http://hz.jqgfzy.top/gtxgfygnen.html

[A21] 保留指定小数位输出
来源：http://hz.hywenlv.cn/gtilaahkdb.html

Py:   f"{3.14159:.2f}"
来源：http://hz.9152youxi.cn/gtlhxdyozg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zycfv.cn/gtymrrfvxd.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ehwqpu.com/gtzaoimwio.html

TS:   (3.14159).toFixed(2)
来源：http://hz.tian-w.cn/gtkxuyxsuj.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.cheryme.top/gtdqcycatr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.yueranfly.top/gtmnpzctur.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.sysykeji.top/gtgnrebdvr.html

C#:   3.14159.ToString("F2")
来源：http://hz.yangfankeji.com/gtsxbytzma.html

[A22] 获取字符串长度
来源：http://hz.jinyuanbaomall.cn/gtoyleadrb.html

Py:   len(s)
来源：http://hz.xingfuxueyuan.xyz/gtipcjurao.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.0kj1m.cn/gtkfyroxqc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.gaohongyu789.top/gtpkfaonnb.html

TS:   s.length
来源：http://hz.hnxiangtu.top/gtleitwtcj.html

Java: s.length()
来源：http://hz.ybcxt.top/gtabrajmbd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yj20258888.top/gtdrobglit.html

Ruby: s.length
来源：http://hz.gzhubu.top/gtijfsfniv.html

C#:   s.Length
来源：http://hz.9152youxi.cn/gtqmxuvqsq.html

[A23] 大小写转换
来源：http://hz.fzhhl.top/gthoqlulfz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yj20258888.top/gtmgwxhmfi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.gotoacloud.top/gtdligfoui.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gaohongyu789.top/gtjpykcvdu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuxming.cn/gtayqphuvx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.vqdsnc.cn/gtvyohfvqn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yueranfly.top/gthxtzswxf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.snrcjt.cn/gtfvfawzoa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.hongshengwenyu.top/gtciacsetp.html

[A24] 去除首尾空白
来源：http://hz.xinyue.icu/gtnobpymwh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.pycfn.com/gtjvimccdg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hywenlv.cn/gtbwxttfbj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhaomingkeji.xyz/gtgkvdoaxu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhiwuduotai.top/gtknxbxalo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jinqigfzy.top/gttivubsni.html

Go:   strings.TrimSpace(s)
来源：http://hz.yueranfly.top/gtlzgveexe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.redwolf501.top/gtfxwehznq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cqqwz.cn/gtfvslvscu.html

[A25] 字符串比较
来源：http://hz.vqdsnc.cn/gtazezbynv.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhijiandao.cn/gtijgubwvq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.sweek.top/gtsrjhtvgi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sweek.top/gtirzsrjaf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.haohaochexian.top/gtjczqsxxq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.aizwys.cn/gtawsopysw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.mhx1999.top/gtshjerydk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yuanzhike.top/gtlfvavhsi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jqgfzy.top/gtzxlhciwq.html

[A26] 类型转换总览
来源：http://hz.sxryk.cn/gtymjqxrtr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jyoumei.cn/gtwzgrildx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yanxiufei.cn/gthihpdhnl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hfpthk.cn/gtborjowlu.html

TS:   Number() String() Boolean() x as number
来源：http://hz.wangshuangyany.cn/gtfiabinpb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hywenlv.cn/gtrxisjsfj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.redwolf501.top/gtdqrbessk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.pycfn.com/gtuozogjle.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.snrcjt.cn/gtsrzpwhhx.html

================================================================================
来源：http://hz.52xcode.cn/gtbdkdtbdj.html

B. 流程控制
来源：http://hz.yangfankeji.com/gtygsnumhl.html

================================================================================
来源：http://hz.guowangkeji.top/gteotyvstm.html

[B01] 条件判断 if / else
来源：http://hz.jianghu66.top/gtapjyfttj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ivvv.top/gtgfdaohza.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yonumen.top/gtpdbdtsii.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.meibo888.top/gtshbxfmer.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sufxvd.cn/gtvssiquzq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yangfankeji.com/gtvipobvlz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ybcxt.top/gtbltccxfw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.mhx1999.top/gtzoqaqvoo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xuanzx.com/gtsrsgtbml.html

[B02] 多分支 else if / elif
来源：http://hz.jinqigfzy.top/gtdzxkfemr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.sysykeji.top/gtwxciozgr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shuidangran.top/gtwpdrwukz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.fengsongda.top/gtppotczha.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtqjjejjec.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.aizwys.cn/gtjhzsmuxa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.nwbrower.top/gtdgvcnwvx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ydjk.org.cn/gtpqnwmwdm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtcjlqrkxp.html

[B03] switch / match / case
来源：http://hz.sxryk.cn/gtfnaiehkv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yueranfly.top/gtxmghbdmo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.tian-w.cn/gtueikynqf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xuanzx.com/gtdhndycgt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hammf.cn/gtiqtgbydn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.chenlongwang.top/gtasvasuiy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.quarkkingdee.top/gtzfnawtzi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jinqigufen.top/gtqznvqvgs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.sweek.top/gtdtjmmecg.html

[B04] for 计数循环
来源：http://hz.daria6918.cn/gtazhhlvbu.html

Py:   for i in range(10): print(i)
来源：http://hz.chenjidiqi.icu/gtilbddhzo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yj202588.top/gthdznqvur.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.tianlin.xyz/gtlupneezo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258888.top/gtqvfwvmfn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhengqikj.top/gtxscyedih.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xuetiantiany.cn/gtuibmiawu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yueranfly.top/gtyeiolzbm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yonumen.top/gtmzbqgvrx.html

[B05] 遍历数组 / 列表
来源：http://hz.nanxuanxn.top/gtomvvrmei.html

Py:   for item in arr: print(item)
来源：http://hz.shangyingyoupin.top/gtmeazqcwm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yonumen.top/gteslwmlso.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.cheryme.top/gtzqnomvps.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hfpthk.cn/gtoyutpdhm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhaomingkeji.xyz/gtitulmvlp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shangyingyoupin.top/gttatctchb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.kuanghao11.cn/gttzmmcsdm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.birdmap.top/gtejoaoakw.html

[B06] 遍历字典 / 对象
来源：http://hz.shzxlz.cn/gtilhucmek.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jinghuilouyu.cn/gthcrrgeqx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.birdmap.top/gtpwoxepbe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj20258888.top/gttvhepoul.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hongshengwenyu.top/gtruvbglas.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gogol.net.cn/gtpvrejohj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ywan-chungtsiang.top/gthqecfzqr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jyoumei.cn/gtbfhflcvf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.feifeiyinyue.top/gttgtuduja.html

[B07] while 循环
来源：http://hz.ivvv.top/gtzbhgbfmn.html

Py:   while i < 10: i += 1
来源：http://hz.havefunace.top/gtipztfodi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xylfe.cn/gtlrofahts.html

JS:   while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtoevioydu.html

TS:   while (i < 10) { i++; }
来源：http://hz.tian-w.cn/gtcumxieft.html

Java: while (i < 10) { i++; }
来源：http://hz.sysykeji.top/gtolztxpns.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.mhx1999.top/gtcwmovwzg.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yuanzhike.top/gtjdjjkybd.html

C#:   while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtvybzcrpw.html

[B08] do-while（至少执行一次）
来源：http://hz.ywan-chungtsiang.top/gtgqhkhzmy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ybcxt.top/gtihoicicl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jiagoushi.top/gtjaputttr.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gtgwvitcdy.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtzscjgtrc.html

Java: do { i++; } while (i < 10);
来源：http://hz.ydzc1.top/gtmleefdmz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.meibo888.top/gtgmxuunjt.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.vqdsnc.cn/gttlniwbej.html

C#:   do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtrmctrmdt.html

[B09] break 与 continue
来源：http://hz.zhoulong.xyz/gtllgretje.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shanyushiyangtech.top/gtljajrbnl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jqgfzy.top/gtxgonnqts.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.redwolf501.top/gtrcxwckmv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtidefbcwo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hfpthk.cn/gtgvxiwplq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.havefunace.top/gtqvnrryds.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yangfankeji.com/gtbiskezmg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtamfpapwq.html

[B10] 遍历同时拿索引
来源：http://hz.birdmap.top/gtlgaprcil.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cdnleiting.top/gtuqjjigqm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shuidangran.top/gtihjyydsg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gaohongyu789.top/gtfwnvsqlc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dianchejie.cn/gthvrzfrjf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hongshengwenyu.top/gtgaxntsfl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.aizwys.cn/gtxmbgipkg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenjidiqi.icu/gtyypousuu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.havefunace.top/gtghvpodek.html

[B11] 生成数字序列 / 区间
来源：http://hz.xingfuxueyuan.xyz/gtrtildrrj.html

Py:   list(range(0, 10, 2))
来源：http://hz.yvedp.cn/gtrqmfnrdq.html

PHP:  range(0, 10, 2);
来源：http://hz.zhengqikj.top/gtocvawsae.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hfpthk.cn/gtvvxxowfm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gtglgjeasn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ppjwa.cn/gtqbhrntnb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigufen.top/gtnoylvbug.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yuanzhike.top/gtvqhmsvol.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.fzhhl.top/gtgdookjva.html

[B12] 跳出多层循环
来源：http://hz.jinqigufen.top/gtfcsspztd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xuetiantiany.cn/gtqnzdczne.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hammf.cn/gtsgjrytvt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtanovntrm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fzhhl.top/gtklhsvvxt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtkckavkmp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinqigufen.top/gtdloiwpfx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.dianchejie.cn/gtgkowouyx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ybcxt.top/gtgwuhhpgl.html

[B13] 判断是否为数字
来源：http://hz.xziqi.cn/gtyxnbybyl.html

Py:   isinstance(x, (int, float))
来源：http://hz.havefunace.top/gtmfevpbxg.html

PHP:  is_numeric($x)
来源：http://hz.cucudq.cn/gtictygntc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.c1oappe.top/gtoyrutzoy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258888.top/gteotehwlc.html

Java: x instanceof Number
来源：http://hz.snrcjt.cn/gtuldrycjr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhixingplan.top/gtodfajaam.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhaomingkeji.xyz/gtqgsazkql.html

C#:   x is int or double or decimal
来源：http://hz.yanxiufei.cn/gtgjkttbpb.html

[B14] 判断值是否在集合内
来源：http://hz.hysaishi.cn/gtnmgnggpa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.guowangkeji.top/gtxevmjkkn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hongshengwenyu.top/gtveharaer.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtvfykzxjg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gzhubu.top/gthtzcfmtg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jlsjyb.cn/gtbsqhaflz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.daria6918.cn/gtwrnjhclz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.pycfn.com/gtwxyjruvo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gaohongyu789.top/gttqspykvb.html

[B15] 布尔运算与取反
来源：http://hz.jianghu66.top/gtyolgfyvb.html

Py:   a and b or not c
来源：http://hz.jiagoushi.top/gtgmlcpbuy.html

PHP:  $a && $b || !$c
来源：http://hz.gotoacloud.top/gtrllfslrb.html

JS:   a && b || !c
来源：http://hz.nanxuanxn.top/gtjbhdsxyl.html

TS:   a && b || !c
来源：http://hz.nanxinkj.top/gtxcsjyiam.html

Java: a && b || !c
来源：http://hz.xinyue.icu/gtdcqbfgfz.html

Go:   a && b || !c
来源：http://hz.xylfe.cn/gtaypqcubm.html

Ruby: a && b || !c
来源：http://hz.vqdsnc.cn/gtyzmdygtw.html

C#:   a && b || !c
来源：http://hz.yuxming.cn/gtjmtontlt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yuanzhike.top/gtuklzupep.html

Py:   if not data: return
来源：http://hz.aizwys.cn/gtmwqpstxx.html

PHP:  if (!$data) { return; }
来源：http://hz.hywenlv.cn/gtfhuqsyrs.html

JS:   if (!data) return;
来源：http://hz.ehwqpu.com/gtxbnfezkn.html

TS:   if (!data) return;
来源：http://hz.hywenlv.cn/gteryfkvob.html

Java: if (data == null) return;
来源：http://hz.cashguo.top/gtrftwfkzh.html

Go:   if data == nil { return }
来源：http://hz.redwolf501.top/gtsmvoftzp.html

Ruby: return if data.nil?
来源：http://hz.daxiang520.top/gtucxiycch.html

C#:   if (data == null) return;
来源：http://hz.zhiwuduotai.top/gttwxjyjdx.html

================================================================================
来源：http://hz.pycfn.com/gtkiertmyt.html

C. 函数与作用域
来源：http://hz.aizwys.cn/gtflknotmo.html

================================================================================
来源：http://hz.redwolf501.top/gtgezibuya.html

[C01] 定义函数
来源：http://hz.hysaishi.cn/gtzogyfhlp.html

Py:   def add(a, b): return a + b
来源：http://hz.jianghu66.top/gtuplezwvr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtxjdygwdm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yangfankeji.com/gtzxouhppt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtsmntghnt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtwlrilwgl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.wangdashe.top/gtsxlgkcme.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhaomingkeji.xyz/gtvqzgewwc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtzrisjlwz.html

[C02] 默认参数
来源：http://hz.guowangkeji.top/gtbuqarzcf.html

Py:   def greet(name="World"): return name
来源：http://hz.xingfuxueyuan.xyz/gtuhmobnwy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.kuanghao11.cn/gtdrkgnoec.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hywenlv.cn/gtsejtwlku.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.smart0.xyz/gtyrezrufq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.havefunace.top/gtfrfityvm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.birdmap.top/gtkuycfgql.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigufen.top/gtigctvpmc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhaomingkeji.xyz/gtkugohfpi.html

[C03] 可变参数
来源：http://hz.zhengqikj.top/gtwiepkifh.html

Py:   def total(*args): return sum(args)
来源：http://hz.yanxiufei.cn/gtngnxyene.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sxryk.cn/gtedubcnoc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tian-w.cn/gtddeamevr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shangyingyoupin.top/gtyogxumaq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.kuanghao11.cn/gthfkvnzhz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.andypj.xyz/gtvboyvhko.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zycfv.cn/gtytwknbil.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtedghathn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.52xcode.cn/gtwazotsgf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jyoumei.cn/gtzftaswho.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.meibo888.top/gtmzunqqna.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtyezjohnb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangtech.top/gtkeyfovnm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jianghu66.top/gtaqyqnool.html

Go:   // 无：用配置结构体参数
来源：http://hz.ybcxt.top/gtkepopnzc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtjtqfpwxu.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gtwjqibdpi.html

[C05] 返回多个值
来源：http://hz.xuanzx.com/gtgljsqwsd.html

Py:   return a, b
来源：http://hz.yj20258888.top/gtjuowomfz.html

PHP:  return [$a, $b];
来源：http://hz.shuidangran.top/gthofgciqx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.snrcjt.cn/gtnphljlcv.html

TS:   return { a, b };
来源：http://hz.ybcxt.top/gtfjwppwsw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenlongwang.top/gtqpoyprau.html

Go:   return a, b
来源：http://hz.jyoumei.cn/gtipdvgxco.html

Ruby: return a, b
来源：http://hz.cucudq.cn/gtkecttndg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigfzy.top/gtcvkjevqc.html

[C06] 匿名函数 / lambda
来源：http://hz.ppjwa.cn/gtlkdiupsn.html

Py:   square = lambda x: x * x
来源：http://hz.andypj.xyz/gttudtqiry.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yanxiufei.cn/gtaclqsmik.html

JS:   const square = x => x * x;
来源：http://hz.mhx1999.top/gtswwfyhit.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shanyushiyangtech.top/gtayeckvti.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sxryk.cn/gtqavzhsfq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuxming.cn/gtopvmdgdl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhijiandao.cn/gtyznfvhxz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.daria6918.cn/gtqmrigzaz.html

[C07] 把函数作为参数传入
来源：http://hz.smart0.xyz/gtpjsxxgvn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jyoumei.cn/gtplhowzmz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yonumen.top/gtchjixrze.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxuanxn.top/gtnqzudmex.html

TS:   arr.map(String)
来源：http://hz.wangdashe.top/gtglgexbwt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtzdxkkrrp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhaomingkeji.xyz/gtpsppohrq.html

Ruby: arr.map(&:upcase)
来源：http://hz.dashuyun.cn/gtloyywppj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hfpthk.cn/gtsoexbftb.html

[C08] 闭包
来源：http://hz.bjfxy.top/gtvpiimpac.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.chenjidiqi.icu/gtbztukosj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dianchejie.cn/gtbvbanpzq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gtasabsplu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtxybilgxs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxinkj.top/gtvjtuvvxv.html


<!-- 参考信息 -->