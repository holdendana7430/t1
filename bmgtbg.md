代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydzc1.top/gtbxkvfeab.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gttnzvarda.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.birdmap.top/gtdwkblbwi.html

Go:   // 手写循环累加
来源：http://hz.guowangkeji.top/gtuipvmmua.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.quarkkingdee.top/gtchxsfjaw.html

C#:   list.Sum();  list.Average()
来源：http://hz.cashguo.top/gtngsetaml.html

[D17] 最大值与最小值
来源：http://hz.zhiwuduotai.top/gtiieeiucw.html

Py:   max(arr);  min(arr)
来源：http://hz.wangshuangyany.cn/gtbntrzgur.html

PHP:  max($arr);  min($arr);
来源：http://hz.gogol.net.cn/gturnzfiun.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxuanxn.top/gteowslnlz.html

TS:   Math.max(...arr);
来源：http://hz.cashguo.top/gthlotcoxi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shuidangran.top/gtpjwakwuo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhengqikj.top/gtpozokoue.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtpvxgqhxo.html

C#:   list.Max();  list.Min()
来源：http://hz.xingfuxueyuan.xyz/gttsljymfl.html

[D18] 扁平化嵌套数组
来源：http://hz.tanke756.top/gtumwkcmbh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yongpay.top/gtarzgvlwv.html

PHP:  array_merge(...$nested);
来源：http://hz.zhixingplan.top/gtoamhctjl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.feifeiyinyue.top/gtphmgcfqy.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gtnytgvoik.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.0kj1m.cn/gttbwwefnl.html

Go:   // 手写双层循环
来源：http://hz.sweek.top/gteadrtpju.html

Ruby: nested.flatten
来源：http://hz.dashuyun.cn/gtdkvfrwkk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtdlpjbqpo.html

[D19] 按字段分组
来源：http://hz.xingfuxueyuan.xyz/gtfqlfuuqq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sysykeji.top/gttqwgthco.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sysykeji.top/gtqegwpmqu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.c1oappe.top/gtyyvemypg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zycfv.cn/gttntpjuvw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhixingplan.top/gtnmcquffz.html

Go:   // 手写 map[string][]T
来源：http://hz.dianchejie.cn/gtgmelfhst.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtpptjwihu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.smart0.xyz/gtcqqiwbxr.html

[D20] 统计每个元素出现次数
来源：http://hz.mhx1999.top/gtcqgobndi.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangtech.top/gtjskbqcbl.html

PHP:  array_count_values($arr);
来源：http://hz.cashguo.top/gtpaxrufve.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tanke756.top/gtgrerhhgl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtrvnyopnt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gtyclueoxa.html

Go:   // 手写 map[T]int
来源：http://hz.cashguo.top/gtlvswugpc.html

Ruby: arr.tally
来源：http://hz.wangshuangyany.cn/gtdjhrpujr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gzhubu.top/gtivkunicp.html

[D21] 判断是否包含某元素
来源：http://hz.birdmap.top/gtsztibqfs.html

Py:   x in arr
来源：http://hz.cqqwz.cn/gtugzkybsw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jiagoushi.top/gtyzqivlzs.html

JS:   arr.includes(x)
来源：http://hz.wangshuangyany.cn/gttfgxpnfc.html

TS:   arr.includes(x)
来源：http://hz.yueranfly.top/gtmwuefofi.html

Java: list.contains(x)
来源：http://hz.yj202588.top/gtwgbrwryh.html

Go:   slices.Contains(arr, x)
来源：http://hz.gotoacloud.top/gtsoxdlygb.html

Ruby: arr.include?(x)
来源：http://hz.feifeiyinyue.top/gtccxwolmg.html

C#:   list.Contains(x)
来源：http://hz.jiagoushi.top/gtooaqsaux.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinghuilouyu.cn/gtaxipbikf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jianghu66.top/gtunobzqmz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenlongwang.top/gtbxkbrbsx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xuanzx.com/gtgcntwftt.html

TS:   [...arr];
来源：http://hz.iojbl.cn/gtysyifrkh.html

Java: new ArrayList<>(list);
来源：http://hz.zhaomingkeji.xyz/gtujjmtmwg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.haohaochexian.top/gtwvybhnem.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258.top/gtvgpkcpjs.html

C#:   new List<int>(list);
来源：http://hz.nanxuanxn.top/gtieqhdree.html

