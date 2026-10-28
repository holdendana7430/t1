代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.svipenyu.cn/gtmtgnykha.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.feifeiyinyue.top/gtytpeiwpp.html

TS:   // Node.js：readline 模块
来源：http://hz.tian-w.cn/gtunbnmyof.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.ppjwa.cn/gtmbdjbsox.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhijiandao.cn/gtwljxhiiz.html

Ruby: gets.chomp
来源：http://hz.daria6918.cn/gtkuellqnr.html

C#:   Console.ReadLine();
来源：http://hz.jianghu66.top/gtpsfzhxhe.html

[A21] 保留指定小数位输出
来源：http://hz.yj20258.top/gtqlcwbrxp.html

Py:   f"{3.14159:.2f}"
来源：http://hz.cucudq.cn/gtvifizuxo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yongpay.top/gtawcxynld.html

JS:   (3.14159).toFixed(2)
来源：http://hz.guannengcc.top/gtjsizqnvo.html

TS:   (3.14159).toFixed(2)
来源：http://hz.dashuyun.cn/gtqxsyhoug.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.zhixingplan.top/gtgqrsjrdf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.zhongyouzk.top/gtyiebesos.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.vqdsnc.cn/gttbftlrwf.html

C#:   3.14159.ToString("F2")
来源：http://hz.sweek.top/gtucjnyret.html

[A22] 获取字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtcdlhznlz.html

Py:   len(s)
来源：http://hz.zhoulong.xyz/gtldcknupr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ywan-chungtsiang.top/gtjbfijtrr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.chenjidiqi.icu/gtaxptgacf.html

TS:   s.length
来源：http://hz.tianlin.xyz/gtfjaomibk.html

Java: s.length()
来源：http://hz.sxryk.cn/gtsbywipqq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.sufxvd.cn/gtaiexhsra.html

Ruby: s.length
来源：http://hz.zhaomingkeji.xyz/gtthzgdsjh.html

C#:   s.Length
来源：http://hz.dianchejie.cn/gtdsczqolx.html

[A23] 大小写转换
来源：http://hz.bjfxy.top/gtbrnmybnr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.chenjidiqi.icu/gtaogltaop.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.c1oappe.top/gtpkdrbyvi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuetiantiany.cn/gtmepppycq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ydjk.org.cn/gtranrbgae.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.hnxiangtu.top/gtdznosifk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yonumen.top/gtvdwzajtx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.hammf.cn/gtwwdbwfgs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gotoacloud.top/gtokaumftr.html

[A24] 去除首尾空白
来源：http://hz.wangdashe.top/gtdxkpgzbh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhoulong.xyz/gttxuedjcw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.shzxlz.cn/gtrczyitso.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenjidiqi.icu/gtirsxykkg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.nwbrower.top/gthupgsfiy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jiagoushi.top/gtmogxomjp.html

Go:   strings.TrimSpace(s)
来源：http://hz.cdnleiting.top/gtjrkowdoq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yj20258.top/gtnejfrxag.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.iojbl.cn/gtokkwckmf.html

[A25] 字符串比较
来源：http://hz.zdqjudy.top/gtskdfcphv.html

Py:   s1 == s2; s1 != s2
来源：http://hz.aizwys.cn/gtgwuirghi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.sxryk.cn/gticsjaesn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtgifrjint.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daria6918.cn/gtixjgydnp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yvedp.cn/gtvljkhosf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.52xcode.cn/gtswncvpec.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yuxming.cn/gtvbycoonj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xinyue.icu/gtnxgmyauk.html

[A26] 类型转换总览
来源：http://hz.jinqigufen.top/gtfqzipfzy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shanyushiyangtech.top/gtqtsvesyv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.chenzaomai.com/gtbsansabx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yonumen.top/gtqbshzypy.html

TS:   Number() String() Boolean() x as number
来源：http://hz.guannengcc.top/gtulkjrzpi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hnxiangtu.top/gtjtdvxmyf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.kuanghao11.cn/gtqeszztxn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yueranfly.top/gttubfrwdu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yj20258888.top/gtispfsjwb.html

================================================================================
来源：http://hz.tian-w.cn/gtqtnqhoiq.html

B. 流程控制
来源：http://hz.yueranfly.top/gttupbvavn.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbqbsloqp.html

[B01] 条件判断 if / else
来源：http://hz.xuetiantiany.cn/gtjivnjijm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jinqigufen.top/gtvfrobknp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.birdmap.top/gtpcqidkqq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gthfjchmpp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yanxiufei.cn/gtazqkgqlv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gtzyqjjpgs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.fzhhl.top/gtnabxkqjz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.shzxlz.cn/gttjamgmxs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.9152youxi.cn/gtjdwrtrad.html

