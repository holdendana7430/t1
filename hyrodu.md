代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guannengcc.top/gtktnzxhem.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hfpthk.cn/gtjkwrdems.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aibaodan.cn/gtqbuxdszt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xuanzx.com/gtcvsptrru.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shanyushiyangkeji.top/gtilgnxwjx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigfzy.top/gtpwpzazoi.html

JS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtczvyqsci.html

TS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtzgmzqqce.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dianchejie.cn/gtwsnuwfpo.html

Go:   // 手写循环
来源：http://hz.meibo888.top/gtmdpvproh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.kuanghao11.cn/gtcovclqjr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nwbrower.top/gtnvtisxky.html

[D15] 去重
来源：http://hz.jianghu66.top/gtyaegxkgp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtbmcynskg.html

PHP:  array_unique($arr);
来源：http://hz.chenzaomai.com/gtwjhsmume.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtowlylmak.html

TS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtkcwmyamk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dashuyun.cn/gtcyenomkb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.guowangkeji.top/gtbqdbxxrh.html

Ruby: arr.uniq
来源：http://hz.nanxinkj.top/gtwkaaogrj.html

C#:   list.Distinct().ToList()
来源：http://hz.shangyingyoupin.top/gtzkdvxbrt.html

[D16] 求和与平均值
来源：http://hz.jlsjyb.cn/gtcxvhafho.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258888.top/gtxkvfahee.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nwbrower.top/gtxzrsqcoy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtanunlcsc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtoqceelng.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sufxvd.cn/gtlhqzixfa.html

Go:   // 手写循环累加
来源：http://hz.kuanghao11.cn/gtovtbfykg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.vqdsnc.cn/gtzinxagwl.html

C#:   list.Sum();  list.Average()
来源：http://hz.yueranfly.top/gtmklhrkqa.html

[D17] 最大值与最小值
来源：http://hz.gaohongyu789.top/gtmsjnsfhe.html

Py:   max(arr);  min(arr)
来源：http://hz.ivvv.top/gtdyucvixe.html

PHP:  max($arr);  min($arr);
来源：http://hz.shuidangran.top/gthtacdfhc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtwcjhanir.html

TS:   Math.max(...arr);
来源：http://hz.shuidangran.top/gthzqrivhz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gaohongyu789.top/gtwvfoqejr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydjk.org.cn/gtvrekqlhi.html

Ruby: arr.max;  arr.min
来源：http://hz.pengpengdd.cyou/gtvaiecpdm.html

C#:   list.Max();  list.Min()
来源：http://hz.ydjk.org.cn/gtcarrepio.html

[D18] 扁平化嵌套数组
来源：http://hz.jinghuilouyu.cn/gtlkdeairb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shzxlz.cn/gtlzpfqaiq.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gtyrfrmjxo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.fzhhl.top/gtcqwineex.html

TS:   nested.flat();
来源：http://hz.snrcjt.cn/gtfsdlclgl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuanzhike.top/gtyxuqlfly.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtxkwzxgxq.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtbtwxqhgl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fzhhl.top/gtqekiqmva.html

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gtbifhannw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hysaishi.cn/gthrgybwcu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258888.top/gtltpmbyuy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.52xcode.cn/gtolvyupku.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gthtaxuanx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hfpthk.cn/gtyyxatzlt.html

Go:   // 手写 map[string][]T
来源：http://hz.zhaomingkeji.xyz/gtdoyabwkv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ehwqpu.com/gtalfosjvz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuetiantiany.cn/gtjbgrabvn.html

[D20] 统计每个元素出现次数
来源：http://hz.jyoumei.cn/gtjaxofklt.html

Py:   Counter(arr)
来源：http://hz.mhx1999.top/gtwfkrwwef.html

PHP:  array_count_values($arr);
来源：http://hz.feifeiyinyue.top/gtpfpekwfb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gzhubu.top/gtdhpxrbnl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yongpay.top/gtqozwclim.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgufenzy.top/gtnfamnoob.html

Go:   // 手写 map[T]int
来源：http://hz.zhixingplan.top/gtdzqbytug.html

Ruby: arr.tally
来源：http://hz.smart0.xyz/gtnplpvgrr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shuidangran.top/gtwttvudxs.html

[D21] 判断是否包含某元素
来源：http://hz.jiagoushi.top/gtdntocpup.html

