代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xuetiantiany.cn/gtgpfzsdwc.html

PHP:  array_merge(...$nested);
来源：http://hz.feifeiyinyue.top/gtvtlinqrf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sysykeji.top/gtwqfpstlk.html

TS:   nested.flat();
来源：http://hz.sysykeji.top/gtroxmbjfe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258888.top/gtlvtxqavs.html

Go:   // 手写双层循环
来源：http://hz.quarkkingdee.top/gttgmrbpaz.html

Ruby: nested.flatten
来源：http://hz.yvedp.cn/gtecpyequs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dashuyun.cn/gtvsthtlav.html

[D19] 按字段分组
来源：http://hz.xylfe.cn/gtqlyibnsm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.kuanghao11.cn/gtydqmplil.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zdqjudy.top/gtrbydfdkp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgfzy.top/gtmcunsjdu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtbpdsbgqb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nanxuanxn.top/gtkjgaglgm.html

Go:   // 手写 map[string][]T
来源：http://hz.wangdashe.top/gtvxnbjvta.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.kuanghao11.cn/gtxgqozqph.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangtech.top/gtibtllfzl.html

[D20] 统计每个元素出现次数
来源：http://hz.yanxiufei.cn/gtgtenmkox.html

Py:   Counter(arr)
来源：http://hz.hnxiangtu.top/gtfgmtupdz.html

PHP:  array_count_values($arr);
来源：http://hz.zhixingplan.top/gtbidetmbs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.c1oappe.top/gtahqyrdkj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtrtjtuyzq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.fzhhl.top/gteshuppjb.html

Go:   // 手写 map[T]int
来源：http://hz.birdmap.top/gtylvlmqtp.html

Ruby: arr.tally
来源：http://hz.pengpengdd.cyou/gtnnureatl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cqqwz.cn/gtfuoecxqd.html

[D21] 判断是否包含某元素
来源：http://hz.cucudq.cn/gtwiekznio.html

Py:   x in arr
来源：http://hz.ivvv.top/gtngbulxzc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zdqjudy.top/gthxexfbwk.html

JS:   arr.includes(x)
来源：http://hz.sweek.top/gtgotxnyrw.html

TS:   arr.includes(x)
来源：http://hz.nanxinkj.top/gtxpfmpuly.html

Java: list.contains(x)
来源：http://hz.sweek.top/gtbuqxecuj.html

Go:   slices.Contains(arr, x)
来源：http://hz.cashguo.top/gtkphamqxi.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gtnlrxnwom.html

C#:   list.Contains(x)
来源：http://hz.ybcxt.top/gtxccuvlfs.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daria6918.cn/gtpqlhkavk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnqzz.top/gthtnujope.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cashguo.top/gtdmbzhkqs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.smart0.xyz/gthfudaokv.html

TS:   [...arr];
来源：http://hz.snrcjt.cn/gtivmrnrsi.html

Java: new ArrayList<>(list);
来源：http://hz.iojbl.cn/gtttsdrznd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jiagoushi.top/gtyxwahpin.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daria6918.cn/gtgqfsrphk.html

C#:   new List<int>(list);
来源：http://hz.jiagoushi.top/gtpcmlojrm.html

[D23] reduce 累积计算
来源：http://hz.nwbrower.top/gtnbguthmo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.kuanghao11.cn/gtptizesnb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jlsjyb.cn/gtgmbqvomd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtrlsbmnqm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtkziasnkr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yanxiufei.cn/gtgehupcah.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtydxtmdin.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.havefunace.top/gtvkhnqqyt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sxryk.cn/gtqdydikjn.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenzaomai.com/gteiqslkiz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.bjfxy.top/gtldkjovhz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhoulong.xyz/gtasuhxrlq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.vqdsnc.cn/gthdxbfjig.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.quarkkingdee.top/gtfcghiznr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xylfe.cn/gtnrgzgeus.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yanxiufei.cn/gtltzpemlo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.snrcjt.cn/gtbllazvvn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nanxinkj.top/gtfkeqbtjx.html

[D25] Set 集合去重与交并差
来源：http://hz.smart0.xyz/gtbnupyskf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yonumen.top/gtbnrttmqz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fengsongda.top/gtyfiiohue.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtoreqwjmz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jlsjyb.cn/gtymxaxgbn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhaomingkeji.xyz/gtmpycogvt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aizwys.cn/gtwtpadzne.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhiwuduotai.top/gtnjbesbwl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuanzx.com/gteaolugqw.html

