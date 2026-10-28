代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinghuilouyu.cn/gtemnaenug.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.9152youxi.cn/gtwjirccim.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtmdmnsrof.html

TS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtrkdcigye.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.meibo888.top/gtfhheptiu.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gttgjcwzon.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cucudq.cn/gthyzmpwoy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pengpengdd.cyou/gtskxdwkie.html

[D15] 去重
来源：http://hz.hywenlv.cn/gtzcjyqnrs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xingfuxueyuan.xyz/gtbbbxqqdv.html

PHP:  array_unique($arr);
来源：http://hz.shangyingyoupin.top/gtyqgsciit.html

JS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtkrrcijfo.html

TS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtfcamiutl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtomttfggj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.kuanghao11.cn/gtauvztrjt.html

Ruby: arr.uniq
来源：http://hz.hywenlv.cn/gtwmidztvn.html

C#:   list.Distinct().ToList()
来源：http://hz.cheryme.top/gtwddbxenj.html

[D16] 求和与平均值
来源：http://hz.zhoulong.xyz/gtlliwzlni.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shzxlz.cn/gtofycqldd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhengqikj.top/gtsvxrfdmk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtudkgdoej.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtednmiqod.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pengpengdd.cyou/gtftbgfhfi.html

Go:   // 手写循环累加
来源：http://hz.zdqjudy.top/gteuemwkjw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.andypj.xyz/gtsfaaiyna.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gtmxzrlxzv.html

[D17] 最大值与最小值
来源：http://hz.yj20258.top/gtncqwjzdw.html

Py:   max(arr);  min(arr)
来源：http://hz.yanxiufei.cn/gtskbvroxw.html

PHP:  max($arr);  min($arr);
来源：http://hz.zycfv.cn/gtnojwpbvc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xuanzx.com/gtfjvclkln.html

TS:   Math.max(...arr);
来源：http://hz.zycfv.cn/gtcdeheiap.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shanyushiyangkeji.top/gtthzvcyky.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aizwys.cn/gtjyprqags.html

Ruby: arr.max;  arr.min
来源：http://hz.cashguo.top/gtfuytcngr.html

C#:   list.Max();  list.Min()
来源：http://hz.9152youxi.cn/gtpsrutgqc.html

[D18] 扁平化嵌套数组
来源：http://hz.jinghuilouyu.cn/gtgbfhxcmj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xuanzx.com/gtvtrstebi.html

PHP:  array_merge(...$nested);
来源：http://hz.yangfankeji.com/gtllqvuidn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtzxbsbuvc.html

TS:   nested.flat();
来源：http://hz.yongpay.top/gtfanjtwek.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.52xcode.cn/gtofhqaedd.html

Go:   // 手写双层循环
来源：http://hz.yj202588.top/gtypiqngzs.html

Ruby: nested.flatten
来源：http://hz.daxiang520.top/gtnvjfrhhb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gtkpxufmka.html

[D19] 按字段分组
来源：http://hz.xziqi.cn/gtvjhkykxo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jiagoushi.top/gtzecvivld.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hammf.cn/gtdgctnqun.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hongshengwenyu.top/gtkbrfytwq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinyuanbaomall.cn/gtzjiczlek.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.9152youxi.cn/gtswqhyaeb.html

Go:   // 手写 map[string][]T
来源：http://hz.smart0.xyz/gtrffwtmpo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.9152youxi.cn/gtmculrfri.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.quarkkingdee.top/gtqqrtflit.html

[D20] 统计每个元素出现次数
来源：http://hz.yuanzhike.top/gtosfdqtya.html

Py:   Counter(arr)
来源：http://hz.tian-w.cn/gtgygtdfin.html

PHP:  array_count_values($arr);
来源：http://hz.hongshengwenyu.top/gtohgxuwgo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtgsxjcxon.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtxpbcangu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ybcxt.top/gtwnqtshmo.html

Go:   // 手写 map[T]int
来源：http://hz.jiagoushi.top/gtsgsgrxgl.html

Ruby: arr.tally
来源：http://hz.pycfn.com/gtfckeyoex.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ppjwa.cn/gtuearuytv.html

[D21] 判断是否包含某元素
来源：http://hz.jinghuilouyu.cn/gtgkmbneqw.html

Py:   x in arr
来源：http://hz.havefunace.top/gtihntuoew.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sysykeji.top/gtkuxxlywc.html

JS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtoviwqevz.html

TS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtxiumdzqw.html

Java: list.contains(x)
来源：http://hz.sufxvd.cn/gtzuwmliqw.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhijiandao.cn/gtvctifinp.html

