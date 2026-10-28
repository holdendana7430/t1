代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnqzz.top/gtzsicwdsh.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtphlccybg.html

[D17] 最大值与最小值
来源：http://hz.cucudq.cn/gtergandzr.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangtech.top/gtefctwsjj.html

PHP:  max($arr);  min($arr);
来源：http://hz.shuidangran.top/gtohhzlgft.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.c1oappe.top/gtlsucrtbk.html

TS:   Math.max(...arr);
来源：http://hz.aizwys.cn/gtkeqdzkbw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aibaodan.cn/gtzlrelray.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jyoumei.cn/gtchhkrqbg.html

Ruby: arr.max;  arr.min
来源：http://hz.zdqjudy.top/gtvgtuuigf.html

C#:   list.Max();  list.Min()
来源：http://hz.jlsjyb.cn/gtswrvwttc.html

[D18] 扁平化嵌套数组
来源：http://hz.dianchejie.cn/gtqafozldw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yvedp.cn/gtuxbsguhj.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigfzy.top/gtsncxsmtn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xziqi.cn/gtknpnubwl.html

TS:   nested.flat();
来源：http://hz.ydjk.org.cn/gtxddtcxvq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yongpay.top/gtjahynoni.html

Go:   // 手写双层循环
来源：http://hz.yonumen.top/gtdevfauyc.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtbohmcwil.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gthpjbgfcl.html

[D19] 按字段分组
来源：http://hz.zhoulong.xyz/gtfgmpxvzy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gtilokutfq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.mhx1999.top/gtlgqmpioz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hammf.cn/gtpjeqncxb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtbffzzxzp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtvtatfkze.html

Go:   // 手写 map[string][]T
来源：http://hz.gotoacloud.top/gtmmhevjly.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ppjwa.cn/gtzkcwbeil.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sxryk.cn/gtptaqpyrz.html

[D20] 统计每个元素出现次数
来源：http://hz.ivvv.top/gtjqqacxpw.html

Py:   Counter(arr)
来源：http://hz.c1oappe.top/gtwvdnxhxf.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtfmhpjspr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtcrfvuunc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtpekljtee.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.quarkkingdee.top/gtfzgjiiwd.html

Go:   // 手写 map[T]int
来源：http://hz.xuetiantiany.cn/gtxpakocyo.html

Ruby: arr.tally
来源：http://hz.cashguo.top/gtmidqmitb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ywan-chungtsiang.top/gtjlwzzgep.html

[D21] 判断是否包含某元素
来源：http://hz.gogol.net.cn/gtqivdubko.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gtofcsxwaq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cheryme.top/gticmjtjbd.html

JS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtlmdiuvtm.html

TS:   arr.includes(x)
来源：http://hz.yvedp.cn/gtfexirtal.html

Java: list.contains(x)
来源：http://hz.sysykeji.top/gthndylhvf.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangdashe.top/gtptuariuv.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtyhlrjcww.html

C#:   list.Contains(x)
来源：http://hz.hywenlv.cn/gtmnsoaeeb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.quarkkingdee.top/gtbuvhpmpb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhixingplan.top/gtmgrtjuld.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gtqygyuhum.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jlsjyb.cn/gtfjaweufq.html

TS:   [...arr];
来源：http://hz.vqdsnc.cn/gtdyohlrjc.html

Java: new ArrayList<>(list);
来源：http://hz.zycfv.cn/gtaxvxhvnm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuetiantiany.cn/gttztkdhad.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhengqikj.top/gtlxoiwtqu.html

C#:   new List<int>(list);
来源：http://hz.wangdashe.top/gthjkjvryw.html

[D23] reduce 累积计算
来源：http://hz.zhiwuduotai.top/gtwekkdlwu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.dashuyun.cn/gtnacqwxed.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daria6918.cn/gtvzyiqeqi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtrzltmonn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtxyekfyhk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jyoumei.cn/gtlwsgfqfa.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gtsbtdzbjf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtxwublven.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangshuangyany.cn/gtcdrmkvkk.html

[D24] 字典 / Map 基本操作
来源：http://hz.yangfankeji.com/gtwkkqkpch.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.meibo888.top/gtnspppzib.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangshuangyany.cn/gtbzrknelv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhongyouzk.top/gtgzoximbq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gzhubu.top/gtxdsppxgc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxuanxn.top/gtmdbchfma.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daria6918.cn/gtjqsgnipy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhengqikj.top/gtdhfdwvrg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtmsuhiioa.html