[D23] reduce 累积计算
来源：http://hz.zhixingplan.top/gtgokjqzut.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuetiantiany.cn/gtqqhjdfla.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydzc1.top/gtyvtswptm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtxjfskijq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258.top/gthmjbjols.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtsdqcgrqh.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtxivvvpmu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangkeji.top/gtmxgmuflb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gzhubu.top/gtthidauly.html

[D24] 字典 / Map 基本操作
来源：http://hz.nwbrower.top/gtpldkycod.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenjidiqi.icu/gthhcrrvoz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtndlnwngc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydzc1.top/gtnhczksfb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xylfe.cn/gtlaotbqxb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guowangkeji.top/gtfnstpznk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.snrcjt.cn/gtntscoqkp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.redwolf501.top/gtuplkcrhb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.snrcjt.cn/gtjbffaxef.html

[D25] Set 集合去重与交并差
来源：http://hz.nwbrower.top/gtsmzbngui.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cqqwz.cn/gtwvojvjml.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xinyue.icu/gtadrnqtmk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jianghu66.top/gtcgjeilch.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hnxiangtu.top/gtbqivzbxu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtjqoqwqzu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.iojbl.cn/gtohtfufwh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtvuodifld.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pengpengdd.cyou/gtbbimotnk.html

[D26] 数组转字符串
来源：http://hz.jiagoushi.top/gtkyosqnwo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.daxiang520.top/gtidtiydmu.html

PHP:  implode(", ", $arr);
来源：http://hz.wangdashe.top/gtdnhozeav.html

JS:   arr.join(", ")
来源：http://hz.xuetiantiany.cn/gtxsaguiqf.html

TS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtiplfkbsi.html

Java: String.join(", ", list)
来源：http://hz.sxryk.cn/gtxrgxqcdm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.meibo888.top/gtmnmntfse.html

Ruby: arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtuyllfngq.html

C#:   string.Join(", ", list)
来源：http://hz.ydjk.org.cn/gtjbyvxjwr.html

================================================================================
来源：http://hz.cucudq.cn/gtxveoknof.html

E. 字符串处理
来源：http://hz.ehwqpu.com/gtcaneyupv.html

================================================================================
来源：http://hz.hfpthk.cn/gtglzjfpvz.html

[E01] 拼接字符串
来源：http://hz.yanxiufei.cn/gtlpgfqmlt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigfzy.top/gtmctbqwyu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.redwolf501.top/gtpygtbrav.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhijiandao.cn/gtgbpywvic.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.havefunace.top/gtudraknur.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj202588.top/gtxlcaujrj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.bjfxy.top/gtuhowaixj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnqzz.top/gtajnbohww.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cqqwz.cn/gtkvmafjfp.html

[E02] 重复字符串
来源：http://hz.jinqigfzy.top/gtsdxmrazy.html

Py:   "ab" * 3
来源：http://hz.yonumen.top/gtmccwppon.html

PHP:  str_repeat("ab", 3);
来源：http://hz.c1oappe.top/gtjukagfdd.html

JS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtzgglofjy.html

TS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gtrfunulgl.html

Java: "ab".repeat(3)
来源：http://hz.havefunace.top/gtxcclgwhr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ybcxt.top/gtgokkhppz.html

Ruby: "ab" * 3
来源：http://hz.hfpthk.cn/gtjktjvstq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj202588.top/gtuggzarye.html

[E03] 截取子串
来源：http://hz.yangfankeji.com/gtokdpnjkz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.dianchejie.cn/gttlkgytva.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tian-w.cn/gtsxesjvli.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtoygkkstz.html

TS:   s.slice(1, 4)
来源：http://hz.nwbrower.top/gtvgovlgeq.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtjwrtujyj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuanzx.com/gtfpqrozaw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shangyingyoupin.top/gtesvmfrcr.html

C#:   s.Substring(1, 3)
来源：http://hz.yongpay.top/gtldazgsgo.html

[E04] 查找子串位置
来源：http://hz.quarkkingdee.top/gthbztcqqt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.pycfn.com/gtoaegqvrq.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtpkjvciwn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.havefunace.top/gtdgckvhcc.html

TS:   s.indexOf("x")
来源：http://hz.yongpay.top/gtiyzahumr.html

Java: s.indexOf("x")
来源：http://hz.smart0.xyz/gttxuphwhb.html

Go:   strings.Index(s, "x")
来源：http://hz.yongpay.top/gtejohqwji.html

Ruby: s.index("x")
来源：http://hz.9152youxi.cn/gtbjyxhuct.html

