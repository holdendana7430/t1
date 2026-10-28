代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guannengcc.top/gtdduyzaui.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtjwawlalf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangkeji.top/gtzerghjed.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shzxlz.cn/gtuwfsmibv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gotoacloud.top/gtswemxuvb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jiagoushi.top/gtvfosdrbs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hysaishi.cn/gtfkheiawa.html

[D14] 映射转换（每个元素变形）
来源：http://hz.9152youxi.cn/gtfenvqczl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.316326.xyz/gtusatxkjo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fzhhl.top/gtjavgqllt.html

JS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtkqvecpxg.html

TS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtmrpztbao.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fzhhl.top/gtomxwyjir.html

Go:   // 手写循环
来源：http://hz.cucudq.cn/gtywxeyjgp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtnkytguho.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenlongwang.top/gtgeksouxq.html

[D15] 去重
来源：http://hz.chenzaomai.com/gtyakiyjwk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yj20258.top/gtwihhaaql.html

PHP:  array_unique($arr);
来源：http://hz.meibo888.top/gtumtjouih.html

JS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtlkfkypgl.html

TS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtxkhwoxiw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daria6918.cn/gtzwbsuxqx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhijiandao.cn/gtamralkag.html

Ruby: arr.uniq
来源：http://hz.hfpthk.cn/gtxotscqsw.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gtxbfblaci.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gtnygmonwt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gtzcjsqjdo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hfpthk.cn/gtzyetmzaa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtfkltcbvl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtvsmedjip.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tanke756.top/gtirmmhyjk.html

Go:   // 手写循环累加
来源：http://hz.andypj.xyz/gtnsmvvnlr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258888.top/gtxvljnylz.html

C#:   list.Sum();  list.Average()
来源：http://hz.kuanghao11.cn/gtqrhvhgus.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtmaddyqii.html

Py:   max(arr);  min(arr)
来源：http://hz.cdnleiting.top/gtlisdfvzf.html

PHP:  max($arr);  min($arr);
来源：http://hz.nwbrower.top/gtzramxvcz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258.top/gtsymxajvw.html

TS:   Math.max(...arr);
来源：http://hz.quarkkingdee.top/gtsljseiwx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cdnleiting.top/gteflizyov.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnxiangtu.top/gtkcnchjvp.html

Ruby: arr.max;  arr.min
来源：http://hz.pycfn.com/gtdkjvbzfn.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gthwpdisyf.html

[D18] 扁平化嵌套数组
来源：http://hz.ydzc1.top/gtboasnmev.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gtmlfrhzux.html

PHP:  array_merge(...$nested);
来源：http://hz.chenlongwang.top/gtcckopwyt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtqefurhql.html

TS:   nested.flat();
来源：http://hz.zhaomingkeji.xyz/gtniwiktuy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtmhumzjjj.html

Go:   // 手写双层循环
来源：http://hz.zdqjudy.top/gtjbjaotqd.html

Ruby: nested.flatten
来源：http://hz.ywan-chungtsiang.top/gtisvgdfdw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hfpthk.cn/gtywilbrzh.html

[D19] 按字段分组
来源：http://hz.yueranfly.top/gthckxcest.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhoulong.xyz/gtqqdivgxg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.snrcjt.cn/gtewqpsumy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtvnojdgen.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtazfrkyga.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yonumen.top/gthrftjahp.html

Go:   // 手写 map[string][]T
来源：http://hz.cashguo.top/gtmtumqwie.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.mhx1999.top/gtchnjmekt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.haohaochexian.top/gtsipvqoom.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgfzy.top/gttssxokgy.html

Py:   Counter(arr)
来源：http://hz.cdnleiting.top/gtwdcvnwdg.html

PHP:  array_count_values($arr);
来源：http://hz.smart0.xyz/gtsfsadjyx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gtsyqujqzv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gaohongyu789.top/gtliqrlmur.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.meibo888.top/gtzruyycbk.html

Go:   // 手写 map[T]int
来源：http://hz.ydjk.org.cn/gtinvdobtg.html

Ruby: arr.tally
来源：http://hz.hywenlv.cn/gtvymxctjg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenzaomai.com/gtdrofycwc.html

[D21] 判断是否包含某元素
来源：http://hz.zhengqikj.top/gtqhrrnsqt.html

Py:   x in arr
来源：http://hz.haohaochexian.top/gtsaplcblx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hammf.cn/gtdnrsgnvf.html

JS:   arr.includes(x)
来源：http://hz.pycfn.com/gtoymjfzku.html