[D25] Set 集合去重与交并差
来源：http://hz.cucudq.cn/gtcjljjrun.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgufenzy.top/gtpnugsbvb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xylfe.cn/gtgwhyffgs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhoulong.xyz/gtzogmgrtg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhixingplan.top/gteumpnplh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ivvv.top/gtxuadpgfd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtmraudhmj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.bjfxy.top/gtevhkrnzo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gtaknddnuq.html

[D26] 数组转字符串
来源：http://hz.smart0.xyz/gtdbgatdam.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gaohongyu789.top/gtgbvzpale.html

PHP:  implode(", ", $arr);
来源：http://hz.jyoumei.cn/gthfqbdxtc.html

JS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtsolztqhz.html

TS:   arr.join(", ")
来源：http://hz.xziqi.cn/gtbyasucuy.html

Java: String.join(", ", list)
来源：http://hz.meibo888.top/gtqkaxrpoe.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gogol.net.cn/gtitruhzdb.html

Ruby: arr.join(", ")
来源：http://hz.nanxinkj.top/gtteivkzxc.html

C#:   string.Join(", ", list)
来源：http://hz.jiagoushi.top/gtfjbofgsn.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvvnsvlej.html

E. 字符串处理
来源：http://hz.fengsongda.top/gtxtycodyu.html

================================================================================
来源：http://hz.aibaodan.cn/gtssybmbaw.html

[E01] 拼接字符串
来源：http://hz.sysykeji.top/gtlpeaacen.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtaszfnona.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shangyingyoupin.top/gtsckqkjri.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtyptncyrk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtcvgnhozm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dianchejie.cn/gtbrlusdbv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.redwolf501.top/gtcfubcbqh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cdnleiting.top/gtiimbigka.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cqqwz.cn/gtyglhfekd.html

[E02] 重复字符串
来源：http://hz.jianghu66.top/gtegaggdcl.html

Py:   "ab" * 3
来源：http://hz.pycfn.com/gtfvksanyw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gogol.net.cn/gtfintbfbu.html

JS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtaydyxsch.html

TS:   "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtyfllkbpg.html

Java: "ab".repeat(3)
来源：http://hz.shuidangran.top/gtaoyxzhak.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jiagoushi.top/gtunqabmvp.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gthczvffqi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.redwolf501.top/gtlzooqhye.html

[E03] 截取子串
来源：http://hz.gaohongyu789.top/gtyqchzfhh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ppjwa.cn/gtizysqbrg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj202588.top/gtnemumkzc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.smart0.xyz/gtfasbikco.html

TS:   s.slice(1, 4)
来源：http://hz.dashuyun.cn/gthsrluaob.html

Java: s.substring(1, 4)
来源：http://hz.birdmap.top/gtwicdzgci.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenzaomai.com/gtvpekudwu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yvedp.cn/gtttjdsmnj.html

C#:   s.Substring(1, 3)
来源：http://hz.cdnleiting.top/gtfnamzjyc.html

[E04] 查找子串位置
来源：http://hz.ywan-chungtsiang.top/gtacqexphg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhongyouzk.top/gtejoaunig.html

PHP:  strpos($s, "x");
来源：http://hz.daria6918.cn/gttddlogvt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tanke756.top/gtiprcklcg.html

TS:   s.indexOf("x")
来源：http://hz.316326.xyz/gtqtejkpxb.html

Java: s.indexOf("x")
来源：http://hz.fengsongda.top/gtsqqtbnwa.html

Go:   strings.Index(s, "x")
来源：http://hz.zhengqikj.top/gtrslrqlry.html

Ruby: s.index("x")
来源：http://hz.hammf.cn/gtdwrdqqpx.html

C#:   s.IndexOf("x")
来源：http://hz.nwbrower.top/gtsfzawmiy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hysaishi.cn/gtbpuqhlwg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nwbrower.top/gtggsvtjip.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigufen.top/gtatpsdzwy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtwczsjqyq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xziqi.cn/gtvjzdsprh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhongyouzk.top/gtqiycmyfz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.birdmap.top/gtffzrqwfg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tian-w.cn/gtlktprjzy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gtwjwfwtos.html

[E06] 替换子串
来源：http://hz.jiagoushi.top/gtcdcyprbc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jyoumei.cn/gtojmgglli.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ppjwa.cn/gtkzdpyezx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtzgdarwmq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtiwcgfynu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtskbnmmoy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gzhubu.top/gtumlxcqfq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guowangkeji.top/gtjcgozxrx.html