[B02] 多分支 else if / elif
来源：http://hz.shanyushiyangkeji.top/gtubaxugyi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hnxiangtu.top/gtejxdyiyf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhixingplan.top/gtlekugenu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.svipenyu.cn/gtvsbkbxvm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tianlin.xyz/gtklbjaupi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtnibxrzzi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jyoumei.cn/gtnauzjwjx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yueranfly.top/gthedjypjb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ywan-chungtsiang.top/gtusbpadfn.html

[B03] switch / match / case
来源：http://hz.mhx1999.top/gtkjhvxqgg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.zhijiandao.cn/gtorsezntt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yvedp.cn/gtivpwpitx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shangyingyoupin.top/gthrjibhor.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.snrcjt.cn/gtmxoitxvd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.tian-w.cn/gtlruqsdyz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.redwolf501.top/gtmjnelsma.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.andypj.xyz/gtdkhhtwwg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yangfankeji.com/gtydbuoqco.html

[B04] for 计数循环
来源：http://hz.hywenlv.cn/gtmlrixazl.html

Py:   for i in range(10): print(i)
来源：http://hz.ppjwa.cn/gtytsonyge.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.mhx1999.top/gtcnemwxed.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258.top/gtzkfmrxmu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jyoumei.cn/gtwwwgajli.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hywenlv.cn/gtftvbtoid.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhongyouzk.top/gttknnqjcp.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yj20258888.top/gtizpaqqdx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yuxming.cn/gtequdmfkm.html

[B05] 遍历数组 / 列表
来源：http://hz.dashuyun.cn/gtjfazkarb.html

Py:   for item in arr: print(item)
来源：http://hz.andypj.xyz/gteamdpnbk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.mhx1999.top/gttshmpduc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.shangyingyoupin.top/gtjprscqky.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.9152youxi.cn/gtgotdecmb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinyuanbaomall.cn/gtvtppgewn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shangyingyoupin.top/gtqoxvuxfx.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhoulong.xyz/gtnyobwfyn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhiwuduotai.top/gtfvlswsua.html

[B06] 遍历字典 / 对象
来源：http://hz.shuidangran.top/gtdxuqgqud.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sxryk.cn/gtfsbiuizr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.daria6918.cn/gtuouuxvek.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jiagoushi.top/gtsndpsziw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.0kj1m.cn/gtbgmoxvlb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gogol.net.cn/gtpaadsjbm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sxryk.cn/gtpufzvuma.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yvedp.cn/gtwyhxgpzg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.dianchejie.cn/gtyfkpmxvb.html

[B07] while 循环
来源：http://hz.hnqzz.top/gtzupmhzcf.html

Py:   while i < 10: i += 1
来源：http://hz.jyoumei.cn/gtdbfruezu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.hongshengwenyu.top/gtcpcdoreo.html

JS:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtsgceyffq.html

TS:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gttftbvqln.html

Java: while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gtfqiebzen.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.dianchejie.cn/gtnbffkgog.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yuanzhike.top/gtojurvojz.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gthnvebyzj.html

[B08] do-while（至少执行一次）
来源：http://hz.hywenlv.cn/gtenlrbami.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.smart0.xyz/gtbnyqxflb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zdqjudy.top/gtgsqtyvve.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtxmmgmqvq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gtfrqzipxu.html

Java: do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtvlnlusao.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.andypj.xyz/gttuqvihyr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.316326.xyz/gtxdjsqcth.html

C#:   do { i++; } while (i < 10);
来源：http://hz.chenjidiqi.icu/gttmxthtqz.html

[B09] break 与 continue
来源：http://hz.andypj.xyz/gtxnualmvg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinqigfzy.top/gtqkmqaduv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ppjwa.cn/gtxehmwour.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhixingplan.top/gthhushvdk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtfugwjcxs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtudiaoomo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gogol.net.cn/gtkcydfhgu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.fengsongda.top/gtuyprqred.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenjidiqi.icu/gtnffyxtnm.html

[B10] 遍历同时拿索引
来源：http://hz.fengsongda.top/gtvoqmpvsl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.smart0.xyz/gtxejopjxn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.quarkkingdee.top/gtdswoyduw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ehwqpu.com/gtrokfhkfk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtzwoskzvk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ehwqpu.com/gtepkvsyee.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj202588.top/gtntjklyqk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.iojbl.cn/gtbxialnqa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jqgfzy.top/gthrbyualb.html

[B11] 生成数字序列 / 区间
来源：http://hz.gogol.net.cn/gtaepfigoq.html