Py:   x in arr
来源：http://hz.havefunace.top/gtkdcfgcyc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guowangkeji.top/gtsskvawdb.html

JS:   arr.includes(x)
来源：http://hz.cheryme.top/gtvizvzjxw.html

TS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtiybjylsr.html

Java: list.contains(x)
来源：http://hz.shuidangran.top/gtugdhlwwn.html

Go:   slices.Contains(arr, x)
来源：http://hz.birdmap.top/gtnhgikbww.html

Ruby: arr.include?(x)
来源：http://hz.zdqjudy.top/gttbmdzirf.html

C#:   list.Contains(x)
来源：http://hz.tian-w.cn/gtkkfpumxr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pycfn.com/gtytdjcuuu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.havefunace.top/gtmfpiyuwh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhixingplan.top/gtqsfhcaaf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinqigufen.top/gtlidphebh.html

TS:   [...arr];
来源：http://hz.xylfe.cn/gthbgcipgr.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtjkgqfzcn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jyoumei.cn/gtitymwkse.html

Ruby: arr.dup;  arr.clone
来源：http://hz.svipenyu.cn/gtukdlytux.html

C#:   new List<int>(list);
来源：http://hz.guannengcc.top/gtxlorjijd.html

[D23] reduce 累积计算
来源：http://hz.hysaishi.cn/gtugwojyqe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtxftszdpg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tanke756.top/gtkwbzysds.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtbotluhrn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtvhozgeac.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yonumen.top/gtphtnpzzm.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtdgprepyw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhiwuduotai.top/gtygrladoq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.pengpengdd.cyou/gtmhurembw.html

[D24] 字典 / Map 基本操作
来源：http://hz.birdmap.top/gtiftjqari.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sufxvd.cn/gtsonpezlw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hfpthk.cn/gtbspjrsvi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.pengpengdd.cyou/gtajiyhqdz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hysaishi.cn/gtcquvjipl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinqigfzy.top/gtswbyeurs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtiezxlcgu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.smart0.xyz/gtinjdenzo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtmmxiovxg.html

[D25] Set 集合去重与交并差
来源：http://hz.9152youxi.cn/gtmzgovajk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guannengcc.top/gtpjostkds.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenjidiqi.icu/gtilcmuhqk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yanxiufei.cn/gtmycsrrnp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cucudq.cn/gtnvtyyitd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.smart0.xyz/gtxruztiak.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtockwshfg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ppjwa.cn/gtmguiljqk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgfzy.top/gtyrqjhbzv.html

[D26] 数组转字符串
来源：http://hz.cucudq.cn/gtdvgnxhop.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hysaishi.cn/gtmdwpnhtv.html

PHP:  implode(", ", $arr);
来源：http://hz.birdmap.top/gtkqfvxuhs.html

JS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtifiwxovs.html

TS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtxcysxomf.html

Java: String.join(", ", list)
来源：http://hz.gaohongyu789.top/gtlngcxwon.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ivvv.top/gtvzrpyxdq.html

Ruby: arr.join(", ")
来源：http://hz.cucudq.cn/gthpetzebn.html

C#:   string.Join(", ", list)
来源：http://hz.guannengcc.top/gtzxgowlcx.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtyqrbvsnf.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gtxbbqadnu.html

================================================================================
来源：http://hz.hysaishi.cn/gtcvljaxwp.html

[E01] 拼接字符串
来源：http://hz.hysaishi.cn/gtbiuinzbp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.iojbl.cn/gtlkoytakl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangkeji.top/gtzbolvdqs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gtopieuiqd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtrdtvqxwm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.aibaodan.cn/gtojrhyjud.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fzhhl.top/gtyfiqmtli.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ywan-chungtsiang.top/gtuyvqaiux.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tanke756.top/gtznnqcdnl.html

[E02] 重复字符串
来源：http://hz.aizwys.cn/gttectuyib.html

Py:   "ab" * 3
来源：http://hz.cashguo.top/gtwpmdiqpl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sysykeji.top/gtkleyrfhr.html

JS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gtfuohuqub.html

TS:   "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtzdlpptnn.html

Java: "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtrwjtvltl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.feifeiyinyue.top/gtmdktxknf.html

Ruby: "ab" * 3
来源：http://hz.yonumen.top/gthhjwojxx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhixingplan.top/gtuugescxl.html

[E03] 截取子串
来源：http://hz.ybcxt.top/gtfczejwae.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ivvv.top/gtnyxljrgj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.wangdashe.top/gtjawlcicb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtpkzncnre.html

