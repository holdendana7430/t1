代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtktxddhkr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jyoumei.cn/gtohulsvxx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fengsongda.top/gtagfociir.html

Ruby: arr.uniq
来源：http://hz.havefunace.top/gtrftwtlnh.html

C#:   list.Distinct().ToList()
来源：http://hz.gaohongyu789.top/gtnglqncdv.html

[D16] 求和与平均值
来源：http://hz.jinqigufen.top/gtimezpcoe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtmfujghjs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.9152youxi.cn/gtdkpoybbi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtgchmiutr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pengpengdd.cyou/gttrpghddp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zycfv.cn/gtnfaqrbjj.html

Go:   // 手写循环累加
来源：http://hz.fzhhl.top/gturizydbm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gtttiutzyo.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnqzz.top/gtfqytqmly.html

[D17] 最大值与最小值
来源：http://hz.hnqzz.top/gtwfnsteyu.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtpsnzzdub.html

PHP:  max($arr);  min($arr);
来源：http://hz.kuanghao11.cn/gtmfeuekpo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guowangkeji.top/gttifrchlm.html

TS:   Math.max(...arr);
来源：http://hz.vqdsnc.cn/gtzfvyzaap.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gaohongyu789.top/gtvoohnkwz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jyoumei.cn/gttimuycym.html

Ruby: arr.max;  arr.min
来源：http://hz.svipenyu.cn/gtzbhgpeqe.html

C#:   list.Max();  list.Min()
来源：http://hz.fzhhl.top/gtsdktiylu.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgufenzy.top/gtpihnqeqg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guannengcc.top/gthognavel.html

PHP:  array_merge(...$nested);
来源：http://hz.chenzaomai.com/gtnvnscmiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinghuilouyu.cn/gtgdnljoro.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gtysjnzsnr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zycfv.cn/gtftfrpjpe.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtrrikslqp.html

Ruby: nested.flatten
来源：http://hz.redwolf501.top/gtgdoclfpr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnxiangtu.top/gtymowpzsa.html

[D19] 按字段分组
来源：http://hz.havefunace.top/gtnagbonjb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aizwys.cn/gttjeiizqf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydjk.org.cn/gtttbgifrf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ybcxt.top/gtvfbgxwgc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ywan-chungtsiang.top/gtvspfdbzk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gtmcvgewld.html

Go:   // 手写 map[string][]T
来源：http://hz.dianchejie.cn/gtbfutotti.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.havefunace.top/gtjlfegluf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.0kj1m.cn/gtbzoagswn.html

[D20] 统计每个元素出现次数
来源：http://hz.fzhhl.top/gtfgsnrizm.html

Py:   Counter(arr)
来源：http://hz.havefunace.top/gtjdidfcmh.html

PHP:  array_count_values($arr);
来源：http://hz.svipenyu.cn/gttiblbjpx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtgtclunbo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtcdimockw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenzaomai.com/gtzvsyojda.html

Go:   // 手写 map[T]int
来源：http://hz.shzxlz.cn/gtwfvvovyr.html

Ruby: arr.tally
来源：http://hz.redwolf501.top/gtovcfrffu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenzaomai.com/gtvvmbopoq.html

[D21] 判断是否包含某元素
来源：http://hz.havefunace.top/gthgtopkvf.html

Py:   x in arr
来源：http://hz.yuxming.cn/gtmvsegqif.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xylfe.cn/gtekmzevwn.html

JS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtdaxmxhqb.html

TS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtmaqeshin.html

Java: list.contains(x)
来源：http://hz.shangyingyoupin.top/gtqawdyjfi.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gtpliwfyta.html

Ruby: arr.include?(x)
来源：http://hz.yangfankeji.com/gtjqvllwul.html

C#:   list.Contains(x)
来源：http://hz.pengpengdd.cyou/gtldjfayfv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sufxvd.cn/gtuaxkqbwo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhijiandao.cn/gtbsfwgmmy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.andypj.xyz/gtcxgcjizn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxinkj.top/gtnumjcsuq.html

TS:   [...arr];
来源：http://hz.nanxuanxn.top/gtoyjwzdnf.html

Java: new ArrayList<>(list);
来源：http://hz.shanyushiyangtech.top/gtehetaadd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aibaodan.cn/gtotqrqicu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.haohaochexian.top/gthjbhrral.html

C#:   new List<int>(list);
来源：http://hz.meibo888.top/gtpginairx.html

