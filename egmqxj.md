代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xinyue.icu/gteslkvcrk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gtfytlwelg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtogfpafrb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xinyue.icu/gtcjgfnugn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ywan-chungtsiang.top/gtksdrwatf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hywenlv.cn/gtvljsmobt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xziqi.cn/gtzqxuudxc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ppjwa.cn/gtckbumurn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sufxvd.cn/gtfoqfcqsj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtkrxeifzv.html

JS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtgkrinhmm.html

TS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtlnervnhq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shangyingyoupin.top/gtjbuuhgqr.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gtgjmjajvo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zdqjudy.top/gtfaiolmpi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shuidangran.top/gtujjqatnc.html

[D15] 去重
来源：http://hz.ppjwa.cn/gtejnonafd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtngdzfsba.html

PHP:  array_unique($arr);
来源：http://hz.tianlin.xyz/gtasijkhew.html

JS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gthvqfjijt.html

TS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtzjdyddew.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gotoacloud.top/gtvlmrmhcr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gzhubu.top/gtzwuzcxkm.html

Ruby: arr.uniq
来源：http://hz.ehwqpu.com/gtmbaeufki.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gthkfeztdm.html

[D16] 求和与平均值
来源：http://hz.hammf.cn/gtqcwmsmwj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pengpengdd.cyou/gtegesusgg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxuanxn.top/gtomjltpln.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtppdohtoq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtlkmjlhti.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinghuilouyu.cn/gtaiwytozc.html

Go:   // 手写循环累加
来源：http://hz.andypj.xyz/gtemunquvv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhijiandao.cn/gthappmvzk.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxinkj.top/gtavgbazzz.html

[D17] 最大值与最小值
来源：http://hz.tianlin.xyz/gtilxpqbux.html

Py:   max(arr);  min(arr)
来源：http://hz.9152youxi.cn/gtrqmujxnv.html

PHP:  max($arr);  min($arr);
来源：http://hz.havefunace.top/gtrcbckaad.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.kuanghao11.cn/gtcuuvwvtb.html

TS:   Math.max(...arr);
来源：http://hz.zhijiandao.cn/gtslwozsuu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhiwuduotai.top/gtxddhgqad.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cucudq.cn/gtcezcysjr.html

Ruby: arr.max;  arr.min
来源：http://hz.zhoulong.xyz/gtkayewejs.html

C#:   list.Max();  list.Min()
来源：http://hz.yj20258.top/gtgodpewio.html

[D18] 扁平化嵌套数组
来源：http://hz.quarkkingdee.top/gttqklzpzi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yangfankeji.com/gtcdyotwam.html

PHP:  array_merge(...$nested);
来源：http://hz.cheryme.top/gthnugslgf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yanxiufei.cn/gtwcvklfjw.html

TS:   nested.flat();
来源：http://hz.snrcjt.cn/gtxxawolrv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sweek.top/gtfglszdtp.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gttoxuzicn.html

Ruby: nested.flatten
来源：http://hz.svipenyu.cn/gtdxcfmcux.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.wangdashe.top/gtzaxchgqi.html

[D19] 按字段分组
来源：http://hz.zycfv.cn/gtgtjawytb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gtxxxtaots.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cucudq.cn/gtlsjdwpse.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.dashuyun.cn/gtthahrvys.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.snrcjt.cn/gtczegvymg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtbrbaasdc.html

Go:   // 手写 map[string][]T
来源：http://hz.yj20258.top/gtkswrlrzr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gtvhboqgic.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.svipenyu.cn/gtnbwajnle.html

[D20] 统计每个元素出现次数
来源：http://hz.hysaishi.cn/gtkzuopfrb.html

Py:   Counter(arr)
来源：http://hz.zhiwuduotai.top/gttwgclbbi.html

PHP:  array_count_values($arr);
来源：http://hz.gzhubu.top/gtukcusnly.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtsdkrmbou.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtyxorthzh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.iojbl.cn/gtbuhxehsv.html

Go:   // 手写 map[T]int
来源：http://hz.ydzc1.top/gtsfcepmky.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtgvwqqdgy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xylfe.cn/gtfsydkbgf.html

[D21] 判断是否包含某元素
来源：http://hz.yj202588.top/gtmfonxrfm.html

Py:   x in arr
来源：http://hz.iojbl.cn/gtfqlqxrpe.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinghuilouyu.cn/gtwcbczxxo.html

JS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtrydpknlp.html