TS:   s.slice(1, 4)
来源：http://hz.shuidangran.top/gtaavrghjc.html

Java: s.substring(1, 4)
来源：http://hz.yj20258888.top/gtjyudqhrt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cheryme.top/gtwzzvahvl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cashguo.top/gtsyrwmciw.html

C#:   s.Substring(1, 3)
来源：http://hz.316326.xyz/gthzuscbrl.html

[E04] 查找子串位置
来源：http://hz.tianlin.xyz/gtdytleyts.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yangfankeji.com/gtpzgdntgy.html

PHP:  strpos($s, "x");
来源：http://hz.vqdsnc.cn/gtsqmjqyih.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.chenzaomai.com/gtxlcaudpj.html

TS:   s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtvsthckuh.html

Java: s.indexOf("x")
来源：http://hz.cdnleiting.top/gtjtuakuvf.html

Go:   strings.Index(s, "x")
来源：http://hz.gotoacloud.top/gtrulsmyvm.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtjvoicyih.html

C#:   s.IndexOf("x")
来源：http://hz.yj20258888.top/gtpuzgsoxk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shanyushiyangkeji.top/gtstbbvxsc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yueranfly.top/gtbappyvtg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ppjwa.cn/gtqtkzrbje.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtgpbazxim.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zdqjudy.top/gtsfnefhtl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtfzcrkiyk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtwpjjkbtm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtviibpcju.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jlsjyb.cn/gtpfcfpbpg.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtuwcskctp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hnxiangtu.top/gtwbgidloy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.andypj.xyz/gtgwynrqys.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtopooruin.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtbvyfikso.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtpfqevhpr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuanzx.com/gtyogiublo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.daria6918.cn/gtndzaehqq.html

C#:   s.Replace("a", "b")
来源：http://hz.cashguo.top/gtylbxqdhh.html

[E07] 按分隔符拆分
来源：http://hz.guannengcc.top/gttrhxgdpe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.birdmap.top/gtadubphrt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.9152youxi.cn/gtclcswhqn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tian-w.cn/gtvtynjgcg.html

TS:   s.split(",")
来源：http://hz.gogol.net.cn/gtglhmzpjg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hywenlv.cn/gtmlkbnuef.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxuanxn.top/gtqpjcqqxy.html

Ruby: s.split(",");  s.split
来源：http://hz.gaohongyu789.top/gtattfekpe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dashuyun.cn/gticdeyczh.html

[E08] 数组按分隔符合并
来源：http://hz.quarkkingdee.top/gtfwomuhia.html

Py:   ",".join(items)
来源：http://hz.gotoacloud.top/gtiosakttp.html

PHP:  implode(",", $items);
来源：http://hz.sweek.top/gtqkbpogff.html

JS:   items.join(",")
来源：http://hz.hnxiangtu.top/gtooeahzpl.html

TS:   items.join(",")
来源：http://hz.ppjwa.cn/gtdafselkr.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtmlmxpkpo.html

Go:   strings.Join(items, ",")
来源：http://hz.meibo888.top/gtixjgzdpc.html

Ruby: items.join(",")
来源：http://hz.haohaochexian.top/gtzobipbnm.html

C#:   string.Join(",", items)
来源：http://hz.yj20258888.top/gtginikyog.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtgymbmqkl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhongyouzk.top/gteosuqapb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jlsjyb.cn/gtlnbjtryv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gthytnvuxh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.smart0.xyz/gtdnoutszg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hfpthk.cn/gtfqykkbbu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tianlin.xyz/gtdepehsjo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ppjwa.cn/gtptjwilfv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gtxzyawlml.html

[E10] 左侧补零 / 定长填充
来源：http://hz.daxiang520.top/gtajrfggni.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shangyingyoupin.top/gtuhhmcrhd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hywenlv.cn/gtvikysvad.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtsplbggtw.html

TS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtaigqdmle.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtbbefcpns.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258888.top/gtlfziozmu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtuikkgvwg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cucudq.cn/gtobvjrgmf.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtisgbkvxm.html

Py:   s[::-1]
来源：http://hz.tian-w.cn/gtxhdvmjjw.html

PHP:  strrev($s);
来源：http://hz.gzhubu.top/gtmcarapxq.html

JS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtdelrkzeo.html