[D23] reduce 累积计算
来源：http://hz.aibaodan.cn/gtacbpdeee.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cdnleiting.top/gtgvojxdkq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xingfuxueyuan.xyz/gtwnrcqxww.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtdlxbopqq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtdrxprkon.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ywan-chungtsiang.top/gtzavoavdz.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtbethcuqm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangtech.top/gtbwemydnx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.dashuyun.cn/gtfvxgmhkq.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhengqikj.top/gtvacvyfdf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shanyushiyangtech.top/gteomjydjb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hammf.cn/gtyizvjenz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinyuanbaomall.cn/gtbhgeuvfh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.fengsongda.top/gtjfhxaeha.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.mhx1999.top/gtcwlrgsvn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangdashe.top/gtqbiuresy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.52xcode.cn/gtuhcrseyf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigfzy.top/gtuhcjnayu.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigufen.top/gtspocfzjw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gtizafgzsb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtvthuldnv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sufxvd.cn/gtmotzyecs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gaohongyu789.top/gtchcosxzt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aibaodan.cn/gtisoynmgb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.9152youxi.cn/gtxvyieckk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhoulong.xyz/gtdfhnlbrv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sufxvd.cn/gtxwfpevbf.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangtech.top/gtkewypidh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gtyqtjismy.html

PHP:  implode(", ", $arr);
来源：http://hz.nanxinkj.top/gtnsvdynrg.html

JS:   arr.join(", ")
来源：http://hz.nanxinkj.top/gtoticxozb.html

TS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtvnhbrliq.html

Java: String.join(", ", list)
来源：http://hz.ehwqpu.com/gtwdoqcdxo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shanyushiyangkeji.top/gtpxoyfnek.html

Ruby: arr.join(", ")
来源：http://hz.316326.xyz/gtosxkdgbh.html

C#:   string.Join(", ", list)
来源：http://hz.zhoulong.xyz/gtdpakuxqq.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwxeogxdg.html

E. 字符串处理
来源：http://hz.fzhhl.top/gtmkrrrhky.html

================================================================================
来源：http://hz.ydjk.org.cn/gtqhynfuba.html

[E01] 拼接字符串
来源：http://hz.xziqi.cn/gtxvzthvpt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.kuanghao11.cn/gtwupazmbo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cucudq.cn/gtxpktpxxp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtuwjjscie.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gttwsamgzz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenlongwang.top/gtnulcvpvu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nwbrower.top/gtbmlpumnf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj202588.top/gtxswzeeix.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhiwuduotai.top/gtxjlymbfj.html

[E02] 重复字符串
来源：http://hz.9152youxi.cn/gtzqwisayg.html

Py:   "ab" * 3
来源：http://hz.c1oappe.top/gthjhojfrc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.feifeiyinyue.top/gtfouumivy.html

JS:   "ab".repeat(3)
来源：http://hz.sufxvd.cn/gthpjgjybz.html

TS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtnrvlrgaz.html

Java: "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtgnuxhnwa.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ehwqpu.com/gthzzqakvn.html

Ruby: "ab" * 3
来源：http://hz.jianghu66.top/gtwgshttay.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ydzc1.top/gtserxcjhq.html

[E03] 截取子串
来源：http://hz.feifeiyinyue.top/gtwpmnplpv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fzhhl.top/gtojznzczc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shuidangran.top/gtjkbblubh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pengpengdd.cyou/gtkidebztx.html

TS:   s.slice(1, 4)
来源：http://hz.bjfxy.top/gtmznxmtcj.html

Java: s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtvenlacrd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xziqi.cn/gtaejvpujv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guannengcc.top/gtcjufhnaj.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258888.top/gtnqbvhpbp.html

[E04] 查找子串位置
来源：http://hz.yj20258.top/gtyyskoonr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxinkj.top/gtbqtzwaey.html

PHP:  strpos($s, "x");
来源：http://hz.zhengqikj.top/gtgjjukcuw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hammf.cn/gtiqypaphw.html

TS:   s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtkjtjmwqz.html

Java: s.indexOf("x")
来源：http://hz.sysykeji.top/gtxivtsfpa.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgufenzy.top/gtigteqnpl.html

Ruby: s.index("x")
来源：http://hz.yuxming.cn/gtpfmglnlg.html