C#:   s.Replace("a", "b")
来源：http://hz.cashguo.top/gtvqdqmihb.html

[E07] 按分隔符拆分
来源：http://hz.sufxvd.cn/gtctucmqap.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jiagoushi.top/gthwtgamtf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtivbujdck.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhongyouzk.top/gtenjzzcru.html

TS:   s.split(",")
来源：http://hz.fzhhl.top/gthnelanqo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gttbuuvkpe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yvedp.cn/gtclbodtuc.html

Ruby: s.split(",");  s.split
来源：http://hz.guowangkeji.top/gteypowwng.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinghuilouyu.cn/gtbzxuwdzj.html

[E08] 数组按分隔符合并
来源：http://hz.birdmap.top/gtvypoqlqp.html

Py:   ",".join(items)
来源：http://hz.sufxvd.cn/gtmqenldws.html

PHP:  implode(",", $items);
来源：http://hz.yvedp.cn/gtazjqgitr.html

JS:   items.join(",")
来源：http://hz.yonumen.top/gtqhfmdlkm.html

TS:   items.join(",")
来源：http://hz.gogol.net.cn/gtkuhcqvja.html

Java: String.join(",", items)
来源：http://hz.pengpengdd.cyou/gtadwloxur.html

Go:   strings.Join(items, ",")
来源：http://hz.hnxiangtu.top/gtfoorsagr.html

Ruby: items.join(",")
来源：http://hz.cdnleiting.top/gtosvmgczr.html

C#:   string.Join(",", items)
来源：http://hz.jinghuilouyu.cn/gtujaskion.html

[E09] 去除所有空白字符
来源：http://hz.wangshuangyany.cn/gtusbjhyxp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuetiantiany.cn/gtxlbhvgrr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yuanzhike.top/gtdrhypgiq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aizwys.cn/gtcgxzjhpw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtiggcwvse.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hysaishi.cn/gtgnbexrpo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtmibkrfja.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.feifeiyinyue.top/gtevfbyvtq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ppjwa.cn/gtyvhbdbdg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.iojbl.cn/gtxtsilyei.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhoulong.xyz/gtxuwrokhg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtlezvcmzh.html

JS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtgyxbdhbk.html

TS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtptxobtgo.html

Java: String.format("%03d", 7)
来源：http://hz.jqgfzy.top/gtczegdsvq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhongyouzk.top/gtywikxrau.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtpdgyypcz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shangyingyoupin.top/gtphgoabos.html

[E11] 反转字符串
来源：http://hz.cdnleiting.top/gtdttddzfd.html

Py:   s[::-1]
来源：http://hz.cucudq.cn/gtnpcwhqwb.html

PHP:  strrev($s);
来源：http://hz.sweek.top/gtaewgunam.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtuqfjzccp.html

TS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtvcobpwbz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cucudq.cn/gtdtfhlrjb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hywenlv.cn/gtptvujkwn.html

Ruby: s.reverse
来源：http://hz.aizwys.cn/gtpeklbtvr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtjfggrkoc.html

[E12] 统计某字符出现次数
来源：http://hz.xylfe.cn/gtjckfdznz.html

Py:   s.count("a")
来源：http://hz.yj20258888.top/gtwuwgoebe.html

PHP:  substr_count($s, "a");
来源：http://hz.0kj1m.cn/gtikdwvkvc.html

JS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtkjpqfczn.html

TS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtvivcqcvv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hysaishi.cn/gtvhsxhkbz.html

Go:   strings.Count(s, "a")
来源：http://hz.andypj.xyz/gtuwxezyrz.html

Ruby: s.count("a")
来源：http://hz.havefunace.top/gtnpwuoijt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gogol.net.cn/gtyyukhxrt.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtikfkrcxi.html

Py:   for ch in s: print(ch)
来源：http://hz.hysaishi.cn/gtzksggtue.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangtech.top/gtyxiunpex.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gtvcvhmynx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtzwhhdigs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuanzx.com/gtrzhxfyoa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtrwaaztfx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jianghu66.top/gtjlrfnklq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.mhx1999.top/gtpjtcbmaa.html

[E14] URL 编码与 Base64
来源：http://hz.meibo888.top/gtpwivhlfa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gtyloumevx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinyuanbaomall.cn/gtbplcyphj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sxryk.cn/gtozfcxpvu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ywan-chungtsiang.top/gtjhppdflu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aibaodan.cn/gtxyjitogm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangkeji.top/gtvkpxbsel.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jlsjyb.cn/gtwimyxord.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.haohaochexian.top/gtkfeezrtf.html

