代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xingfuxueyuan.xyz/gtbwdovvbn.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gthatwwolk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhiwuduotai.top/gtkzncbrzy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yj202588.top/gtptgxvdwd.html

[D15] 去重
来源：http://hz.xuanzx.com/gtaainwflh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.aizwys.cn/gtlinhiznx.html

PHP:  array_unique($arr);
来源：http://hz.feifeiyinyue.top/gtvrdsiqqc.html

JS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtdgyedcjt.html

TS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtnwtfimrm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sysykeji.top/gtzplxpehk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.vqdsnc.cn/gtbdvsjkmq.html

Ruby: arr.uniq
来源：http://hz.pycfn.com/gtmkhdmxzz.html

C#:   list.Distinct().ToList()
来源：http://hz.xingfuxueyuan.xyz/gtlwlkhbxs.html

[D16] 求和与平均值
来源：http://hz.yonumen.top/gtxzhwpqmb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.quarkkingdee.top/gtoilxgnyr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jianghu66.top/gtwzthetxw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtqifgncut.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gttldyfdsx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cheryme.top/gtpgokbdrs.html

Go:   // 手写循环累加
来源：http://hz.shzxlz.cn/gtgobcwwvs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258888.top/gtvcyludpm.html

C#:   list.Sum();  list.Average()
来源：http://hz.9152youxi.cn/gtyncprxzi.html

[D17] 最大值与最小值
来源：http://hz.chenlongwang.top/gtyhptijky.html

Py:   max(arr);  min(arr)
来源：http://hz.yonumen.top/gtbrkxcmjf.html

PHP:  max($arr);  min($arr);
来源：http://hz.hammf.cn/gtriujzwwy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yangfankeji.com/gtwyxpbvwg.html

TS:   Math.max(...arr);
来源：http://hz.quarkkingdee.top/gtdiyoipxx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sxryk.cn/gtfdelprcc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.quarkkingdee.top/gtkqvcjjtu.html

Ruby: arr.max;  arr.min
来源：http://hz.pengpengdd.cyou/gtqzjtdinu.html

C#:   list.Max();  list.Min()
来源：http://hz.zhaomingkeji.xyz/gtmgirebjo.html

[D18] 扁平化嵌套数组
来源：http://hz.xziqi.cn/gtduxgaywq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.316326.xyz/gtnwoilnos.html

PHP:  array_merge(...$nested);
来源：http://hz.tian-w.cn/gtsxijyfjc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ehwqpu.com/gtwcyrzrtn.html

TS:   nested.flat();
来源：http://hz.pycfn.com/gtpiltyoqj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guannengcc.top/gtkxgxmzpg.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtygjtaxor.html

Ruby: nested.flatten
来源：http://hz.hnxiangtu.top/gtmkahxsct.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zycfv.cn/gtxrgohwvq.html

[D19] 按字段分组
来源：http://hz.xziqi.cn/gtcknymawv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.svipenyu.cn/gtwpylnfnq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gtbkzkfxcg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.snrcjt.cn/gtxvorstpa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtljrxnwed.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgfzy.top/gtprhzuzwp.html

Go:   // 手写 map[string][]T
来源：http://hz.shzxlz.cn/gtwllfqmac.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgufenzy.top/gtcsrzrokr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sufxvd.cn/gtyblvydtm.html

[D20] 统计每个元素出现次数
来源：http://hz.zhijiandao.cn/gtftnzgxcu.html

Py:   Counter(arr)
来源：http://hz.dianchejie.cn/gtovkcowbx.html

PHP:  array_count_values($arr);
来源：http://hz.chenjidiqi.icu/gtjnfxmdfd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtibgronca.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtmutqgtyt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yanxiufei.cn/gtkvgaphos.html

Go:   // 手写 map[T]int
来源：http://hz.svipenyu.cn/gtlfprvaxc.html

Ruby: arr.tally
来源：http://hz.dashuyun.cn/gtfjngpamw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hfpthk.cn/gtdchaipkx.html

[D21] 判断是否包含某元素
来源：http://hz.guannengcc.top/gtouwjujby.html

Py:   x in arr
来源：http://hz.chenlongwang.top/gtstvgpozu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daria6918.cn/gtsegxbise.html

JS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtegltxclw.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtskmclqsz.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtnnitkkih.html