TS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtzlcjqhyj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.mhx1999.top/gtnemhdguk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gaohongyu789.top/gtudnuprbi.html

Ruby: s.reverse
来源：http://hz.chenjidiqi.icu/gtngctkuvg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtakbhppej.html

[E12] 统计某字符出现次数
来源：http://hz.jqgfzy.top/gtpwmyqymu.html

Py:   s.count("a")
来源：http://hz.nanxuanxn.top/gtcbhpnobl.html

PHP:  substr_count($s, "a");
来源：http://hz.shangyingyoupin.top/gtouagyuzx.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtdablbhit.html

TS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtpqoedznj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhaomingkeji.xyz/gtxjujjpac.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258.top/gtxcojfkgv.html

Ruby: s.count("a")
来源：http://hz.andypj.xyz/gtiksprfyi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.fengsongda.top/gtfvyebwgf.html

[E13] 逐字符遍历
来源：http://hz.zycfv.cn/gtvyfstpat.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxuanxn.top/gtdvwvzpnx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigfzy.top/gtxxdkazim.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gttnzupkjv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtqbdhzxaj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ybcxt.top/gtvxjarcrc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cashguo.top/gtdjgnnytm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgufenzy.top/gtjyrldmlx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yangfankeji.com/gtqxtmjdwo.html

[E14] URL 编码与 Base64
来源：http://hz.gzhubu.top/gtmnwglztf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj202588.top/gtjlrxcide.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydjk.org.cn/gttfwuucgq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.9152youxi.cn/gtjxxenhqg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.52xcode.cn/gtlbfjhume.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daxiang520.top/gtglbkpzak.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.iojbl.cn/gtcyhlnyzr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangshuangyany.cn/gtytsofejh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhijiandao.cn/gtocoaqvrz.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtonrfrtmg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yueranfly.top/gtzfzvoboj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tianlin.xyz/gtxsldqahu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.smart0.xyz/gtvncbkujd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gtbdwhnqby.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinghuilouyu.cn/gtmxfxgosr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.bjfxy.top/gtfeotavik.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daria6918.cn/gttparzndd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shuidangran.top/gtgwfhobwy.html

[E16] 数字千分位
来源：http://hz.c1oappe.top/gtnwzgyugj.html

Py:   f"{1234567:,}"
来源：http://hz.jianghu66.top/gtweaisblc.html

PHP:  number_format(1234567);
来源：http://hz.meibo888.top/gteddossju.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gttizruiub.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtuvllyxbk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daria6918.cn/gtsbkqxpbv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jiagoushi.top/gtuujfzpqb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gtpvvpmjor.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgfzy.top/gtacahpamb.html

[E17] 首字母大写
来源：http://hz.zhongyouzk.top/gtdlwadlyv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gtckxcbeaa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shanyushiyangtech.top/gtsfomsbdd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtewgpvoci.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtzcemuvjj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gtderfdsuh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pycfn.com/gtenbcyznv.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtzzakyucw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jqgufenzy.top/gtqyetslbs.html

[E18] 模板占位符替换
来源：http://hz.hammf.cn/gtvxviuszt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nanxinkj.top/gtmrbbrglb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jianghu66.top/gtylwrpmpw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gthtmbpvar.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zdqjudy.top/gtuiylbeth.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cashguo.top/gtjucoequj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigfzy.top/gtfgppjons.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gtwkrmirif.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hammf.cn/gtdpuqicaz.html

[E19] 多行文本按行拆分
来源：http://hz.tian-w.cn/gtozhxdiay.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtzxinyhse.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ivvv.top/gtgjbkakmf.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtsqiyeyek.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gthyyxbopj.html

Java: s.lines().toList()
来源：http://hz.316326.xyz/gtpquchudv.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtqeaclhms.html

Ruby: s.lines
来源：http://hz.andypj.xyz/gtsuukjglf.html

C#:   s.Split('\n')
来源：http://hz.yvedp.cn/gtmwcqukwp.html

[E20] 判断字符串是否为空
来源：http://hz.dashuyun.cn/gtjncopoaa.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gttpykagoq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.smart0.xyz/gtmxkxledb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxuanxn.top/gtoqthlauz.html

TS:   if (s === "") {}
来源：http://hz.tianlin.xyz/gtzlgzipir.html

Java: if (s.isEmpty()) {}
来源：http://hz.zdqjudy.top/gtfginzrac.html


<!-- 参考信息 -->