C#:   s.IndexOf("x")
来源：http://hz.nwbrower.top/gtdxvnwjro.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gogol.net.cn/gtcynkjpjv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuanzx.com/gtwubinpwf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.redwolf501.top/gtslrfnvbq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gthxilxvok.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zdqjudy.top/gtqbpuiwyi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtfganjgcd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hnqzz.top/gtthzjzsti.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fzhhl.top/gtqnepgjtw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ybcxt.top/gtmicxwxth.html

[E06] 替换子串
来源：http://hz.tianlin.xyz/gtatrpokxc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtxgbblcem.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shanyushiyangtech.top/gtjhzablkp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtqxbgthkx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtlnqbqjue.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtjhkloaln.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuxming.cn/gtveuasxba.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nanxinkj.top/gtbfseauel.html

C#:   s.Replace("a", "b")
来源：http://hz.guannengcc.top/gtcfmthiuy.html

[E07] 按分隔符拆分
来源：http://hz.cucudq.cn/gtidbyagha.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinqigufen.top/gtjtmyrbks.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yonumen.top/gtsymhrkvv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhengqikj.top/gtjevegxsg.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtmvcbumfn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnqzz.top/gttclsawug.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gthvjjhvzd.html

Ruby: s.split(",");  s.split
来源：http://hz.haohaochexian.top/gtlovhhizc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pengpengdd.cyou/gtlybnfert.html

[E08] 数组按分隔符合并
来源：http://hz.hnqzz.top/gtigvyleyp.html

Py:   ",".join(items)
来源：http://hz.sufxvd.cn/gtpamzpgno.html

PHP:  implode(",", $items);
来源：http://hz.gzhubu.top/gtwmcaueoa.html

JS:   items.join(",")
来源：http://hz.hysaishi.cn/gtbczylxjb.html

TS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtganigxkj.html

Java: String.join(",", items)
来源：http://hz.wangdashe.top/gtevfdxzug.html

Go:   strings.Join(items, ",")
来源：http://hz.tianlin.xyz/gtiyclvyqk.html

Ruby: items.join(",")
来源：http://hz.cdnleiting.top/gtabtjxnqm.html

C#:   string.Join(",", items)
来源：http://hz.nanxuanxn.top/gttvngkapv.html

[E09] 去除所有空白字符
来源：http://hz.shangyingyoupin.top/gtmarpmodp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xingfuxueyuan.xyz/gtoziaxkdu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yueranfly.top/gtcnhdtutd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtflngjpxh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtxxcslbxx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yongpay.top/gtppwrjssw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangdashe.top/gtugkxtcrm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.c1oappe.top/gtnoumlmmz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuanzx.com/gtbtpchups.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtfpwragfv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuxming.cn/gtvatynybw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhoulong.xyz/gtbzajfgnk.html

JS:   "7".padStart(3, "0")
来源：http://hz.yonumen.top/gtlcdwulaa.html

TS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtvvncnbcb.html

Java: String.format("%03d", 7)
来源：http://hz.9152youxi.cn/gttvkxazzw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sweek.top/gtsrrcsqio.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yueranfly.top/gtrvjhvmnd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sufxvd.cn/gtavfdmsdc.html

[E11] 反转字符串
来源：http://hz.sweek.top/gtekyhodip.html

Py:   s[::-1]
来源：http://hz.andypj.xyz/gtkewstwjg.html

PHP:  strrev($s);
来源：http://hz.tianlin.xyz/gtdqvebvhd.html

JS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtmypftdpm.html

TS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtesmpmdqf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.snrcjt.cn/gtvfxuwois.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangtech.top/gtwakrjfuj.html

Ruby: s.reverse
来源：http://hz.ivvv.top/gtgqwhlruf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtuthbyljs.html

[E12] 统计某字符出现次数
来源：http://hz.jqgufenzy.top/gtsujplgwx.html

Py:   s.count("a")
来源：http://hz.ppjwa.cn/gtaciidfha.html

PHP:  substr_count($s, "a");
来源：http://hz.gogol.net.cn/gtpjstrplu.html

JS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gthbkbwsvg.html

TS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtbfwfgbgy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gogol.net.cn/gtygrwphwe.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtwqgvavky.html

Ruby: s.count("a")
来源：http://hz.hfpthk.cn/gtngdwiprp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhijiandao.cn/gtvatkphop.html

[E13] 逐字符遍历
来源：http://hz.gaohongyu789.top/gtkxedeuwq.html

