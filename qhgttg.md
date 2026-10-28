代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinqigfzy.top/gtajiwgpdx.html

Java: (int) 'A'; (char) 65
来源：http://hz.quarkkingdee.top/gtwcwiwidm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.shangyingyoupin.top/gtrldyxdyi.html

Ruby: "A".ord; 65.chr
来源：http://hz.mhx1999.top/gterojcozk.html

C#:   (int)'A'; (char)65
来源：http://hz.aibaodan.cn/gtcjhhahjz.html

[A19] 交换两个变量
来源：http://hz.zhongyouzk.top/gthcobgnsx.html

Py:   a, b = b, a
来源：http://hz.xylfe.cn/gtnzpfpprb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.c1oappe.top/gtmrfujhql.html

JS:   [a, b] = [b, a];
来源：http://hz.ydzc1.top/gtmagwdmld.html

TS:   [a, b] = [b, a];
来源：http://hz.hammf.cn/gtqeaohjac.html

Java: int t = a; a = b; b = t;
来源：http://hz.wangshuangyany.cn/gtrbtvyiba.html

Go:   a, b = b, a
来源：http://hz.bjfxy.top/gtrsamzjyx.html

Ruby: a, b = b, a
来源：http://hz.smart0.xyz/gtydmsmfyp.html

C#:   (a, b) = (b, a);
来源：http://hz.zycfv.cn/gtkgszcmzr.html

[A20] 读取标准输入
来源：http://hz.tanke756.top/gthyezaomy.html

Py:   name = input("请输入：")
来源：http://hz.ehwqpu.com/gtbxfhxbhu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.zhengqikj.top/gtibiqlnhj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zhoulong.xyz/gtvigkzhtx.html

TS:   // Node.js：readline 模块
来源：http://hz.sufxvd.cn/gttcrnwbme.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.hfpthk.cn/gtjljwgdhv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.haohaochexian.top/gtokwoxnzt.html

Ruby: gets.chomp
来源：http://hz.jiagoushi.top/gtiqmsuhhx.html

C#:   Console.ReadLine();
来源：http://hz.yuxming.cn/gtjsybewrv.html

[A21] 保留指定小数位输出
来源：http://hz.snrcjt.cn/gtoyziipff.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ivvv.top/gtegsyeblx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.wangshuangyany.cn/gtkgnkxgsr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.nanxuanxn.top/gttppithhi.html

TS:   (3.14159).toFixed(2)
来源：http://hz.shzxlz.cn/gtpbunyxep.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jiagoushi.top/gtnexxusub.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.52xcode.cn/gtaqmpoecr.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zhixingplan.top/gtouecjlrk.html

C#:   3.14159.ToString("F2")
来源：http://hz.svipenyu.cn/gtcsjxuyaa.html

[A22] 获取字符串长度
来源：http://hz.pycfn.com/gtbvylfueh.html

Py:   len(s)
来源：http://hz.xuetiantiany.cn/gttcaowome.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.gzhubu.top/gtpqkcrwxk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.hywenlv.cn/gtdyazoknq.html

TS:   s.length
来源：http://hz.vqdsnc.cn/gthhamctmc.html

Java: s.length()
来源：http://hz.hnqzz.top/gtkpqgqvil.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.sweek.top/gtyrvgoqio.html

Ruby: s.length
来源：http://hz.andypj.xyz/gtxekhoihz.html

C#:   s.Length
来源：http://hz.aibaodan.cn/gtbmpoymgz.html

[A23] 大小写转换
来源：http://hz.quarkkingdee.top/gtutfnllbm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jiagoushi.top/gtrwehxyjm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cdnleiting.top/gteyxgmrww.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.bjfxy.top/gtngzelqzn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cqqwz.cn/gtazexbysw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuanzhike.top/gtllpchyih.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yonumen.top/gtamkccyak.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.shanyushiyangtech.top/gtnejkxhxj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zhixingplan.top/gttgvtianf.html

[A24] 去除首尾空白
来源：http://hz.daria6918.cn/gtixtsqzon.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yueranfly.top/gtfpjqikbl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.dashuyun.cn/gtiiamowty.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.aizwys.cn/gtfvnqzrye.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangshuangyany.cn/gtjsleeahd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.316326.xyz/gtgluvhezf.html

Go:   strings.TrimSpace(s)
来源：http://hz.dianchejie.cn/gtdwhwwrnh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.daxiang520.top/gtftkbsrln.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cdnleiting.top/gtvvcwmbin.html