Ruby: arr.include?(x)
来源：http://hz.yonumen.top/gtqgobswny.html

C#:   list.Contains(x)
来源：http://hz.cdnleiting.top/gttwbuwjvp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnxiangtu.top/gtkaigonjt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhijiandao.cn/gtzzwjbipt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenjidiqi.icu/gtadiyicax.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenlongwang.top/gtbkqqqwqw.html

TS:   [...arr];
来源：http://hz.daxiang520.top/gttjqelsqg.html

Java: new ArrayList<>(list);
来源：http://hz.hnqzz.top/gtamqonmjt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.svipenyu.cn/gtvmywyrya.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtslczsjrj.html

C#:   new List<int>(list);
来源：http://hz.0kj1m.cn/gtphqztecg.html

[D23] reduce 累积计算
来源：http://hz.xuanzx.com/gtirvsgmzm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sufxvd.cn/gtomdrtgra.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gogol.net.cn/gtmnpmuaod.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtzglusjuw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtujprolcp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhaomingkeji.xyz/gtwawumtqe.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gtchctgvio.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gtypjvsvkd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yangfankeji.com/gtkzrsurcf.html

[D24] 字典 / Map 基本操作
来源：http://hz.ydjk.org.cn/gthkkghcus.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pycfn.com/gtmleznfmj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtsqxohjwu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydjk.org.cn/gtsazpfnmm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.birdmap.top/gtsmdpksiy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnxiangtu.top/gtucmtbhnt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gtkaslrlru.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dianchejie.cn/gtcmubgtln.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sysykeji.top/gtzvxgcnif.html

[D25] Set 集合去重与交并差
来源：http://hz.jiagoushi.top/gtegjofhop.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dianchejie.cn/gtvxujsakx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuetiantiany.cn/gtuhuxynuo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj202588.top/gtfhlccgkv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hywenlv.cn/gtvwgzubly.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zycfv.cn/gtvkdtatpt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ivvv.top/gtrdvyeulh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxuanxn.top/gtkjombjtu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cdnleiting.top/gtbglgeszr.html

[D26] 数组转字符串
来源：http://hz.sufxvd.cn/gtaxpfepid.html

Py:   ", ".join(map(str, arr))
来源：http://hz.daxiang520.top/gtpzhgtcwv.html

PHP:  implode(", ", $arr);
来源：http://hz.aizwys.cn/gtuyfserwf.html

JS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtyjarbxmb.html

TS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtlksluwrc.html

Java: String.join(", ", list)
来源：http://hz.daria6918.cn/gtumoapdbk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sufxvd.cn/gtukzvxgoe.html

Ruby: arr.join(", ")
来源：http://hz.52xcode.cn/gtlxlgrcyu.html

C#:   string.Join(", ", list)
来源：http://hz.zdqjudy.top/gttiuhqpxq.html

================================================================================
来源：http://hz.haohaochexian.top/gtsthmbdya.html

E. 字符串处理
来源：http://hz.xuetiantiany.cn/gtzsmoewlo.html

================================================================================
来源：http://hz.aizwys.cn/gtrwnaywnk.html

[E01] 拼接字符串
来源：http://hz.daria6918.cn/gtradaysxo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.feifeiyinyue.top/gtgojzjiru.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jianghu66.top/gtxydquswt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtldziydrg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtrdaguenb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinghuilouyu.cn/gtwroqniag.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aibaodan.cn/gtuxmlrvwz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pengpengdd.cyou/gtyreclhxq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.kuanghao11.cn/gtkmvholpv.html

[E02] 重复字符串
来源：http://hz.hysaishi.cn/gtprvfneam.html

Py:   "ab" * 3
来源：http://hz.iojbl.cn/gtycghdnws.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ybcxt.top/gtrmquegjy.html

JS:   "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtdcckbrqv.html

TS:   "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtlbvvhtid.html

Java: "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtekfcupxg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.vqdsnc.cn/gthlgxjwth.html

Ruby: "ab" * 3
来源：http://hz.gzhubu.top/gtlzkwxsws.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hammf.cn/gtcgodcdrf.html

[E03] 截取子串
来源：http://hz.sweek.top/gtcimiongm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gtbnxyjrxo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cqqwz.cn/gtlislqqfx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pycfn.com/gtigihylwf.html

TS:   s.slice(1, 4)
来源：http://hz.redwolf501.top/gtvfenzigb.html

Java: s.substring(1, 4)
来源：http://hz.jlsjyb.cn/gthfgdiwom.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnxiangtu.top/gtusolqaof.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ivvv.top/gtwvizofvy.html

C#:   s.Substring(1, 3)
来源：http://hz.ppjwa.cn/gtitlvsapq.html