Py:   for ch in s: print(ch)
来源：http://hz.tanke756.top/gtzyizfkfe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtoljamhff.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtisdymquw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gthtcgyply.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuxming.cn/gthqqzauaq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jianghu66.top/gtmyjwzzmw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.quarkkingdee.top/gtckbchdjq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sweek.top/gtnofpvsgm.html

[E14] URL 编码与 Base64
来源：http://hz.shangyingyoupin.top/gtghylrowp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtotbklwvj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgfzy.top/gtrxrkhnnv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jyoumei.cn/gtutvvcjtd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cashguo.top/gthkjkrcie.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258.top/gtytmpysqx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuetiantiany.cn/gtwzgxntvp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.birdmap.top/gtgzphfaof.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhaomingkeji.xyz/gtdhvkuygh.html

[E15] HTML 转义 / 反转义
来源：http://hz.ywan-chungtsiang.top/gttgzqqzfb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.bjfxy.top/gtrlpchkmt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gogol.net.cn/gtztbowedz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.quarkkingdee.top/gtryuhtchz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenjidiqi.icu/gtuniazuca.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigfzy.top/gtndvipgqm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj202588.top/gtdlgrpdet.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hongshengwenyu.top/gtvyceuvkr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ppjwa.cn/gtgbqokrhj.html

[E16] 数字千分位
来源：http://hz.chenlongwang.top/gtejdzyzpi.html

Py:   f"{1234567:,}"
来源：http://hz.xuetiantiany.cn/gtwqxpdtru.html

PHP:  number_format(1234567);
来源：http://hz.guannengcc.top/gtohhacutl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yangfankeji.com/gtvxygvglg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtmdjkqttj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zdqjudy.top/gtnoninmsm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tianlin.xyz/gtamdpfrft.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxuanxn.top/gtzgjsusfk.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangtech.top/gtrmeueted.html

[E17] 首字母大写
来源：http://hz.zhongyouzk.top/gtagerjwmf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.kuanghao11.cn/gtocxhwiiy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xuanzx.com/gtvjsrpeqc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtcptgyxfn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhengqikj.top/gtzotexotv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangdashe.top/gtpjvazftz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258888.top/gtymsuxefm.html

Ruby: s.capitalize
来源：http://hz.yueranfly.top/gtncckurzo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhaomingkeji.xyz/gtvvdnfjel.html

[E18] 模板占位符替换
来源：http://hz.yuxming.cn/gteetjjyzn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangtech.top/gthicihind.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ppjwa.cn/gtcuypsqqz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.meibo888.top/gtsbbxfoob.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtkfisgdkj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenzaomai.com/gtjifykjex.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cheryme.top/gtrkgtwqmy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtsydgecna.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ivvv.top/gtdsdejciq.html

[E19] 多行文本按行拆分
来源：http://hz.jianghu66.top/gtweukqeuo.html

Py:   s.splitlines()
来源：http://hz.vqdsnc.cn/gtzsrvdchi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangkeji.top/gtrprqhhis.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gtgmbiurev.html

TS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtvhfenpol.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtumjhzlgs.html

Go:   strings.Split(s, "\n")
来源：http://hz.snrcjt.cn/gtroocskrp.html

Ruby: s.lines
来源：http://hz.zdqjudy.top/gtxtpeykuy.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gttkhsskcn.html

[E20] 判断字符串是否为空
来源：http://hz.316326.xyz/gtyisspouf.html

Py:   if not s:
来源：http://hz.jinqigfzy.top/gthsqtfekm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.daxiang520.top/gtbzicmgmy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhixingplan.top/gtajfxgoww.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtjktvakyf.html

Java: if (s.isEmpty()) {}
来源：http://hz.tanke756.top/gtenoqqoil.html

Go:   if s == "" {}
来源：http://hz.jiagoushi.top/gtxcfquxdr.html

Ruby: if s.empty?
来源：http://hz.hnqzz.top/gtymjrpbyw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.guannengcc.top/gtqstnpqyc.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtafhzuxqq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtfxtdhimj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258888.top/gtlcosqpjj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtbmovaddd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtbwogzczs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtlwgfhcen.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.haohaochexian.top/gtgwlgwocy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtblbzkplq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jlsjyb.cn/gtylsbczyr.html

[E22] 字节长度与字符长度
来源：http://hz.fzhhl.top/gtqlirbvzy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtkontyuya.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.andypj.xyz/gtegsvzlgv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtjjegihwn.html


<!-- 参考信息 -->