[D26] 数组转字符串
来源：http://hz.sysykeji.top/gtkbigobmd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guannengcc.top/gtefscstyw.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtblnlqqew.html

JS:   arr.join(", ")
来源：http://hz.jianghu66.top/gtkthstxec.html

TS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gthxyocigp.html

Java: String.join(", ", list)
来源：http://hz.yonumen.top/gttqjyehlz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tanke756.top/gtcsllytwj.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtrexeddgb.html

C#:   string.Join(", ", list)
来源：http://hz.sxryk.cn/gtnekwzpkd.html

================================================================================
来源：http://hz.daria6918.cn/gtaatkzwlc.html

E. 字符串处理
来源：http://hz.cheryme.top/gtkqvtoywa.html

================================================================================
来源：http://hz.yueranfly.top/gtzazgxgef.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gtbcodoedv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.c1oappe.top/gtqpjsfxde.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.52xcode.cn/gtnhqsagqq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cdnleiting.top/gtdekboasu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtoubioqww.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ybcxt.top/gtrlkukymb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtpksxiwxo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuxming.cn/gtxzcupmpd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sufxvd.cn/gtfqfijnyi.html

[E02] 重复字符串
来源：http://hz.xylfe.cn/gtcrywdjdf.html

Py:   "ab" * 3
来源：http://hz.hysaishi.cn/gtuomhudkk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.52xcode.cn/gtzfbqmuwt.html

JS:   "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtdzucqnvk.html

TS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtdortnpcy.html

Java: "ab".repeat(3)
来源：http://hz.guannengcc.top/gtroumpyqx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sysykeji.top/gttiiuszco.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtkmdlcpao.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.0kj1m.cn/gtbozgirwj.html

[E03] 截取子串
来源：http://hz.xingfuxueyuan.xyz/gtyvpnupif.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yonumen.top/gtviwugkpk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daria6918.cn/gtjlaosuxx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtxskvmndv.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gtvldkygki.html

Java: s.substring(1, 4)
来源：http://hz.shuidangran.top/gtbgxospny.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhongyouzk.top/gtwvzcufnl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yanxiufei.cn/gttvljajlj.html

C#:   s.Substring(1, 3)
来源：http://hz.sxryk.cn/gttwzickeh.html

[E04] 查找子串位置
来源：http://hz.xingfuxueyuan.xyz/gtyshgpszh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shuidangran.top/gthhncbjrf.html

PHP:  strpos($s, "x");
来源：http://hz.chenzaomai.com/gtjjugbodw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.smart0.xyz/gtlvfbulcc.html

TS:   s.indexOf("x")
来源：http://hz.hnqzz.top/gtmnkwrjki.html

Java: s.indexOf("x")
来源：http://hz.snrcjt.cn/gtwsmqzaax.html

Go:   strings.Index(s, "x")
来源：http://hz.cdnleiting.top/gtepfxvqvn.html

Ruby: s.index("x")
来源：http://hz.wangshuangyany.cn/gtecmvthha.html

C#:   s.IndexOf("x")
来源：http://hz.wangshuangyany.cn/gtqavskzfv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.c1oappe.top/gtfuopzpax.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.aibaodan.cn/gtwexxpsyu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtrzfwrxif.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtqefxyjrm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhiwuduotai.top/gtbukxbxxi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtrpndejvk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.bjfxy.top/gtlgmwbrwc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.birdmap.top/gtzisxmhco.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cashguo.top/gtbavkqorz.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtbxqimiiv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuxming.cn/gtnrvlhuay.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.andypj.xyz/gtxvrjkzox.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtxrnoempr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtqszswhii.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtxhokkaps.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zycfv.cn/gtxxwuipqv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ppjwa.cn/gtueypesbh.html

C#:   s.Replace("a", "b")
来源：http://hz.gotoacloud.top/gtikwhzbey.html

[E07] 按分隔符拆分
来源：http://hz.redwolf501.top/gtgzcqdulj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ivvv.top/gtqxfqfdpc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jyoumei.cn/gtczfawnht.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydjk.org.cn/gtvikhmsgv.html

TS:   s.split(",")
来源：http://hz.yuxming.cn/gtrygcasre.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sweek.top/gtfcgojzwm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sweek.top/gtagjnzyzx.html

Ruby: s.split(",");  s.split
来源：http://hz.sxryk.cn/gtolfxmwgr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yuxming.cn/gtzywngqbn.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtbsnsiacp.html