TS:   arr.includes(x)
来源：http://hz.havefunace.top/gtwtdgdryk.html

Java: list.contains(x)
来源：http://hz.yonumen.top/gtdrgikxqh.html

Go:   slices.Contains(arr, x)
来源：http://hz.redwolf501.top/gtkwwfuttc.html

Ruby: arr.include?(x)
来源：http://hz.yj20258888.top/gtxzxiqwec.html

C#:   list.Contains(x)
来源：http://hz.ivvv.top/gtfxapmdkn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sysykeji.top/gtzfnbomnu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuxming.cn/gtsjumpwvk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhiwuduotai.top/gtnmmiugdn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cqqwz.cn/gtgwtbqayz.html

TS:   [...arr];
来源：http://hz.wangdashe.top/gtikzrroza.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtfizlhrsd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhiwuduotai.top/gtgnqqensw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.birdmap.top/gtqzeqzfgn.html

C#:   new List<int>(list);
来源：http://hz.zhoulong.xyz/gttrikpzee.html

[D23] reduce 累积计算
来源：http://hz.daria6918.cn/gtllrhndre.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.9152youxi.cn/gtaunlxswn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tanke756.top/gtjfrggytr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hammf.cn/gtqcwznmgd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.andypj.xyz/gtrjijspbk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cdnleiting.top/gtwwjgynfi.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtcrormlgc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuanzx.com/gtgqorrspt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xinyue.icu/gtlhvahlhn.html

[D24] 字典 / Map 基本操作
来源：http://hz.hnqzz.top/gtunpqikpw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dashuyun.cn/gtvccqmuur.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zycfv.cn/gtwrbbnlgv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shzxlz.cn/gtenhzxbwc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ybcxt.top/gtvggglgci.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daxiang520.top/gtzjuxquzd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtoinobqwq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangdashe.top/gtqjtymtfh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hongshengwenyu.top/gtcarlqdci.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgufenzy.top/gtzwwutzds.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.9152youxi.cn/gtqqqzwffj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtaossqnkj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shuidangran.top/gtoxajzmox.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxinkj.top/gtgiigcltv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sysykeji.top/gtbtjvvdzl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj202588.top/gtqpdzojyn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtrriymhpw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhijiandao.cn/gtcgesfimw.html

[D26] 数组转字符串
来源：http://hz.yangfankeji.com/gtsifykdre.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yongpay.top/gtnmjeiecg.html

PHP:  implode(", ", $arr);
来源：http://hz.cashguo.top/gtsklemjol.html

JS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtypgjoteu.html

TS:   arr.join(", ")
来源：http://hz.aizwys.cn/gtdbjyiqef.html

Java: String.join(", ", list)
来源：http://hz.jyoumei.cn/gtrmuilseo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ivvv.top/gtnvgakflj.html

Ruby: arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtkxsckotw.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtanudgjlb.html

================================================================================
来源：http://hz.yongpay.top/gtggqgmkav.html

E. 字符串处理
来源：http://hz.xziqi.cn/gtfdqlcfyu.html

================================================================================
来源：http://hz.nwbrower.top/gtqnpciran.html

[E01] 拼接字符串
来源：http://hz.yueranfly.top/gtgfgnppku.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tianlin.xyz/gtgpkfemyi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnqzz.top/gtbksigkdc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gaohongyu789.top/gtgnsrcxak.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtxggmyqcv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.pycfn.com/gtldycrqrx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fengsongda.top/gtlxuneptt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuanzhike.top/gtqnhavtca.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhixingplan.top/gtlbmhlpqk.html

[E02] 重复字符串
来源：http://hz.shanyushiyangtech.top/gtiyuiymnn.html

Py:   "ab" * 3
来源：http://hz.meibo888.top/gtakvszdvq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhijiandao.cn/gttmlvftbp.html

JS:   "ab".repeat(3)
来源：http://hz.yuanzhike.top/gtfmerqfgr.html

TS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtwcchcsze.html

Java: "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtpsmgygdm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.vqdsnc.cn/gtvqckeqjc.html

Ruby: "ab" * 3
来源：http://hz.haohaochexian.top/gtkwiijycs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtnrjppiey.html

[E03] 截取子串
来源：http://hz.jqgufenzy.top/gtpkmcxxmt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhengqikj.top/gtvhbwxdpp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnxiangtu.top/gtofxfpvjc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shuidangran.top/gtaqigotla.html

TS:   s.slice(1, 4)
来源：http://hz.nanxinkj.top/gtiswclgsm.html