[A25] 字符串比较
来源：http://hz.ydjk.org.cn/gtyulsicwn.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cashguo.top/gtvzvntnkr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.kuanghao11.cn/gtmkeydtxh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.dianchejie.cn/gtmbetctyn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gogol.net.cn/gtsogskjid.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hongshengwenyu.top/gtekemvqyn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.daria6918.cn/gthscfqibo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hysaishi.cn/gtfzsqajpz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xylfe.cn/gthzmwdxno.html

[A26] 类型转换总览
来源：http://hz.smart0.xyz/gtusxrltlm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenlongwang.top/gtycrlavxj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xingfuxueyuan.xyz/gtxrzmserv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gaohongyu789.top/gtwsjezgmq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zdqjudy.top/gtkelmbetr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jianghu66.top/gtzzwfwbkh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.guannengcc.top/gtvckfwwwr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.tian-w.cn/gtpupwgtaz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yvedp.cn/gtinexiiyh.html

================================================================================
来源：http://hz.shuidangran.top/gtowojpbzz.html

B. 流程控制
来源：http://hz.pengpengdd.cyou/gtcqbjzahx.html

================================================================================
来源：http://hz.cucudq.cn/gtwqdxcfdg.html

[B01] 条件判断 if / else
来源：http://hz.ybcxt.top/gtwcpjfizh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.guowangkeji.top/gttyvqtnet.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.tian-w.cn/gtdxpkowef.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtivktvjep.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtwrjklqmr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.cashguo.top/gtayzkpiqb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ydjk.org.cn/gtzjcjeyrj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhaomingkeji.xyz/gtajujhluk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtorqpzxva.html

[B02] 多分支 else if / elif
来源：http://hz.guannengcc.top/gtogkbsxrs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.ivvv.top/gtlejerckh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.9152youxi.cn/gtgmqclyzm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gtdpccbakz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gtugtdgrxi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtzivyirzs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yj202588.top/gtixxncdnj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ywan-chungtsiang.top/gtertivtdf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sysykeji.top/gtzihqdple.html

[B03] switch / match / case
来源：http://hz.nanxinkj.top/gtwtcposxo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.fzhhl.top/gtgfvqvczu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.haohaochexian.top/gtevzwdqjo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenjidiqi.icu/gtwobnhbsz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.quarkkingdee.top/gtrmgqozhm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.aizwys.cn/gttasqvbki.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hfpthk.cn/gtzhsfbeqm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.mhx1999.top/gtlzjdsoau.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.pycfn.com/gthyolthre.html

[B04] for 计数循环
来源：http://hz.xuetiantiany.cn/gtjxbeahdu.html

Py:   for i in range(10): print(i)
来源：http://hz.shangyingyoupin.top/gtgmjydlmn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cdnleiting.top/gtshdhjiuf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nanxinkj.top/gteikitvgd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hysaishi.cn/gtwcdyvtab.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zdqjudy.top/gthqlmdrlx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yj20258888.top/gthfssbghb.html

Ruby: 10.times { |i| puts i }
来源：http://hz.pycfn.com/gtiintxhtu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.kuanghao11.cn/gtcventuia.html

[B05] 遍历数组 / 列表
来源：http://hz.sweek.top/gtvqynfdqm.html

Py:   for item in arr: print(item)
来源：http://hz.tianlin.xyz/gtsgtrwxkm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.tanke756.top/gththmjpgn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.haohaochexian.top/gtjlqiokjm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj202588.top/gtwgezlxkt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.guowangkeji.top/gtyorwuxpc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xingfuxueyuan.xyz/gtevxubsuq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shzxlz.cn/gtrydciexj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.tanke756.top/gtwkloucgs.html

[B06] 遍历字典 / 对象
来源：http://hz.hywenlv.cn/gtutrgwdjt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jinghuilouyu.cn/gtpdwjvyss.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hfpthk.cn/gtbpsgsofy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.chenlongwang.top/gtqcpngtso.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinghuilouyu.cn/gtixbybviv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.wangshuangyany.cn/gtnqkqzmjc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jianghu66.top/gtqrlzecra.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.9152youxi.cn/gtnbcsgvzy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.chenzaomai.com/gtkmkztxoq.html

[B07] while 循环
来源：http://hz.guowangkeji.top/gtxbkdafqd.html

Py:   while i < 10: i += 1
来源：http://hz.pengpengdd.cyou/gtjuofbzyv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yongpay.top/gtqeauttpe.html

JS:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtctpvxslk.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gteiqjtuzz.html

Java: while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtgtpachxa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.aizwys.cn/gthnljaoki.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gttnikgpih.html

C#:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtxhehuxbf.html

[B08] do-while（至少执行一次）
来源：http://hz.xylfe.cn/gtevaubblx.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.fengsongda.top/gtfrzhedzw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xinyue.icu/gtqmitxeqj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtjbvovben.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtztviswkd.html