C#:   s.IndexOf("x")
来源：http://hz.ppjwa.cn/gtvhpleujb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dashuyun.cn/gtgpjxpkby.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenjidiqi.icu/gtpvwkwwvx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigufen.top/gtofzdiuoq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtdudtkrhd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zycfv.cn/gtzarsshnw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtnczdkqkp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenlongwang.top/gticuqynuv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hnxiangtu.top/gtydnawxhf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fzhhl.top/gtjlidbhpc.html

[E06] 替换子串
来源：http://hz.hfpthk.cn/gtxgwunzsd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yongpay.top/gtjkfoadxh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinyuanbaomall.cn/gtlebbxsmw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtidkmznvv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtpozebthg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtwpgzxutl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tanke756.top/gthopvkepj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aibaodan.cn/gtmabkosbi.html

C#:   s.Replace("a", "b")
来源：http://hz.cdnleiting.top/gtyceiovoz.html

[E07] 按分隔符拆分
来源：http://hz.meibo888.top/gtczunulvg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cheryme.top/gtopqyaydb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jlsjyb.cn/gteyjmmncj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.wangshuangyany.cn/gttggomixc.html

TS:   s.split(",")
来源：http://hz.cheryme.top/gtlskkketv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.kuanghao11.cn/gtrpdpyeds.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj202588.top/gtffggzoym.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangtech.top/gtgscydpuk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yueranfly.top/gtsaknpwig.html

[E08] 数组按分隔符合并
来源：http://hz.jianghu66.top/gtrxlzwalk.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangkeji.top/gtovaumiav.html

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gtevcffkxq.html

JS:   items.join(",")
来源：http://hz.dianchejie.cn/gtgqombpqb.html

TS:   items.join(",")
来源：http://hz.yj20258888.top/gtvriqhezw.html

Java: String.join(",", items)
来源：http://hz.fengsongda.top/gtybkrxgot.html

Go:   strings.Join(items, ",")
来源：http://hz.jinyuanbaomall.cn/gttkspsbbx.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtizcpgtqj.html

C#:   string.Join(",", items)
来源：http://hz.hysaishi.cn/gtnewqlpdk.html

[E09] 去除所有空白字符
来源：http://hz.xylfe.cn/gtsnqnnpau.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gtqdfffmug.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgufenzy.top/gtvrzkhiul.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtljeibogm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtpolasaei.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtkzkrknbo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hfpthk.cn/gtielygsbx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.pycfn.com/gtsdhvroll.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shzxlz.cn/gtsuqdgqzr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.c1oappe.top/gtmukeuhvz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shangyingyoupin.top/gtxvadbooj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yangfankeji.com/gtoftbmhzk.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtsmhdayou.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtxkyrayor.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtithpkcum.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zycfv.cn/gtaajyqffy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cqqwz.cn/gtezgdyqhb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yangfankeji.com/gtjnwnqead.html

[E11] 反转字符串
来源：http://hz.gotoacloud.top/gtepjpmjas.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtnxbcktcz.html

PHP:  strrev($s);
来源：http://hz.daxiang520.top/gtrrbvzggb.html

JS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtrhlvfhgi.html

TS:   [...s].reverse().join("")
来源：http://hz.birdmap.top/gtdfuzfcle.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.quarkkingdee.top/gtiwgqepqc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258888.top/gtptgmqecm.html

Ruby: s.reverse
来源：http://hz.yonumen.top/gtobxvfrxi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtkucyqhao.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gthhkfzjhg.html

Py:   s.count("a")
来源：http://hz.zhengqikj.top/gtacuwvviw.html

PHP:  substr_count($s, "a");
来源：http://hz.tian-w.cn/gtumpjcozc.html

JS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtbbavwapi.html

TS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtescosksm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ybcxt.top/gtnhacfbfi.html

Go:   strings.Count(s, "a")
来源：http://hz.zhoulong.xyz/gtbctjghqt.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangtech.top/gtslsgznan.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xziqi.cn/gtwtnqaspn.html

[E13] 逐字符遍历
来源：http://hz.yanxiufei.cn/gttjncabqt.html

Py:   for ch in s: print(ch)
来源：http://hz.cheryme.top/gtizuaaxzu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jiagoushi.top/gtybclibop.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtjxurakmg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtcbilzedw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tianlin.xyz/gtyykfvtyz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhengqikj.top/gtnmwzecnc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinyuanbaomall.cn/gttfqzkcaw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.andypj.xyz/gttlcaoyrb.html