TS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtorwbdyeg.html

Java: list.contains(x)
来源：http://hz.jqgfzy.top/gthpwdpwec.html

Go:   slices.Contains(arr, x)
来源：http://hz.aibaodan.cn/gthpcyywfl.html

Ruby: arr.include?(x)
来源：http://hz.yonumen.top/gtdndxoaof.html

C#:   list.Contains(x)
来源：http://hz.chenlongwang.top/gtysfzlekc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtcekqjend.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cdnleiting.top/gtzhfatfwf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yueranfly.top/gthmrivikg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinqigfzy.top/gtxpawdyjy.html

TS:   [...arr];
来源：http://hz.mhx1999.top/gtwycivvlk.html

Java: new ArrayList<>(list);
来源：http://hz.zhoulong.xyz/gtoslyjjxv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cucudq.cn/gtntjndwri.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guowangkeji.top/gtokdagmyu.html

C#:   new List<int>(list);
来源：http://hz.gzhubu.top/gtscvndlyn.html

[D23] reduce 累积计算
来源：http://hz.zhaomingkeji.xyz/gtkhqfajws.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.c1oappe.top/gttmsbdqzt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhaomingkeji.xyz/gtjjtwnuwu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258.top/gtmmbvmfuq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gtotonecob.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxuanxn.top/gtrhezglvt.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gtadyfdooo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ydzc1.top/gtgmjrlmfl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xinyue.icu/gtvykbausy.html

[D24] 字典 / Map 基本操作
来源：http://hz.shzxlz.cn/gteqogawdu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xingfuxueyuan.xyz/gtecngwtre.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.fzhhl.top/gtjgwlcwia.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgufenzy.top/gtuovbhkjm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.pengpengdd.cyou/gtmjdoyhyv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydzc1.top/gtdkimrpsh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.aibaodan.cn/gtdlblwaug.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sufxvd.cn/gthmtofxso.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnqzz.top/gtjtnsatqy.html

[D25] Set 集合去重与交并差
来源：http://hz.bjfxy.top/gtbswuxxjf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.meibo888.top/gtrrfjglke.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxinkj.top/gtjwhgviri.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhiwuduotai.top/gtjtmzelbk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cheryme.top/gtemqvkcgu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxinkj.top/gthkaajcrq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.iojbl.cn/gtuphcphmc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtcnclvtgj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.redwolf501.top/gtgyffrkgq.html

[D26] 数组转字符串
来源：http://hz.zhaomingkeji.xyz/gthwrunbxl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.feifeiyinyue.top/gticpyzmbo.html

PHP:  implode(", ", $arr);
来源：http://hz.yj202588.top/gtigdmxwhf.html

JS:   arr.join(", ")
来源：http://hz.tanke756.top/gtjfyukvlu.html

TS:   arr.join(", ")
来源：http://hz.aizwys.cn/gthdcafqkw.html

Java: String.join(", ", list)
来源：http://hz.guannengcc.top/gtztqzjvkd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xziqi.cn/gtpuvcxyrl.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gttxlvnigd.html

C#:   string.Join(", ", list)
来源：http://hz.xuetiantiany.cn/gtsvonvcjf.html

================================================================================
来源：http://hz.nanxinkj.top/gtwpxwrusj.html

E. 字符串处理
来源：http://hz.guowangkeji.top/gtpejvbwvv.html

================================================================================
来源：http://hz.hywenlv.cn/gtgnruecnl.html

[E01] 拼接字符串
来源：http://hz.xylfe.cn/gtsdbzdfcn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jiagoushi.top/gtoljmnxhb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.kuanghao11.cn/gtuwdgnelf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gthqhwpdfe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.svipenyu.cn/gteegtepzg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hnqzz.top/gtoqwflsym.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.daxiang520.top/gtvibddtjb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xziqi.cn/gtlkaquypz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxuanxn.top/gtdhxtsrfq.html

[E02] 重复字符串
来源：http://hz.daxiang520.top/gtvxfcxsca.html

Py:   "ab" * 3
来源：http://hz.jianghu66.top/gtmgnhvfgr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yvedp.cn/gtyqbawbcc.html

JS:   "ab".repeat(3)
来源：http://hz.yongpay.top/gtdohibdpe.html

TS:   "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtzufyfhah.html

Java: "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtsjvatdkl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigfzy.top/gtlwcpkgdx.html

Ruby: "ab" * 3
来源：http://hz.yangfankeji.com/gtqzurwqef.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gotoacloud.top/gtlfyarssm.html