Java: do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtmwaonzdf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gogol.net.cn/gtjadpqsbj.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.52xcode.cn/gtnimickog.html

C#:   do { i++; } while (i < 10);
来源：http://hz.pycfn.com/gtqycvxgbm.html

[B09] break 与 continue
来源：http://hz.jinqigfzy.top/gtiwffygku.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cucudq.cn/gtvijseszd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hfpthk.cn/gtwgvddhtp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtjebjhvgi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtmoqaotza.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtpkmyjcxu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jlsjyb.cn/gttvuoimrc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zycfv.cn/gtbagnurxd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtjoemtcml.html

[B10] 遍历同时拿索引
来源：http://hz.zhiwuduotai.top/gtbsqbzeht.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xuanzx.com/gtbbtszfaj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cucudq.cn/gtrozwtlor.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ppjwa.cn/gtxadjndii.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yj202588.top/gtnszklvmm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigfzy.top/gtqhvhdpnm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yongpay.top/gthyiwextk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cdnleiting.top/gtnkrtkvfc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yueranfly.top/gtxmiwnucp.html

[B11] 生成数字序列 / 区间
来源：http://hz.daria6918.cn/gtgfdzuksd.html

Py:   list(range(0, 10, 2))
来源：http://hz.quarkkingdee.top/gtdsaguuei.html

PHP:  range(0, 10, 2);
来源：http://hz.cheryme.top/gtrbhbmoar.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenzaomai.com/gtxlpaixhx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj202588.top/gtawlephdc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ybcxt.top/gtgvvenehu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.fzhhl.top/gtxdaebnvc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xuetiantiany.cn/gtsaottzhy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yangfankeji.com/gtxuduughm.html

[B12] 跳出多层循环
来源：http://hz.52xcode.cn/gtkyaooajm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.316326.xyz/gtpfhqpikk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guowangkeji.top/gtkzramsgo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj202588.top/gtwlgwhcgt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtqrcakvqj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtpudmydzn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shzxlz.cn/gtmunvbeqj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jqgufenzy.top/gtwkshqnoi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xingfuxueyuan.xyz/gtnmbfepbv.html

[B13] 判断是否为数字
来源：http://hz.guowangkeji.top/gtliwfyrea.html

Py:   isinstance(x, (int, float))
来源：http://hz.bjfxy.top/gtgjwrhldy.html

PHP:  is_numeric($x)
来源：http://hz.shanyushiyangtech.top/gtyjsxautr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ppjwa.cn/gtpabqrzae.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aizwys.cn/gtylvbpieb.html

Java: x instanceof Number
来源：http://hz.gotoacloud.top/gtplwftlld.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.bjfxy.top/gtjevhzrqr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.tian-w.cn/gtpqwxxiuf.html

C#:   x is int or double or decimal
来源：http://hz.zhongyouzk.top/gtsjqgwbjc.html

[B14] 判断值是否在集合内
来源：http://hz.hywenlv.cn/gtwzqgceie.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.aibaodan.cn/gtidskyfty.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cashguo.top/gtwcgedjxk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtuytbncho.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangtech.top/gtuogumvoe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guowangkeji.top/gtqvegpvki.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.vqdsnc.cn/gtiltphjoc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ywan-chungtsiang.top/gtcnpnfnwb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cheryme.top/gtmzmhyafa.html

[B15] 布尔运算与取反
来源：http://hz.ydzc1.top/gtzxrfdbjf.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtavurcdxh.html

PHP:  $a && $b || !$c
来源：http://hz.fengsongda.top/gtutzpkngp.html

JS:   a && b || !c
来源：http://hz.jinqigufen.top/gtpehlculc.html

TS:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtmonpoenk.html

Java: a && b || !c
来源：http://hz.yj202588.top/gttcsnmeox.html

Go:   a && b || !c
来源：http://hz.yangfankeji.com/gtzojurqmq.html

Ruby: a && b || !c
来源：http://hz.0kj1m.cn/gtiewknxic.html

C#:   a && b || !c
来源：http://hz.zhengqikj.top/gtngojqyia.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.c1oappe.top/gthnjecjai.html

Py:   if not data: return
来源：http://hz.yuanzhike.top/gtstgxseic.html

PHP:  if (!$data) { return; }
来源：http://hz.gaohongyu789.top/gtgdlisaks.html

JS:   if (!data) return;
来源：http://hz.zhengqikj.top/gtikmdrvou.html

TS:   if (!data) return;
来源：http://hz.zycfv.cn/gtszvbiajk.html

Java: if (data == null) return;
来源：http://hz.shzxlz.cn/gthrgqdvwc.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gtbzndfxer.html