Py:   ",".join(items)
来源：http://hz.cqqwz.cn/gtdsxvsfwj.html

PHP:  implode(",", $items);
来源：http://hz.hongshengwenyu.top/gtfnqeapcw.html

JS:   items.join(",")
来源：http://hz.redwolf501.top/gtjuzbpruz.html

TS:   items.join(",")
来源：http://hz.birdmap.top/gttomprhmg.html

Java: String.join(",", items)
来源：http://hz.smart0.xyz/gtpytsgjkx.html

Go:   strings.Join(items, ",")
来源：http://hz.aibaodan.cn/gtjtrdtvtj.html

Ruby: items.join(",")
来源：http://hz.yangfankeji.com/gtsxbfqubd.html

C#:   string.Join(",", items)
来源：http://hz.guannengcc.top/gtfzbghdfj.html

[E09] 去除所有空白字符
来源：http://hz.yj20258.top/gtakbsgxqk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hongshengwenyu.top/gtbxrwcwvz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenjidiqi.icu/gtleksebsb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtmdaunyne.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ywan-chungtsiang.top/gtotdneuef.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jiagoushi.top/gtmrlxulhu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.meibo888.top/gtpuedmxxd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydzc1.top/gtofcoytaq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aizwys.cn/gtkqkroqib.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgufenzy.top/gtzfontyus.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sysykeji.top/gtficefudr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtpsqmvmov.html

JS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtkqvoxsht.html

TS:   "7".padStart(3, "0")
来源：http://hz.tian-w.cn/gtdicpawhh.html

Java: String.format("%03d", 7)
来源：http://hz.gzhubu.top/gttdhhpdan.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhongyouzk.top/gtizmcydam.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.0kj1m.cn/gtuytawakj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.smart0.xyz/gtrptzfzom.html

[E11] 反转字符串
来源：http://hz.shzxlz.cn/gteluipsjo.html

Py:   s[::-1]
来源：http://hz.c1oappe.top/gtwgthqbos.html

PHP:  strrev($s);
来源：http://hz.yanxiufei.cn/gtfgyzcnuz.html