[E14] URL 编码与 Base64
来源：http://hz.xingfuxueyuan.xyz/gtyrwqwqjw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258888.top/gtgafyzlwd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.pycfn.com/gttxtnxhco.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangshuangyany.cn/gtnjvxridf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenlongwang.top/gtigufizln.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aizwys.cn/gtryxrlefw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tian-w.cn/gthbdtyjtf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinqigufen.top/gtsxsfwjlq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuanzhike.top/gtuhjqhucs.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenlongwang.top/gtynnerdby.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yanxiufei.cn/gtzfjejhqr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shangyingyoupin.top/gtijtamsgn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hysaishi.cn/gtmedkukpu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xinyue.icu/gtwjlreffe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gtompsismg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hywenlv.cn/gtntaqsoel.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cqqwz.cn/gtcktnvpum.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shuidangran.top/gtrrwvikgt.html

[E16] 数字千分位
来源：http://hz.chenlongwang.top/gtvqfkhthi.html

Py:   f"{1234567:,}"
来源：http://hz.iojbl.cn/gtjfofghpj.html

PHP:  number_format(1234567);
来源：http://hz.jinyuanbaomall.cn/gtbujbdcbm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtcqarknlk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtilbdgyyu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shzxlz.cn/gtrbfnjzlo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.mhx1999.top/gtnebraswy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.iojbl.cn/gtlrosfplm.html

C#:   1234567.ToString("N0")
来源：http://hz.iojbl.cn/gtldadwvou.html

[E17] 首字母大写
来源：http://hz.ydjk.org.cn/gtbwaualql.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258.top/gtdavldunu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhongyouzk.top/gtmcowkvdj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtzynhjcca.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtkesdiigj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinqigfzy.top/gtpfndaxyu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hongshengwenyu.top/gthcizwumj.html

Ruby: s.capitalize
来源：http://hz.xuanzx.com/gtjjywihkr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuetiantiany.cn/gtfrhzcixy.html

[E18] 模板占位符替换
来源：http://hz.guowangkeji.top/gtgfbtptzf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gotoacloud.top/gtxwirmpsk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhengqikj.top/gtbeolaneh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhixingplan.top/gtngbyenpq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtuzerrqnt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.iojbl.cn/gttexmxure.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ppjwa.cn/gtddeuxdlc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.kuanghao11.cn/gtoeixczyy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cheryme.top/gtmtfklycc.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangkeji.top/gtfvhqbisp.html

Py:   s.splitlines()
来源：http://hz.yvedp.cn/gtjzlcubbk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gogol.net.cn/gtwvgqontb.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gtvmzidaue.html

TS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gtboftpvrb.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gtjhwtatrg.html

Go:   strings.Split(s, "\n")
来源：http://hz.ehwqpu.com/gtyziyfbwq.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtuxwegjop.html

C#:   s.Split('\n')
来源：http://hz.nwbrower.top/gtbhyioebt.html

[E20] 判断字符串是否为空
来源：http://hz.316326.xyz/gtgwgtoewb.html

Py:   if not s:
来源：http://hz.sufxvd.cn/gtfssfxyjn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yongpay.top/gtkhrdohbz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtjrcekpbc.html

TS:   if (s === "") {}
来源：http://hz.jiagoushi.top/gtdsfxchtm.html

Java: if (s.isEmpty()) {}
来源：http://hz.cheryme.top/gtducrsofp.html

Go:   if s == "" {}
来源：http://hz.zhongyouzk.top/gthzflxbtb.html

Ruby: if s.empty?
来源：http://hz.cucudq.cn/gtitppklrk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gtgpiubtst.html

[E21] 超长截断加省略号
来源：http://hz.aibaodan.cn/gtqbmilshv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guannengcc.top/gtqunqlske.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gtnpfcpggf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtwftluzft.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtqbwdtdfz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtrrsolsgf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gzhubu.top/gtrsjlnkxb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.kuanghao11.cn/gtravvlxav.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhijiandao.cn/gtkdkldxxu.html

[E22] 字节长度与字符长度
来源：http://hz.tanke756.top/gtiqmuqker.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.316326.xyz/gtpaadtsvr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gteqznvoug.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtziuvqaji.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tian-w.cn/gtkggapneb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gaohongyu789.top/gtsqkweolp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jlsjyb.cn/gtepumrsue.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258.top/gtjfqginub.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sufxvd.cn/gthwsboxwe.html

================================================================================
来源：http://hz.dashuyun.cn/gtqwbmmqtc.html

F. 文件与目录
来源：http://hz.yueranfly.top/gteehvflfd.html

================================================================================
来源：http://hz.smart0.xyz/gtrjztobyr.html


<!-- 参考信息 -->