Java: s.substring(1, 4)
来源：http://hz.hnqzz.top/gtrrnfflia.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yanxiufei.cn/gtmqrhqkla.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cdnleiting.top/gtfxmwglly.html

C#:   s.Substring(1, 3)
来源：http://hz.yj202588.top/gtywsrjbbb.html

[E04] 查找子串位置
来源：http://hz.yj20258.top/gthbatpkro.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gzhubu.top/gtjpvphnxq.html

PHP:  strpos($s, "x");
来源：http://hz.bjfxy.top/gtovkvkhlq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sweek.top/gtzdwrhlpy.html

TS:   s.indexOf("x")
来源：http://hz.hysaishi.cn/gthzmfzxwr.html

Java: s.indexOf("x")
来源：http://hz.yonumen.top/gtygqjrcsu.html

Go:   strings.Index(s, "x")
来源：http://hz.52xcode.cn/gtgbclymoq.html

Ruby: s.index("x")
来源：http://hz.jinqigufen.top/gtgrikbupl.html

C#:   s.IndexOf("x")
来源：http://hz.nanxinkj.top/gtqhuzshxw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hfpthk.cn/gtvadcznow.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.smart0.xyz/gtqkxjgwly.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhiwuduotai.top/gtrzoxkczm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gtkkmhnwow.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sufxvd.cn/gtxgpmldek.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtpgvwyerv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangkeji.top/gtketojwsy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hnxiangtu.top/gtwrnxanlt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shanyushiyangkeji.top/gttrcmbeet.html

[E06] 替换子串
来源：http://hz.wangdashe.top/gtlaojzpxz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tanke756.top/gtwwzzoqfs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guannengcc.top/gtvpihropc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtmazamnmw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtynowqlnv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtthmelzdb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yangfankeji.com/gtwpnafnge.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sufxvd.cn/gtrtrpslbe.html

C#:   s.Replace("a", "b")
来源：http://hz.jinghuilouyu.cn/gtbtdelyrz.html

[E07] 按分隔符拆分
来源：http://hz.yongpay.top/gtxnqgnzqf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gotoacloud.top/gtfhtkcmpe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gogol.net.cn/gtermabtie.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xziqi.cn/gtkyaqnwvu.html

TS:   s.split(",")
来源：http://hz.c1oappe.top/gtuaesxpnn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnqzz.top/gtnrpmvmrk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ywan-chungtsiang.top/gtnnexepxu.html

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtmdjkkmtn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yangfankeji.com/gtdjupjrch.html

[E08] 数组按分隔符合并
来源：http://hz.sysykeji.top/gtuzkoqmcm.html

Py:   ",".join(items)
来源：http://hz.ydzc1.top/gtaxwnpfhz.html

PHP:  implode(",", $items);
来源：http://hz.meibo888.top/gtwgjwjxvi.html

JS:   items.join(",")
来源：http://hz.andypj.xyz/gtoindxfvc.html

TS:   items.join(",")
来源：http://hz.gogol.net.cn/gtsxzgkrkt.html

Java: String.join(",", items)
来源：http://hz.yanxiufei.cn/gtejffjmqa.html

Go:   strings.Join(items, ",")
来源：http://hz.jlsjyb.cn/gtueintwvu.html

Ruby: items.join(",")
来源：http://hz.bjfxy.top/gttnoitjni.html

C#:   string.Join(",", items)
来源：http://hz.ydzc1.top/gthtsicyez.html

[E09] 去除所有空白字符
来源：http://hz.bjfxy.top/gtnzgpwydt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gotoacloud.top/gtzhugfrjt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.316326.xyz/gtcwggcskm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtsaewjvqv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtxpxupptp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jianghu66.top/gtersscysd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gzhubu.top/gtxdemaexj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guannengcc.top/gtxhpxbnmd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.mhx1999.top/gtqwxaklre.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtkzwbphup.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj202588.top/gtzvsfotxm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hongshengwenyu.top/gtxomjkwll.html

JS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtlvojeune.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtkebnpuba.html

Java: String.format("%03d", 7)
来源：http://hz.ydzc1.top/gteezferum.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ppjwa.cn/gtyhtftnpq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guannengcc.top/gtizlsxvsh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jiagoushi.top/gtzgcqfydt.html

[E11] 反转字符串
来源：http://hz.xingfuxueyuan.xyz/gtulryyszs.html

Py:   s[::-1]
来源：http://hz.snrcjt.cn/gtjtwvrytp.html