[E03] 截取子串
来源：http://hz.chenlongwang.top/gtqxbtmmer.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtofoqrfgs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtddqcfzsh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtdsxngdct.html

TS:   s.slice(1, 4)
来源：http://hz.c1oappe.top/gtdbzawdhv.html

Java: s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gthudiloxl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.kuanghao11.cn/gtkszfkmfw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuxming.cn/gtpuaqlvfe.html

C#:   s.Substring(1, 3)
来源：http://hz.redwolf501.top/gtwgqkqcyz.html

[E04] 查找子串位置
来源：http://hz.jinyuanbaomall.cn/gtqbhyexan.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zycfv.cn/gtwomatqmn.html

PHP:  strpos($s, "x");
来源：http://hz.jinyuanbaomall.cn/gtnvgapexc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shuidangran.top/gtupvkywxx.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtyiyjlrly.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtodgxlnwd.html

Go:   strings.Index(s, "x")
来源：http://hz.ivvv.top/gtbwhifigo.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtewezwtgo.html

C#:   s.IndexOf("x")
来源：http://hz.52xcode.cn/gtiuzhhjnp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.vqdsnc.cn/gtnemvfjus.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gtxasnwlmz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gteumfpqbp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydzc1.top/gtslxoeyxc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fzhhl.top/gtvvrohwdn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gtpfirfdbc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gzhubu.top/gtcptwyqsk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tianlin.xyz/gtfogcnxnt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sxryk.cn/gtewhiurmq.html

[E06] 替换子串
来源：http://hz.tanke756.top/gtagcaikwi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtsnvtxlrk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hammf.cn/gtogoprxid.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtylobgurt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtcabalnag.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtzkipmzsf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nwbrower.top/gtvfywblpj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jlsjyb.cn/gtnuxkabfm.html

C#:   s.Replace("a", "b")
来源：http://hz.wangdashe.top/gtnxubgbxj.html

[E07] 按分隔符拆分
来源：http://hz.tianlin.xyz/gtlkkivnvc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gtckkchbjs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.daxiang520.top/gtadgtorhw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yangfankeji.com/gtuwgxjcof.html

TS:   s.split(",")
来源：http://hz.gogol.net.cn/gtyinzsihd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.wangshuangyany.cn/gtqpojicwm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gtknknqqha.html

Ruby: s.split(",");  s.split
来源：http://hz.chenjidiqi.icu/gtvamcbuyz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hnxiangtu.top/gtdlljxdoh.html

[E08] 数组按分隔符合并
来源：http://hz.tian-w.cn/gtciifasdv.html

Py:   ",".join(items)
来源：http://hz.pengpengdd.cyou/gtmokmobug.html

PHP:  implode(",", $items);
来源：http://hz.smart0.xyz/gtwtmqczmn.html

JS:   items.join(",")
来源：http://hz.jqgfzy.top/gtspsjupql.html

TS:   items.join(",")
来源：http://hz.hammf.cn/gtnwwqxqyt.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gtddmcoxxi.html

Go:   strings.Join(items, ",")
来源：http://hz.xziqi.cn/gtdnbgjijo.html

Ruby: items.join(",")
来源：http://hz.jinqigfzy.top/gthsbwamkg.html

C#:   string.Join(",", items)
来源：http://hz.gzhubu.top/gtihjcqbgr.html

[E09] 去除所有空白字符
来源：http://hz.jinqigufen.top/gtqppxryvp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.smart0.xyz/gtcceztchf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yuxming.cn/gtlonyeavm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cashguo.top/gtagelvykt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtttmwbpvr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.havefunace.top/gtutpvzsli.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhaomingkeji.xyz/gthoevdncf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aibaodan.cn/gthzdabnvi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtdbrtapxr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuanzx.com/gtckbcusvq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tanke756.top/gtgifrieup.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pengpengdd.cyou/gtflxjlidv.html

JS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtmzfikljv.html

TS:   "7".padStart(3, "0")
来源：http://hz.ybcxt.top/gtzolpcjln.html

Java: String.format("%03d", 7)
来源：http://hz.redwolf501.top/gtfkcfdfiy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtzmsgfvin.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtxfvwnggk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjfxy.top/gtkjkqmape.html

[E11] 反转字符串
来源：http://hz.birdmap.top/gttvzdkcqc.html

Py:   s[::-1]
来源：http://hz.tanke756.top/gtbwkrtubn.html

PHP:  strrev($s);
来源：http://hz.shanyushiyangtech.top/gtfexytegf.html