JS:   [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtmfidmunw.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtympxsuep.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jyoumei.cn/gtnxchbhjx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guannengcc.top/gtaysfnwil.html

Ruby: s.reverse
来源：http://hz.nanxinkj.top/gtgfufcuzz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gthgazwcah.html

[E12] 统计某字符出现次数
来源：http://hz.zhiwuduotai.top/gtdeatuukm.html

Py:   s.count("a")
来源：http://hz.zycfv.cn/gtjwpxpqie.html

PHP:  substr_count($s, "a");
来源：http://hz.hnqzz.top/gttzbuesxw.html

JS:   s.split("a").length - 1
来源：http://hz.kuanghao11.cn/gtmwfsfwcn.html

TS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtseugxsvm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gtzftabssk.html

Go:   strings.Count(s, "a")
来源：http://hz.ppjwa.cn/gtqlhckbni.html

Ruby: s.count("a")
来源：http://hz.nwbrower.top/gtecvajclj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yanxiufei.cn/gtdctxkupo.html

[E13] 逐字符遍历
来源：http://hz.havefunace.top/gtcdlsbvzb.html

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtqkrotexd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aibaodan.cn/gtdcqhkddt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtdzrduwwl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtmoslcmpp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhiwuduotai.top/gtphxlmloq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhixingplan.top/gthaxhmsnv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jlsjyb.cn/gtxbtycvvh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.birdmap.top/gtfvvkgptx.html

[E14] URL 编码与 Base64
来源：http://hz.ydzc1.top/gtyurixghq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuetiantiany.cn/gtlatuyajo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtqupqgsso.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.andypj.xyz/gtcnlphmme.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aizwys.cn/gtltrojozz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zdqjudy.top/gtsefrnyxt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gttyyjlsfa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yonumen.top/gtwhqpytnr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenjidiqi.icu/gtuursdqem.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenjidiqi.icu/gtixwzglrb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydzc1.top/gtloosuoil.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinghuilouyu.cn/gtfbdgodia.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hysaishi.cn/gtfjkamoqn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.52xcode.cn/gtjezwtpvp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangshuangyany.cn/gtgxpvuwmg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangshuangyany.cn/gtlytsdhvz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ivvv.top/gtlgybojjh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shangyingyoupin.top/gtiiiiefpk.html

[E16] 数字千分位
来源：http://hz.zhiwuduotai.top/gtxpmwsyoy.html

Py:   f"{1234567:,}"
来源：http://hz.guowangkeji.top/gtixsjpaci.html

PHP:  number_format(1234567);
来源：http://hz.hywenlv.cn/gtisswvniw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtrbdtiupv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtcznjpugb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangshuangyany.cn/gtlwaxlpmw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.aibaodan.cn/gtdxdwblve.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhongyouzk.top/gtnqxxbgnb.html

C#:   1234567.ToString("N0")
来源：http://hz.sysykeji.top/gtcqqmiabn.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gthedudoal.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gtcjccrrqu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xinyue.icu/gtuaimxmbq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtgcpismzj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtgobhlsdl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cqqwz.cn/gtxwfongdr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fengsongda.top/gtsqxzwyqi.html

Ruby: s.capitalize
来源：http://hz.xinyue.icu/gtxldvsmls.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ybcxt.top/gtfdsmfzpg.html

[E18] 模板占位符替换
来源：http://hz.cheryme.top/gtjtbofgft.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shzxlz.cn/gttyzovnry.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtsoyzcatb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtdxagdfqo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtihohjdfq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtbpfafznm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.svipenyu.cn/gtspkqbgol.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.redwolf501.top/gtadvvtgxj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.0kj1m.cn/gtqtopjdlo.html

[E19] 多行文本按行拆分
来源：http://hz.iojbl.cn/gtnxaaddhl.html

Py:   s.splitlines()
来源：http://hz.yj202588.top/gtvthhlbgo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhongyouzk.top/gtxilygdke.html

JS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtppqonbqy.html

TS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gtvqrsjdhs.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtgazigbrq.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtynujptfo.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gtktcbxkfl.html

C#:   s.Split('\n')
来源：http://hz.jlsjyb.cn/gtuolrrmot.html

[E20] 判断字符串是否为空
来源：http://hz.svipenyu.cn/gttttgbzuv.html

Py:   if not s:
来源：http://hz.hammf.cn/gtzqlshcko.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shangyingyoupin.top/gtaxlauzoa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydzc1.top/gtwzxndeuj.html

TS:   if (s === "") {}
来源：http://hz.sxryk.cn/gtintogkim.html

Java: if (s.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtgzttmfzu.html

Go:   if s == "" {}
来源：http://hz.feifeiyinyue.top/gtqsgmetvw.html

Ruby: if s.empty?
来源：http://hz.zhijiandao.cn/gttbfotyxz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hysaishi.cn/gtkahcyuyq.html

[E21] 超长截断加省略号
来源：http://hz.bjfxy.top/gtwljyyzjo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhongyouzk.top/gtdjutcjlj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hnxiangtu.top/gtvgccwiug.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtbblcvdnr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtlasssvsh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtdrwyekio.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gogol.net.cn/gtqkkawchr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ehwqpu.com/gtejddiwhk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yueranfly.top/gtrevwywdn.html

[E22] 字节长度与字符长度
来源：http://hz.c1oappe.top/gtbhnzigms.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jyoumei.cn/gtkynzniyq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuanzx.com/gtxlvppnzh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtxwnbwnob.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtehgmcdjx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xinyue.icu/gtgovjtctk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sysykeji.top/gtjegvrqcz.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtbmvtkrzs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgfzy.top/gtrzeblnan.html

================================================================================
来源：http://hz.zhijiandao.cn/gtieaxiqdq.html

F. 文件与目录
来源：http://hz.iojbl.cn/gtoyldjgnv.html

================================================================================
来源：http://hz.kuanghao11.cn/gthgfkjani.html

[F01] 读取整个文件
来源：http://hz.zycfv.cn/gtkojxgvth.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yanxiufei.cn/gtcivcugre.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gtcmvkkpqx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.haohaochexian.top/gtdfatdwua.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yonumen.top/gtkqlcttrz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtbkkxzotz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtthimpwka.html

Ruby: File.read("a.txt")
来源：http://hz.zdqjudy.top/gtifyxgcjd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.bjfxy.top/gtjpqgeakn.html

[F02] 逐行读取文件
来源：http://hz.snrcjt.cn/gtjqdpvpui.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.birdmap.top/gtbzjyfezv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jlsjyb.cn/gtydeqhuao.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.quarkkingdee.top/gtnopuhsqf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtzsutvpeo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtqxmxfvjc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daria6918.cn/gtpiroubwc.html


<!-- 参考信息 -->