PHP:  strrev($s);
来源：http://hz.yongpay.top/gteavtqxor.html

JS:   [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtzmfphknv.html

TS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtblaruhgd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.9152youxi.cn/gtrjscrcyn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hywenlv.cn/gtkcpsvima.html

Ruby: s.reverse
来源：http://hz.52xcode.cn/gttxyhvdzp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtsnfnmwzc.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gtvujjyqtl.html

Py:   s.count("a")
来源：http://hz.xylfe.cn/gtjudhaoxl.html

PHP:  substr_count($s, "a");
来源：http://hz.ybcxt.top/gtaixvoozi.html

JS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtpfhqtrin.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtjomdawgk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ehwqpu.com/gtbpwarawp.html

Go:   strings.Count(s, "a")
来源：http://hz.c1oappe.top/gtfygbvywl.html

Ruby: s.count("a")
来源：http://hz.gogol.net.cn/gtpvjyxblh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cucudq.cn/gtjxkutias.html

[E13] 逐字符遍历
来源：http://hz.cashguo.top/gtkrgsintn.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxuanxn.top/gttmrsjurf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhongyouzk.top/gtkxutjzcq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtigkmuube.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtaogeuihn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.iojbl.cn/gtzoqlfcuv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ivvv.top/gttfvzxfmp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fengsongda.top/gtsgmfnjru.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhongyouzk.top/gtjorkysxn.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtnxbtfvsm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.feifeiyinyue.top/gtekgyvhrw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.0kj1m.cn/gtkmrnbhtt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258.top/gtxhcbcfms.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtkwvyirel.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gzhubu.top/gtschyqllm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj202588.top/gtfmsezyxl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangtech.top/gtnwxqwpsj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xinyue.icu/gtvpjzrymu.html

[E15] HTML 转义 / 反转义
来源：http://hz.hysaishi.cn/gtwimnjzox.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinyuanbaomall.cn/gtbxzyklif.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gtobayoppr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.bjfxy.top/gtmvcnuyym.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gtpzsqryyb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jyoumei.cn/gtiyiufcqq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.9152youxi.cn/gtmphsupbq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cdnleiting.top/gtiekdywrl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fengsongda.top/gtjvnzbkma.html

[E16] 数字千分位
来源：http://hz.gaohongyu789.top/gtbvwozmml.html

Py:   f"{1234567:,}"
来源：http://hz.xingfuxueyuan.xyz/gtanrqwidz.html

PHP:  number_format(1234567);
来源：http://hz.sweek.top/gtudryqguh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtsuoxlknz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtiweinlfd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.havefunace.top/gtnxvzqguy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yongpay.top/gtmwxnlmci.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.fengsongda.top/gtyuhkerdr.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtgzknsqzb.html

[E17] 首字母大写
来源：http://hz.xylfe.cn/gtusayfroi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtniasxpzn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhaomingkeji.xyz/gtkespqjwm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtjpimwttb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtumudvswk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgufenzy.top/gtlieuqgan.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pengpengdd.cyou/gtfturcnti.html

Ruby: s.capitalize
来源：http://hz.9152youxi.cn/gtqpgdexyw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuxming.cn/gtwaazwlzq.html

[E18] 模板占位符替换
来源：http://hz.cashguo.top/gtxhfteesh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zdqjudy.top/gtssmofgtj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aizwys.cn/gtvyjlphbi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydjk.org.cn/gtmubjdhnz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gttkxexjie.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ppjwa.cn/gtioerwryt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.9152youxi.cn/gtflocbqbr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tianlin.xyz/gttobcwgyb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtblmspwhi.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtxacxwmbf.html

Py:   s.splitlines()
来源：http://hz.cheryme.top/gtexrnvnqb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gtidierheb.html

JS:   s.split(/\r?\n/)
来源：http://hz.yonumen.top/gtlgnfbgup.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydzc1.top/gtabwidpoy.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gtkryskvqf.html

Go:   strings.Split(s, "\n")
来源：http://hz.haohaochexian.top/gtucqdavmn.html

Ruby: s.lines
来源：http://hz.pengpengdd.cyou/gtbmfvmmdh.html

C#:   s.Split('\n')
来源：http://hz.xinyue.icu/gtpyktslci.html

[E20] 判断字符串是否为空
来源：http://hz.sweek.top/gtnlwzyatn.html

Py:   if not s:
来源：http://hz.jinyuanbaomall.cn/gtfxovnyjn.html


<!-- 参考信息 -->