Ruby: return if data.nil?
来源：http://hz.hnxiangtu.top/gtrtqzqvnm.html

C#:   if (data == null) return;
来源：http://hz.dianchejie.cn/gtpuhciwfx.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtnblxngnj.html

C. 函数与作用域
来源：http://hz.smart0.xyz/gtwqldkjqz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtvalgeyia.html

[C01] 定义函数
来源：http://hz.sxryk.cn/gthndallxa.html

Py:   def add(a, b): return a + b
来源：http://hz.fengsongda.top/gtzyrhrhto.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtfczazizc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hammf.cn/gtmadwbvxs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shzxlz.cn/gtcbfmgxtc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gthqzsnvbo.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258888.top/gtusgzbmjn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.mhx1999.top/gtbxeaxncl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ppjwa.cn/gtjwlclfbs.html

[C02] 默认参数
来源：http://hz.snrcjt.cn/gtyxtfrhwg.html

Py:   def greet(name="World"): return name
来源：http://hz.zhixingplan.top/gtpwlxlksw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenjidiqi.icu/gtuieicxfa.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtkjpkybtq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhoulong.xyz/gtcjvsvvvk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.52xcode.cn/gtosrxfsna.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.vqdsnc.cn/gtjsihqznm.html

Ruby: def greet(name = "World") = name
来源：http://hz.daria6918.cn/gtsoxmydld.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.feifeiyinyue.top/gtjfapnqbd.html

[C03] 可变参数
来源：http://hz.xuetiantiany.cn/gtlsndyibz.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenzaomai.com/gtrignrntk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.svipenyu.cn/gtyvmxohtu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhijiandao.cn/gtezugufmy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gtaezhxcsu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ehwqpu.com/gtwqvxnoku.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gzhubu.top/gtugzcjspj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jiagoushi.top/gtdpqdmtqx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.52xcode.cn/gteznpbctz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhongyouzk.top/gtdugsumwq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenzaomai.com/gtuuyyxvlh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jyoumei.cn/gtuzuwkote.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtwwszvwmx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gtdabyglxn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.andypj.xyz/gtlumrzojl.html

Go:   // 无：用配置结构体参数
来源：http://hz.xuetiantiany.cn/gthlqdcamo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cucudq.cn/gtsireuehk.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gtxuzpkbhd.html

[C05] 返回多个值
来源：http://hz.chenlongwang.top/gtwqjahdtl.html

Py:   return a, b
来源：http://hz.cqqwz.cn/gtybzxszog.html

PHP:  return [$a, $b];
来源：http://hz.sweek.top/gtuakfftbz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.meibo888.top/gtybgflrgn.html

TS:   return { a, b };
来源：http://hz.quarkkingdee.top/gtdpovbero.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gtmwiingnp.html

Go:   return a, b
来源：http://hz.andypj.xyz/gtlvoepigw.html

Ruby: return a, b
来源：http://hz.zhengqikj.top/gtsosksqqv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.aizwys.cn/gtkpsdjfqk.html

[C06] 匿名函数 / lambda
来源：http://hz.hywenlv.cn/gtoitvhoon.html

Py:   square = lambda x: x * x
来源：http://hz.xylfe.cn/gtitptjiah.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.0kj1m.cn/gtrzbhobfp.html

JS:   const square = x => x * x;
来源：http://hz.yvedp.cn/gtgojmflzb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hywenlv.cn/gtpbuxhprh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtakgzghgw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnqzz.top/gtfngxhyie.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangtech.top/gtspixkqsq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yanxiufei.cn/gtxxnryfew.html

[C07] 把函数作为参数传入
来源：http://hz.yonumen.top/gtihqnrqir.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.mhx1999.top/gtsazbjefv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yongpay.top/gtnhkzumst.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenjidiqi.icu/gtsixrlcbj.html

TS:   arr.map(String)
来源：http://hz.jinqigufen.top/gtcczljysu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sufxvd.cn/gthqwpjhgu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenlongwang.top/gtpafbzikt.html

Ruby: arr.map(&:upcase)
来源：http://hz.dashuyun.cn/gtqgckhzin.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhongyouzk.top/gtbpcaohku.html

[C08] 闭包
来源：http://hz.yanxiufei.cn/gtdxneaqvs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jlsjyb.cn/gtzsnpykwt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guowangkeji.top/gtgupanahs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtrfjqawqj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtsjzbxnxb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yonumen.top/gtkodeaaaf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258888.top/gtqegijazj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.vqdsnc.cn/gttmwnlrvq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtgchtdsyk.html

[C09] 递归
来源：http://hz.zhaomingkeji.xyz/gtvsyhihph.html


<!-- 参考信息 -->