[E04] 查找子串位置
来源：http://hz.dashuyun.cn/gteoefruhp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dianchejie.cn/gtnqaxyefj.html

PHP:  strpos($s, "x");
来源：http://hz.havefunace.top/gthamjqgqt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.quarkkingdee.top/gtjsbposiz.html

TS:   s.indexOf("x")
来源：http://hz.yvedp.cn/gtvzhyugvj.html

Java: s.indexOf("x")
来源：http://hz.sxryk.cn/gtyoqynbfa.html

Go:   strings.Index(s, "x")
来源：http://hz.sysykeji.top/gtcmhyviiq.html

Ruby: s.index("x")
来源：http://hz.aizwys.cn/gtlzwqlihs.html

C#:   s.IndexOf("x")
来源：http://hz.wangshuangyany.cn/gtgprokhvh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydjk.org.cn/gtirmfvhcq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tianlin.xyz/gtyjnccibr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shangyingyoupin.top/gtzunlsfwi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tianlin.xyz/gtnvveztnu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pycfn.com/gttgdbgani.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gthjrtcnla.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ywan-chungtsiang.top/gtkscalbqn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cheryme.top/gtzyacsdcm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cucudq.cn/gtpckzamde.html

[E06] 替换子串
来源：http://hz.iojbl.cn/gtbyzshvyc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.c1oappe.top/gtnivikslw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yuanzhike.top/gtnkggehsi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtefnheqcd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtkbdteivd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gthafggdry.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cheryme.top/gtjeqpkotu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnqzz.top/gtrcfyescy.html

C#:   s.Replace("a", "b")
来源：http://hz.gogol.net.cn/gtoymtnbqt.html

[E07] 按分隔符拆分
来源：http://hz.hongshengwenyu.top/gtszlkiczl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sufxvd.cn/gtrjvvelcz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.dashuyun.cn/gthxgeoyik.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ppjwa.cn/gtxndmcbmy.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtdhgmiypc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gaohongyu789.top/gtgaycwitq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jyoumei.cn/gtbpppjssh.html

Ruby: s.split(",");  s.split
来源：http://hz.wangshuangyany.cn/gtrlbljpgn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.andypj.xyz/gtcokveids.html

[E08] 数组按分隔符合并
来源：http://hz.chenlongwang.top/gtgrkitqmx.html

Py:   ",".join(items)
来源：http://hz.quarkkingdee.top/gtxbaxmajc.html

PHP:  implode(",", $items);
来源：http://hz.ybcxt.top/gtrmbjdgbw.html

JS:   items.join(",")
来源：http://hz.0kj1m.cn/gtwldnuzqb.html

TS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtxudeqzqa.html

Java: String.join(",", items)
来源：http://hz.bjfxy.top/gtkldmrdfg.html

Go:   strings.Join(items, ",")
来源：http://hz.zhixingplan.top/gtsrxnaiai.html

Ruby: items.join(",")
来源：http://hz.jianghu66.top/gtruhhrwyv.html

C#:   string.Join(",", items)
来源：http://hz.ivvv.top/gtnvtheedr.html

[E09] 去除所有空白字符
来源：http://hz.shangyingyoupin.top/gtsdfdkcae.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shuidangran.top/gtcoudnfwm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xziqi.cn/gtdbvucryw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtgzmwguhl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gtvkmotbay.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.guannengcc.top/gtegnxfark.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenjidiqi.icu/gtpefhqpnw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gtontxhttt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gtpustnhem.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sufxvd.cn/gtkbtcvfil.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jlsjyb.cn/gtcmevicek.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangtech.top/gtbvnqldcz.html

JS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtmgpixlbz.html

TS:   "7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtocxdrwde.html

Java: String.format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtlddrtavk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guowangkeji.top/gteistnjwo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.mhx1999.top/gtxkcpiqoj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.andypj.xyz/gtofkdtqym.html

[E11] 反转字符串
来源：http://hz.yj20258888.top/gtzinbpdwo.html

Py:   s[::-1]
来源：http://hz.hammf.cn/gtmcxmgkiq.html

PHP:  strrev($s);
来源：http://hz.yj202588.top/gtunmfcopq.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtplwugmfq.html

TS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtiosrjjyx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigfzy.top/gtogijvpqy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cashguo.top/gtsbkxwkkl.html

Ruby: s.reverse
来源：http://hz.jinghuilouyu.cn/gtrdrulkvu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtfnhlysao.html

[E12] 统计某字符出现次数
来源：http://hz.cucudq.cn/gtfszeqjzo.html