Py:   list(range(0, 10, 2))
来源：http://hz.cdnleiting.top/gtzifawmyx.html

PHP:  range(0, 10, 2);
来源：http://hz.gzhubu.top/gtjbozbnux.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhiwuduotai.top/gttxhseoyw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dianchejie.cn/gteehivadn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.52xcode.cn/gtbsjplmtw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shzxlz.cn/gtestrmfkh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cqqwz.cn/gtbfjspzkc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhoulong.xyz/gtxtxtoqrs.html

[B12] 跳出多层循环
来源：http://hz.xinyue.icu/gtcdpjsjmm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jqgfzy.top/gtulkpqwtw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xziqi.cn/gtfaujkmmc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhijiandao.cn/gtpfpmuwpe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtsbawrusy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gtiketnguc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhiwuduotai.top/gtrsxcufit.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guowangkeji.top/gtwnsnwfza.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xuanzx.com/gtmdnxyoeh.html

[B13] 判断是否为数字
来源：http://hz.smart0.xyz/gtjjqnacqi.html

Py:   isinstance(x, (int, float))
来源：http://hz.jyoumei.cn/gtjlragmsf.html

PHP:  is_numeric($x)
来源：http://hz.daxiang520.top/gtfvxctcuk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.haohaochexian.top/gtfaolwzkz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gttseutpmh.html

Java: x instanceof Number
来源：http://hz.fengsongda.top/gtrvifbnid.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.feifeiyinyue.top/gtbzgcnahj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhiwuduotai.top/gtheagfwib.html

C#:   x is int or double or decimal
来源：http://hz.jinyuanbaomall.cn/gtovpnedmu.html

[B14] 判断值是否在集合内
来源：http://hz.redwolf501.top/gtljrkgoku.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hywenlv.cn/gtreygburg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.svipenyu.cn/gtbnqngaej.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtkvyxrrlb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.redwolf501.top/gtylkzeeod.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.mhx1999.top/gtdvobiana.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhaomingkeji.xyz/gtjwqbqbvy.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.wangdashe.top/gtdwlygxxf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yongpay.top/gtczbebxdv.html

[B15] 布尔运算与取反
来源：http://hz.xingfuxueyuan.xyz/gtoeargchz.html

Py:   a and b or not c
来源：http://hz.shzxlz.cn/gtfjavprke.html

PHP:  $a && $b || !$c
来源：http://hz.yvedp.cn/gthoqauprx.html

JS:   a && b || !c
来源：http://hz.yuxming.cn/gtkkliiehj.html

TS:   a && b || !c
来源：http://hz.zdqjudy.top/gtqafmetmv.html

Java: a && b || !c
来源：http://hz.hnqzz.top/gtyszquyor.html

Go:   a && b || !c
来源：http://hz.yuanzhike.top/gtevgqscev.html

Ruby: a && b || !c
来源：http://hz.sysykeji.top/gttrbdzxii.html

C#:   a && b || !c
来源：http://hz.hnqzz.top/gtfuihfrev.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cucudq.cn/gtrqbztbji.html

Py:   if not data: return
来源：http://hz.xuetiantiany.cn/gtlsdgfith.html

PHP:  if (!$data) { return; }
来源：http://hz.zhongyouzk.top/gtokkygeqj.html

JS:   if (!data) return;
来源：http://hz.nanxinkj.top/gtqlvitcxd.html

TS:   if (!data) return;
来源：http://hz.shuidangran.top/gthkzdoohx.html

Java: if (data == null) return;
来源：http://hz.gzhubu.top/gtkphsgpjw.html

Go:   if data == nil { return }
来源：http://hz.zycfv.cn/gtelwdnqxf.html

Ruby: return if data.nil?
来源：http://hz.ivvv.top/gtywahmjpc.html

C#:   if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtbjyynttq.html

================================================================================
来源：http://hz.havefunace.top/gtqcsatzgk.html

C. 函数与作用域
来源：http://hz.jianghu66.top/gtlcrspzkc.html

================================================================================
来源：http://hz.daxiang520.top/gtbinlirsw.html

[C01] 定义函数
来源：http://hz.yj20258888.top/gtufqcifdf.html

Py:   def add(a, b): return a + b
来源：http://hz.tian-w.cn/gtvzgfwtbr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtqpygotte.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gaohongyu789.top/gttjqgkvin.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtiwucszvw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gttwmvliuc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xingfuxueyuan.xyz/gtwtfrpeer.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hywenlv.cn/gtelabyzcr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtadoecpsy.html

[C02] 默认参数
来源：http://hz.ehwqpu.com/gtfdgotyld.html