Go:   slices.Contains(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtthawyagl.html

Ruby: arr.include?(x)
来源：http://hz.tanke756.top/gtlbckufzv.html

C#:   list.Contains(x)
来源：http://hz.ivvv.top/gtvxkazkwo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gtadwzrboy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnqzz.top/gtocvisnxp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhaomingkeji.xyz/gtnudwcxod.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gotoacloud.top/gtyeomupvs.html

TS:   [...arr];
来源：http://hz.zycfv.cn/gtvpcwbsmx.html

Java: new ArrayList<>(list);
来源：http://hz.snrcjt.cn/gtthfcoyvs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yueranfly.top/gttgrsmobx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhiwuduotai.top/gtaxyplxer.html

C#:   new List<int>(list);
来源：http://hz.jyoumei.cn/gtmuewbcyt.html

[D23] reduce 累积计算
来源：http://hz.cdnleiting.top/gtwgdkflpc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenzaomai.com/gtftznlrer.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxinkj.top/gtbhfziymu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtnegpkrbe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtjwzhgkog.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nwbrower.top/gtobpbwoue.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gttcczgchg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cheryme.top/gtkaeaybnr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuanzx.com/gtxjloozrt.html

[D24] 字典 / Map 基本操作
来源：http://hz.fengsongda.top/gtxogrlykj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gogol.net.cn/gthunlgewi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhiwuduotai.top/gtepbskbap.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnxiangtu.top/gtfwumcdso.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtrvqcqobe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.aibaodan.cn/gtxulynucd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nwbrower.top/gtutnixbbx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yanxiufei.cn/gtgwakbvgm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuanzx.com/gtpbbjhuaf.html

[D25] Set 集合去重与交并差
来源：http://hz.cucudq.cn/gtsblsptud.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sysykeji.top/gtepqxwxsl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gtiwinwfpk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shanyushiyangkeji.top/gtrnobbzgh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.bjfxy.top/gteuknrzkg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.quarkkingdee.top/gtimnjewzg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ivvv.top/gtqqcfucgb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxuanxn.top/gtsytapyoo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.smart0.xyz/gtqqvikvzs.html

[D26] 数组转字符串
来源：http://hz.yj202588.top/gtrsqoogpw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aizwys.cn/gticjdpktq.html

PHP:  implode(", ", $arr);
来源：http://hz.mhx1999.top/gtkeakmfwh.html

JS:   arr.join(", ")
来源：http://hz.gzhubu.top/gtevffksgd.html

TS:   arr.join(", ")
来源：http://hz.vqdsnc.cn/gtbrgpxeyd.html

Java: String.join(", ", list)
来源：http://hz.xinyue.icu/gtwctjrpyl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.snrcjt.cn/gthfinnmhc.html

Ruby: arr.join(", ")
来源：http://hz.tianlin.xyz/gtunvjnivs.html

C#:   string.Join(", ", list)
来源：http://hz.sufxvd.cn/gtivyjqxml.html

================================================================================
来源：http://hz.nanxuanxn.top/gteyqdcxjz.html

E. 字符串处理
来源：http://hz.redwolf501.top/gtzeyiwpdm.html

================================================================================
来源：http://hz.aibaodan.cn/gtuqgsxoyq.html

[E01] 拼接字符串
来源：http://hz.sufxvd.cn/gtuueeoluo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.birdmap.top/gticiruxwh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cashguo.top/gtkjirfiul.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.52xcode.cn/gtvqnbskhg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtpdahxdhe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hywenlv.cn/gthjblhzsa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinyuanbaomall.cn/gtidobyrtu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydzc1.top/gttmmbnsip.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.kuanghao11.cn/gtrlwsrzot.html

[E02] 重复字符串
来源：http://hz.shanyushiyangtech.top/gtvdzicich.html

Py:   "ab" * 3
来源：http://hz.hywenlv.cn/gtgdhkkllg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenjidiqi.icu/gtauoiaslz.html

JS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gthklebpvn.html

TS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtchgqvwus.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtrffcwylz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.dianchejie.cn/gtlqlzfzbx.html

Ruby: "ab" * 3
来源：http://hz.cheryme.top/gturjzldcx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuanzx.com/gtrxtxajvz.html

[E03] 截取子串
来源：http://hz.xziqi.cn/gthnkebpoa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258.top/gtagwfvbdu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ybcxt.top/gtizngjfra.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtzsjausla.html

TS:   s.slice(1, 4)
来源：http://hz.xuanzx.com/gtssvkldqw.html

Java: s.substring(1, 4)
来源：http://hz.ydzc1.top/gtowetziil.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sufxvd.cn/gttavjfmje.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.vqdsnc.cn/gtqxtnnbne.html

C#:   s.Substring(1, 3)
来源：http://hz.sysykeji.top/gtlvgchizk.html

[E04] 查找子串位置
来源：http://hz.pycfn.com/gtpejnpmzx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.pycfn.com/gtmujdebdx.html

PHP:  strpos($s, "x");
来源：http://hz.hongshengwenyu.top/gtzxincoxz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258.top/gtiswuflzq.html

TS:   s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtozwmbpbz.html

Java: s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtlvppffhv.html

Go:   strings.Index(s, "x")
来源：http://hz.hnxiangtu.top/gtumbghuhs.html

Ruby: s.index("x")
来源：http://hz.yangfankeji.com/gtedsgviso.html

C#:   s.IndexOf("x")
来源：http://hz.52xcode.cn/gtplbdphuu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydjk.org.cn/gtrjpgkjvq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.meibo888.top/gtszpdtbqq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dashuyun.cn/gtfrrzlcsj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtgoowyzte.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.dianchejie.cn/gtwxmzesyg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtmkwieaif.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hongshengwenyu.top/gtvxylmxsc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.wangdashe.top/gtylowfbsx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shanyushiyangtech.top/gtroffzcoo.html

[E06] 替换子串
来源：http://hz.xinyue.icu/gtdkdradmp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jyoumei.cn/gtllmeqrcx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xylfe.cn/gtgohdolrs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtqlznufau.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtmxviipwi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtenmivyxb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gtuorhlddy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zdqjudy.top/gtssfbxuft.html

C#:   s.Replace("a", "b")
来源：http://hz.zdqjudy.top/gtwssjmyas.html

[E07] 按分隔符拆分
来源：http://hz.cucudq.cn/gtrnxlsafa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hywenlv.cn/gtwrlhnzcs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.316326.xyz/gtotgclllh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jlsjyb.cn/gtoyjdvcqw.html

TS:   s.split(",")
来源：http://hz.zycfv.cn/gtjqzeotyt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sysykeji.top/gtjcnmtvyv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj202588.top/gtqvdjszin.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258.top/gtehvtkpbv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtvdezivtp.html

[E08] 数组按分隔符合并
来源：http://hz.tanke756.top/gtrksitqyx.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gtqinsonbv.html

PHP:  implode(",", $items);
来源：http://hz.gotoacloud.top/gtcsebrguf.html

JS:   items.join(",")
来源：http://hz.zdqjudy.top/gtbdytqrwy.html

TS:   items.join(",")
来源：http://hz.zdqjudy.top/gtourqjiuv.html

Java: String.join(",", items)
来源：http://hz.0kj1m.cn/gtnspkguvk.html

Go:   strings.Join(items, ",")
来源：http://hz.xuetiantiany.cn/gtggwsndbv.html

Ruby: items.join(",")
来源：http://hz.hammf.cn/gtwfknmtai.html

C#:   string.Join(",", items)
来源：http://hz.yvedp.cn/gtwcvqueiu.html

[E09] 去除所有空白字符
来源：http://hz.jinghuilouyu.cn/gtlxvvbeek.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cucudq.cn/gtpjfckfuc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tanke756.top/gtbxraphnr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.kuanghao11.cn/gtexginmhr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gthecavjao.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigufen.top/gtbsnjowjk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daxiang520.top/gtxxwvocly.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xingfuxueyuan.xyz/gtczbxqbhp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nanxinkj.top/gtioovzwfy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dianchejie.cn/gtqugnhera.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.aibaodan.cn/gtcaktjkwu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.bjfxy.top/gtyqcexypd.html

JS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtfbqeixqo.html

TS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtuljisfqx.html

Java: String.format("%03d", 7)
来源：http://hz.hysaishi.cn/gtaxhpaoif.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.52xcode.cn/gttpxeywdn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dashuyun.cn/gticgmprwk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yueranfly.top/gtvunuirtx.html

[E11] 反转字符串
来源：http://hz.hfpthk.cn/gtbnljpdzy.html

Py:   s[::-1]
来源：http://hz.daria6918.cn/gtpzofbfja.html

PHP:  strrev($s);
来源：http://hz.pycfn.com/gtehgpcols.html

JS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtblfggrbe.html

TS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtermmisbf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tian-w.cn/gtpwxbeqvp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.kuanghao11.cn/gtvtzoktwg.html

Ruby: s.reverse
来源：http://hz.cdnleiting.top/gtjbvevyrg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtjqnmnxam.html

[E12] 统计某字符出现次数
来源：http://hz.hnxiangtu.top/gtfqkaaksz.html

Py:   s.count("a")
来源：http://hz.tanke756.top/gtsvcqyamz.html

PHP:  substr_count($s, "a");
来源：http://hz.guowangkeji.top/gtlewzrwac.html

JS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtjhhnccnx.html

TS:   s.split("a").length - 1
来源：http://hz.sufxvd.cn/gthclkntse.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnqzz.top/gtcxfxzbjw.html

Go:   strings.Count(s, "a")
来源：http://hz.yj202588.top/gttjlegkro.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gtthhvbmfc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhengqikj.top/gtdkkdxfct.html

[E13] 逐字符遍历
来源：http://hz.wangshuangyany.cn/gtclqunaif.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258.top/gtqjahvait.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinghuilouyu.cn/gtoidbtmjp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenjidiqi.icu/gtmawvlvni.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cucudq.cn/gtxlyegaus.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guannengcc.top/gtakmyixml.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hfpthk.cn/gtdohzmsyq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenzaomai.com/gtuqiuevgw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jyoumei.cn/gtcujpcnrw.html

[E14] URL 编码与 Base64
来源：http://hz.pengpengdd.cyou/gtavseqqmt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtfdqwtsjt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ppjwa.cn/gtbvqbmflr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shuidangran.top/gtqhxgjmqk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cucudq.cn/gtmhwoijoq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yanxiufei.cn/gtdqueugqp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jiagoushi.top/gtaczfjifs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.meibo888.top/gtzdcasxsp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinqigufen.top/gtmnkuahhe.html

[E15] HTML 转义 / 反转义
来源：http://hz.cucudq.cn/gtrelnulti.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.fzhhl.top/gtnrigwmgl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gaohongyu789.top/gtjsbstfbw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtsgianbpw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hongshengwenyu.top/gtutmjfvjq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aizwys.cn/gthuyolrut.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtawwzavel.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangdashe.top/gtvpbbftmo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuanzx.com/gtzbubjajw.html

[E16] 数字千分位
来源：http://hz.yj20258.top/gtubmnbpex.html

Py:   f"{1234567:,}"
来源：http://hz.tanke756.top/gtmufleqlx.html

PHP:  number_format(1234567);
来源：http://hz.sweek.top/gtyayrwkep.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtbijpqtii.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtwfudizih.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gogol.net.cn/gtausxhocb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shanyushiyangkeji.top/gtogsssndg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shzxlz.cn/gtvvqgqsxy.html

C#:   1234567.ToString("N0")
来源：http://hz.smart0.xyz/gtbkxogxhv.html

[E17] 首字母大写
来源：http://hz.hnxiangtu.top/gtdhsthiqx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenjidiqi.icu/gtdmvxpagn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sweek.top/gtbexjvcdl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtqagqnfyo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgufenzy.top/gtxrysnpdg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xziqi.cn/gtfpnnaotr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuanzhike.top/gtnnkfbekv.html

Ruby: s.capitalize
来源：http://hz.pengpengdd.cyou/gtcrsnvcdg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gtyjaijygm.html

[E18] 模板占位符替换
来源：http://hz.hnqzz.top/gtqyadxyhy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tianlin.xyz/gtjvgjjrvk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtxllmoqwd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtzyiwhdeh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gttkqhmgnw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.haohaochexian.top/gtxaskucnj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgufenzy.top/gtehrtdmeg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daria6918.cn/gtioxbkmzb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.svipenyu.cn/gtwagoxgmg.html

[E19] 多行文本按行拆分
来源：http://hz.nanxinkj.top/gtfkniprzx.html

Py:   s.splitlines()
来源：http://hz.9152youxi.cn/gttkxpdnqx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aibaodan.cn/gtdmieumfh.html

JS:   s.split(/\r?\n/)
来源：http://hz.fengsongda.top/gtjlnmakjj.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtjhvdclwm.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gthrdpyaor.html

Go:   strings.Split(s, "\n")
来源：http://hz.ywan-chungtsiang.top/gtnkghitcs.html

Ruby: s.lines
来源：http://hz.sysykeji.top/gtjxowejjj.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gtawwnplko.html

[E20] 判断字符串是否为空
来源：http://hz.pengpengdd.cyou/gthmwumyud.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtaazaigaf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtdetjvscr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.quarkkingdee.top/gtleoievgp.html

TS:   if (s === "") {}
来源：http://hz.xziqi.cn/gtgwjasadn.html

Java: if (s.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtjzqmkzsa.html

Go:   if s == "" {}
来源：http://hz.cdnleiting.top/gtwdplhazo.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gttdirsmrm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydjk.org.cn/gtimybkvsh.html

[E21] 超长截断加省略号
来源：http://hz.chenlongwang.top/gttjlfnkau.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.meibo888.top/gtvnvzvfxt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zdqjudy.top/gtyrtlgpty.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtxveaiyzy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtmcsuggkl.html


<!-- 参考信息 -->