[E15] HTML 转义 / 反转义
来源：http://hz.nanxuanxn.top/gtpxbehwwo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.andypj.xyz/gtkahntocn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shzxlz.cn/gtsjxzastr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sufxvd.cn/gtmzdwjnoe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtooqrbflc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yonumen.top/gtcjmpdtjw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hywenlv.cn/gtuxizqwsp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinyuanbaomall.cn/gtzcrtxfwl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinghuilouyu.cn/gtjsihsdnx.html

[E16] 数字千分位
来源：http://hz.c1oappe.top/gtwqwzdqaa.html

Py:   f"{1234567:,}"
来源：http://hz.ywan-chungtsiang.top/gtxtcfqdqc.html

PHP:  number_format(1234567);
来源：http://hz.xziqi.cn/gtzcwozotk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtqnfgcdyr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhijiandao.cn/gtckrjqgnr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuetiantiany.cn/gtiphraxqx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tanke756.top/gtoiadersl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tianlin.xyz/gtlrvsckcv.html

C#:   1234567.ToString("N0")
来源：http://hz.52xcode.cn/gtctctcqse.html

[E17] 首字母大写
来源：http://hz.quarkkingdee.top/gtxxnwhqgp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yvedp.cn/gtqcylcywo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtljqwosbo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgufenzy.top/gtyheuryip.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtotqdgyzk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yuxming.cn/gtnzkoxnzi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj202588.top/gtnujbmzvi.html

Ruby: s.capitalize
来源：http://hz.jyoumei.cn/gtsfcudshf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sweek.top/gtpjhfoptl.html

[E18] 模板占位符替换
来源：http://hz.mhx1999.top/gtnribtsrc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shuidangran.top/gtscvmhbvd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cucudq.cn/gtnwelzmha.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gtyphpouez.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gtnwaiiorl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gthcljzlgr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jianghu66.top/gtfaecsmhd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.redwolf501.top/gtcxnhwoht.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.52xcode.cn/gtdungpnkv.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtivfwxnzv.html

Py:   s.splitlines()
来源：http://hz.guowangkeji.top/gtruvukkdl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.birdmap.top/gtqpiwfkpm.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gtyrxuuhet.html

TS:   s.split(/\r?\n/)
来源：http://hz.vqdsnc.cn/gtitrsiikn.html

Java: s.lines().toList()
来源：http://hz.yvedp.cn/gtdjaxzoif.html

Go:   strings.Split(s, "\n")
来源：http://hz.snrcjt.cn/gtipgbplrs.html

Ruby: s.lines
来源：http://hz.xuanzx.com/gtadwaunxa.html

C#:   s.Split('\n')
来源：http://hz.52xcode.cn/gtizhdcmdk.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtgswonjqi.html

Py:   if not s:
来源：http://hz.yueranfly.top/gtzeumdifp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.52xcode.cn/gttaodastk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ybcxt.top/gtfscoqkfw.html

TS:   if (s === "") {}
来源：http://hz.zycfv.cn/gtsjqhcyje.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtatpnnlpx.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtmroevpwe.html

Ruby: if s.empty?
来源：http://hz.redwolf501.top/gtzbkdwthw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yonumen.top/gtjqgngmov.html

[E21] 超长截断加省略号
来源：http://hz.hammf.cn/gtczzubmng.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuetiantiany.cn/gtwtiefatv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hammf.cn/gtwhsqfmey.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtqfyufmzh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtvgvubbvj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtnqhgraug.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtqkyllptl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ybcxt.top/gtgsydtmwh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.birdmap.top/gtcaxvzrwy.html

[E22] 字节长度与字符长度
来源：http://hz.iojbl.cn/gtnruqgltv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenjidiqi.icu/gtwhlkvdpq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gttjcxozaf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtlkiyiztj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtngewyrea.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtqmjlrwhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.svipenyu.cn/gtsaajveid.html

Ruby: s.bytesize;  s.length
来源：http://hz.bjfxy.top/gtdxjwkxbd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj202588.top/gtynitlnqw.html

================================================================================
来源：http://hz.yuanzhike.top/gtmiilhggl.html

F. 文件与目录
来源：http://hz.svipenyu.cn/gtaxoftoef.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtazzbxeox.html

[F01] 读取整个文件
来源：http://hz.ppjwa.cn/gtpcowhaci.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhongyouzk.top/gtxmnjibzf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hysaishi.cn/gtwudldwoq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhengqikj.top/gtxqbkoees.html


<!-- 参考信息 -->