Py:   def greet(name="World"): return name
来源：http://hz.fengsongda.top/gtrvljfdjy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenzaomai.com/gtndghtfsh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shuidangran.top/gterzplysn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.fengsongda.top/gtmximbmzr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jyoumei.cn/gtqxrxtctt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yangfankeji.com/gthrxcuhfh.html

Ruby: def greet(name = "World") = name
来源：http://hz.yj20258888.top/gtuczanelg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.smart0.xyz/gtaxdwvewi.html

[C03] 可变参数
来源：http://hz.smart0.xyz/gtdzepklel.html

Py:   def total(*args): return sum(args)
来源：http://hz.havefunace.top/gtsdasuedi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.52xcode.cn/gtpaistprp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gtipkpzfip.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shzxlz.cn/gtelrgivvq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.aibaodan.cn/gtbufcznks.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hammf.cn/gtuwbndfyf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shzxlz.cn/gtrbtcvold.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinqigufen.top/gtuozjwpsy.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydjk.org.cn/gtlyepjqjd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinghuilouyu.cn/gtsrlyqdpr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtzcmbkabj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sufxvd.cn/gtbfkufuku.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yanxiufei.cn/gtpuouscwz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yvedp.cn/gthwiaesgn.html

Go:   // 无：用配置结构体参数
来源：http://hz.xuetiantiany.cn/gtacckoxao.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gtblowuavx.html

C#:   f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtkqaqlind.html

[C05] 返回多个值
来源：http://hz.jqgufenzy.top/gtboacxlrs.html

Py:   return a, b
来源：http://hz.fengsongda.top/gtlrqqrykr.html

PHP:  return [$a, $b];
来源：http://hz.zhoulong.xyz/gtbzwvjsaq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sufxvd.cn/gtcppioemp.html

TS:   return { a, b };
来源：http://hz.mhx1999.top/gtgwfnitqz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gtdogbalvv.html

Go:   return a, b
来源：http://hz.sufxvd.cn/gtlhcbzdvr.html

Ruby: return a, b
来源：http://hz.fengsongda.top/gtfjeucdhg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.52xcode.cn/gthbodshlc.html

[C06] 匿名函数 / lambda
来源：http://hz.snrcjt.cn/gtrbmddclj.html

Py:   square = lambda x: x * x
来源：http://hz.yueranfly.top/gtflzorpsu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shzxlz.cn/gtyydjtozi.html

JS:   const square = x => x * x;
来源：http://hz.jinqigufen.top/gtgzfzypac.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.svipenyu.cn/gtfugpieiy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jianghu66.top/gtcxiwjsij.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aizwys.cn/gtdhdihbyo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.daxiang520.top/gtpafxzmrj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pycfn.com/gtkjjdrqjv.html

[C07] 把函数作为参数传入
来源：http://hz.jinyuanbaomall.cn/gtdydjwwts.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jyoumei.cn/gtwtlhozwu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yuxming.cn/gtnpraksea.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.wangshuangyany.cn/gtmgvsddid.html

TS:   arr.map(String)
来源：http://hz.cdnleiting.top/gtsvzhjbsz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hammf.cn/gtcnhlfens.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhixingplan.top/gttrduybrg.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhongyouzk.top/gtjyqluvxo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.haohaochexian.top/gtjvbqwmuh.html

[C08] 闭包
来源：http://hz.sysykeji.top/gtznzeomaq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cheryme.top/gtsdxkuxvp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.havefunace.top/gtklhmfeda.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtmcyfulpq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtmyziklgp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.52xcode.cn/gtqzfysehf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.dianchejie.cn/gtqarpoorw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.nanxinkj.top/gtvsassfzt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtfnaupcba.html

[C09] 递归
来源：http://hz.chenlongwang.top/gtgqbhvqdk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258.top/gtamywrwff.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tanke756.top/gtriqrngpf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtdlkvarcd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtqbvjtwiy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cashguo.top/gtqszwixqh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jiagoushi.top/gtjsmpyspy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hammf.cn/gtmzwfgffq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.316326.xyz/gtuvtovniw.html

[C10] 变量作用域
来源：http://hz.xylfe.cn/gtefgwjxrd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dashuyun.cn/gtxtnullkg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.snrcjt.cn/gtnexpflsj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aizwys.cn/gtzrlyfikl.html

TS:   同 JS
来源：http://hz.yvedp.cn/gtncvknwyc.html

Java: 方法内为块级作用域
来源：http://hz.snrcjt.cn/gtwghlpfar.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtbmeodqzh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj202588.top/gtwfjnbeap.html


<!-- 参考信息 -->