Py:   s.count("a")
来源：http://hz.kuanghao11.cn/gtdnvuheqr.html

PHP:  substr_count($s, "a");
来源：http://hz.hywenlv.cn/gtdwzqsbic.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtwhchgjtf.html

TS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtojqpozth.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.svipenyu.cn/gtrrapxzjp.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258.top/gtruvmugly.html

Ruby: s.count("a")
来源：http://hz.zhoulong.xyz/gtxqubwrfy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nanxinkj.top/gtbpcnbell.html

[E13] 逐字符遍历
来源：http://hz.havefunace.top/gtqahtyshn.html

Py:   for ch in s: print(ch)
来源：http://hz.xziqi.cn/gtpyfvsnbj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fengsongda.top/gtsbxaoerq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gtpgxqqvlr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtzzmdbspx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daria6918.cn/gtedocwjwn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtoarqzycy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.meibo888.top/gtmxzulzyw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.mhx1999.top/gtpabtulna.html

[E14] URL 编码与 Base64
来源：http://hz.mhx1999.top/gtgogxwnam.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.iojbl.cn/gtjfdtilte.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hongshengwenyu.top/gtohqlcuag.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aizwys.cn/gtodlodsam.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hywenlv.cn/gtygezamlm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xylfe.cn/gthchfojby.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.vqdsnc.cn/gtzzbbkkdi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sxryk.cn/gtpvakfrkq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnqzz.top/gtcqnslyun.html

[E15] HTML 转义 / 反转义
来源：http://hz.guannengcc.top/gtdxrcaulp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.mhx1999.top/gtjqoetmts.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jiagoushi.top/gtqqomoegx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.quarkkingdee.top/gtjwwadktm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nanxuanxn.top/gtvynlnxfd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gzhubu.top/gtzzcocrwh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.9152youxi.cn/gtrdxacmqn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.mhx1999.top/gtmxjbxkwb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gtwpinkeqi.html

[E16] 数字千分位
来源：http://hz.dashuyun.cn/gtzyalaogf.html

Py:   f"{1234567:,}"
来源：http://hz.hongshengwenyu.top/gtigywvbxr.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtqeeftxnm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtrnncnpqf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtqdboyipu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xingfuxueyuan.xyz/gtrbxidgzy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuxming.cn/gtnyzumvgn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxuanxn.top/gtiiwofjlm.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtaikrarjr.html

[E17] 首字母大写
来源：http://hz.sufxvd.cn/gtyqmftspq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xingfuxueyuan.xyz/gtqgkzspkl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhengqikj.top/gtyilmntnx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtlucuwwyz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtaogyznmp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.52xcode.cn/gtyzkybwgr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shuidangran.top/gtojbqvqim.html

Ruby: s.capitalize
来源：http://hz.jinqigfzy.top/gtykxrwpfw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhixingplan.top/gtbrppnwsf.html

[E18] 模板占位符替换
来源：http://hz.gotoacloud.top/gtkqrleloi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.meibo888.top/gtlsppewka.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guowangkeji.top/gtognkkppe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gtczvganbx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gtvmkgzuzi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ehwqpu.com/gtbciztsjp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258.top/gtzflempqi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinqigfzy.top/gtsxogeyep.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgufenzy.top/gttipoxfto.html

[E19] 多行文本按行拆分
来源：http://hz.pycfn.com/gtbecfmiqj.html

Py:   s.splitlines()
来源：http://hz.xziqi.cn/gtugixqqri.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangtech.top/gtizvphote.html

JS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtgezojaeq.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtslujhiep.html

Java: s.lines().toList()
来源：http://hz.zhaomingkeji.xyz/gtbpfgandm.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gtyjdsgaij.html

Ruby: s.lines
来源：http://hz.pycfn.com/gtdwuidfgt.html

C#:   s.Split('\n')
来源：http://hz.nwbrower.top/gtmbxrlhgy.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangtech.top/gtsnktkesf.html

Py:   if not s:
来源：http://hz.daxiang520.top/gtvaqrwpcu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hywenlv.cn/gtbcmorycj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuanzhike.top/gtynelyuws.html

TS:   if (s === "") {}
来源：http://hz.haohaochexian.top/gtcqowyrbc.html

Java: if (s.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtjfxhuyvo.html

Go:   if s == "" {}
来源：http://hz.yueranfly.top/gtwmtuzslz.html

Ruby: if s.empty?
来源：http://hz.jqgufenzy.top/gtseplxevr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.andypj.xyz/gtxzxcfwgy.html

[E21] 超长截断加省略号
来源：http://hz.jianghu66.top/gtomdmtlpl.html


<!-- 参考信息 -->