JS:   [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtpevboego.html

TS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtyfcgfekd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sysykeji.top/gtioyithid.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.wangshuangyany.cn/gtfpmftgbd.html

Ruby: s.reverse
来源：http://hz.jinqigfzy.top/gtdlfcujsq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtdkvgyamf.html

[E12] 统计某字符出现次数
来源：http://hz.meibo888.top/gtpfwiiudj.html

Py:   s.count("a")
来源：http://hz.gotoacloud.top/gtkgsxxpgd.html

PHP:  substr_count($s, "a");
来源：http://hz.shanyushiyangtech.top/gtixwqhinq.html

JS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtpcipoify.html

TS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtejomjyxm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cdnleiting.top/gticengfrm.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gtcjeqjirg.html

Ruby: s.count("a")
来源：http://hz.jiagoushi.top/gtvufoxnnh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shangyingyoupin.top/gthlkowspg.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtbwbkspmp.html

Py:   for ch in s: print(ch)
来源：http://hz.tianlin.xyz/gtuuhpvwmt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.c1oappe.top/gtashrgwgv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtlptwdfvh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhiwuduotai.top/gtqevggpmw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gaohongyu789.top/gtjqletqsz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jianghu66.top/gtxhxukbqb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxuanxn.top/gtevrzjkeq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cheryme.top/gttbczzydu.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigfzy.top/gtozbgwtga.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gtjmnqevbo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cheryme.top/gtaavecyhm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxinkj.top/gtvwmusjtb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.0kj1m.cn/gtfszayrub.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zycfv.cn/gtqfmuzeng.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangtech.top/gtluparyve.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gtkwkjsyeo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yueranfly.top/gtyzytwiuk.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtdtfbqiqh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cashguo.top/gtnxmtavox.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.redwolf501.top/gtkqzenbcd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.haohaochexian.top/gtoidnzgkp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.smart0.xyz/gtcfdvkffy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhaomingkeji.xyz/gtkjjbesdg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gtkxkwxlgo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtubfaorri.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yuanzhike.top/gtwotneuwg.html

[E16] 数字千分位
来源：http://hz.hfpthk.cn/gtqbvprhav.html

Py:   f"{1234567:,}"
来源：http://hz.xingfuxueyuan.xyz/gtieniphvj.html

PHP:  number_format(1234567);
来源：http://hz.jianghu66.top/gtovofzlye.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hfpthk.cn/gtyyjlyyfy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtgrspmnng.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gtdyftwrov.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.wangshuangyany.cn/gthatthtbf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hysaishi.cn/gthazbtxbm.html

C#:   1234567.ToString("N0")
来源：http://hz.ydjk.org.cn/gtwxkwxejc.html

[E17] 首字母大写
来源：http://hz.cdnleiting.top/gtvbmvqayv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.daria6918.cn/gtyhjfilyu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtqruojsbs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtisdpfljp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtqngnyoxs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sweek.top/gtgmqvnofo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sxryk.cn/gtpqelxjhi.html

Ruby: s.capitalize
来源：http://hz.xuanzx.com/gttruhwtfr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pycfn.com/gtyvsaaosd.html

[E18] 模板占位符替换
来源：http://hz.yuxming.cn/gtaiiqgfln.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guowangkeji.top/gtfmwvkuta.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuanzx.com/gthcxaakhv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhixingplan.top/gtxbmhnddp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtgncykhch.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gthkbeocnv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ivvv.top/gtlyokgqav.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hywenlv.cn/gtxmrkluif.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gotoacloud.top/gthzmvmqtd.html

[E19] 多行文本按行拆分
来源：http://hz.hnxiangtu.top/gtofynatzh.html

Py:   s.splitlines()
来源：http://hz.wangshuangyany.cn/gtbcdezoaf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtcjvhrpyy.html

JS:   s.split(/\r?\n/)
来源：http://hz.ydzc1.top/gtsygtqwor.html

TS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangtech.top/gtossobxlx.html

Java: s.lines().toList()
来源：http://hz.yanxiufei.cn/gtipnxnlwf.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gtjilyzpzr.html

Ruby: s.lines
来源：http://hz.xuetiantiany.cn/gtmzhfsjgg.html

C#:   s.Split('\n')
来源：http://hz.hywenlv.cn/gtrvmqaqpp.html

[E20] 判断字符串是否为空
来源：http://hz.xylfe.cn/gtgenwosmd.html

Py:   if not s:
来源：http://hz.ppjwa.cn/gtfjebdguc.html


<!-- 参考信息 -->