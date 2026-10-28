代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yonumen.top/gtyflbayzw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.iojbl.cn/gtlqnwtcej.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtdvmnqmoa.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhaomingkeji.xyz/gtaevhtyup.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.snrcjt.cn/gtcgzaouco.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtwawixplv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yvedp.cn/gtpdzjctln.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ehwqpu.com/gteqermjnz.html

[D15] 去重
来源：http://hz.cqqwz.cn/gtsmiiyznt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtbcqmcavz.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtixupogph.html

JS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gthmluurly.html

TS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtujhieudq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.0kj1m.cn/gtuxfzffpj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aizwys.cn/gtvujfedke.html

Ruby: arr.uniq
来源：http://hz.yueranfly.top/gtesbuqsfc.html

C#:   list.Distinct().ToList()
来源：http://hz.havefunace.top/gtmnyxkzpw.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gtkokyxhrq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.mhx1999.top/gtmxwbulsn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuanzhike.top/gtmfmqmtfs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtdahedgjc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gtjjesuryk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnqzz.top/gtmxoydlkf.html

Go:   // 手写循环累加
来源：http://hz.tian-w.cn/gtqssorkco.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shuidangran.top/gtgepusuwf.html

C#:   list.Sum();  list.Average()
来源：http://hz.redwolf501.top/gtwgrbmhnq.html

[D17] 最大值与最小值
来源：http://hz.xylfe.cn/gtlkkntzsi.html

Py:   max(arr);  min(arr)
来源：http://hz.zhaomingkeji.xyz/gterizgbcl.html

PHP:  max($arr);  min($arr);
来源：http://hz.zycfv.cn/gtjndghgej.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yvedp.cn/gtdnwrrwur.html

TS:   Math.max(...arr);
来源：http://hz.52xcode.cn/gtpnmbzlfc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.pengpengdd.cyou/gttmbuswke.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dashuyun.cn/gtillmlycm.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gtdztvuwrl.html

C#:   list.Max();  list.Min()
来源：http://hz.dianchejie.cn/gthbkhmhoc.html

[D18] 扁平化嵌套数组
来源：http://hz.xinyue.icu/gtfgqpeymi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daria6918.cn/gtqdojsjhd.html

PHP:  array_merge(...$nested);
来源：http://hz.zhixingplan.top/gtgddkqzjl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.0kj1m.cn/gtgfytjirg.html

TS:   nested.flat();
来源：http://hz.xziqi.cn/gtmrwocjbi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhengqikj.top/gtuzbfkzum.html

Go:   // 手写双层循环
来源：http://hz.gzhubu.top/gtgxmyqmgh.html

Ruby: nested.flatten
来源：http://hz.sxryk.cn/gtpcoybomj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dianchejie.cn/gtykytgypg.html

[D19] 按字段分组
来源：http://hz.jqgufenzy.top/gtjzyoyzzg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj202588.top/gtbblrbmjc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cheryme.top/gtlwwifrui.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gotoacloud.top/gtihqqizhy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinghuilouyu.cn/gtkihxcqnk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.mhx1999.top/gtmcnfsrye.html

Go:   // 手写 map[string][]T
来源：http://hz.52xcode.cn/gtghhpazym.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinghuilouyu.cn/gtuolxxyzd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yongpay.top/gtawlrftpm.html

[D20] 统计每个元素出现次数
来源：http://hz.chenzaomai.com/gtozttbklp.html

Py:   Counter(arr)
来源：http://hz.wangshuangyany.cn/gtnlyvbfgy.html

PHP:  array_count_values($arr);
来源：http://hz.cucudq.cn/gtwurixyxe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gteoarrmut.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ywan-chungtsiang.top/gtmholmkkb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenzaomai.com/gtxqhuztxw.html

Go:   // 手写 map[T]int
来源：http://hz.sweek.top/gtelermxzf.html

Ruby: arr.tally
来源：http://hz.0kj1m.cn/gtfyqtuyuh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xziqi.cn/gtzbfjrqhp.html

[D21] 判断是否包含某元素
来源：http://hz.vqdsnc.cn/gtkuiiftmj.html

Py:   x in arr
来源：http://hz.jqgfzy.top/gtrdytfuoj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gthuvjpjfu.html

JS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtrvqmrdio.html

TS:   arr.includes(x)
来源：http://hz.yuanzhike.top/gtjqujammw.html

Java: list.contains(x)
来源：http://hz.sufxvd.cn/gtbxmbxepy.html

Go:   slices.Contains(arr, x)
来源：http://hz.kuanghao11.cn/gtrbntdfqp.html

Ruby: arr.include?(x)
来源：http://hz.yj202588.top/gtwlpxnrge.html

C#:   list.Contains(x)
来源：http://hz.yj202588.top/gtolrimhsn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtzicojfbl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shangyingyoupin.top/gtedarsmvn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hammf.cn/gtwcvwgkul.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yangfankeji.com/gtgjemtpad.html

TS:   [...arr];
来源：http://hz.cqqwz.cn/gtbtmqxiyp.html

Java: new ArrayList<>(list);
来源：http://hz.kuanghao11.cn/gtnpacoycd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xziqi.cn/gtyrgstgwi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hnxiangtu.top/gtzbrkuudx.html

C#:   new List<int>(list);
来源：http://hz.nwbrower.top/gtbwxbxllc.html

[D23] reduce 累积计算
来源：http://hz.hammf.cn/gtvnhsopke.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.haohaochexian.top/gtiowwhefw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yueranfly.top/gtdfohlaem.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtbwlvmgqn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtepicwtfz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenzaomai.com/gtltzigtuu.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtobhatlsw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aibaodan.cn/gtaehjgqki.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gthpqgbjcd.html

[D24] 字典 / Map 基本操作
来源：http://hz.cucudq.cn/gtpidavxak.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yuxming.cn/gtwsdeheth.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.meibo888.top/gtmjeiowrh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jiagoushi.top/gtpxcryxbr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xinyue.icu/gtlcdddnlj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.0kj1m.cn/gtuhotwhtf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fengsongda.top/gtxfirrmau.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhixingplan.top/gtrvaivgzs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuanzx.com/gthisubgfj.html

[D25] Set 集合去重与交并差
来源：http://hz.cucudq.cn/gtjolwnzxa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ybcxt.top/gtvlcoeqfq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxinkj.top/gtakbiuxgc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jyoumei.cn/gtoqlfrjjv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.9152youxi.cn/gtvhfxjpey.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xylfe.cn/gtqaczxcqu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258888.top/gtthtvmece.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.vqdsnc.cn/gtcmvztbxs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gzhubu.top/gtxgkldwww.html

[D26] 数组转字符串
来源：http://hz.0kj1m.cn/gtxhyaacez.html

Py:   ", ".join(map(str, arr))
来源：http://hz.bjfxy.top/gtmgdashki.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangkeji.top/gtihgurcii.html

JS:   arr.join(", ")
来源：http://hz.nanxinkj.top/gtseiroecm.html

TS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtxrnrbgub.html

Java: String.join(", ", list)
来源：http://hz.daria6918.cn/gtrqmtawht.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fengsongda.top/gtihpsbdjv.html

Ruby: arr.join(", ")
来源：http://hz.tianlin.xyz/gtgcipzaba.html

C#:   string.Join(", ", list)
来源：http://hz.zhongyouzk.top/gtzvvriskz.html

================================================================================
来源：http://hz.cheryme.top/gtwusijzzn.html

E. 字符串处理
来源：http://hz.xuanzx.com/gtoftitaqx.html

================================================================================
来源：http://hz.zycfv.cn/gtihsvdzwz.html

[E01] 拼接字符串
来源：http://hz.kuanghao11.cn/gtzbhlqcbd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ivvv.top/gtwzpxjutq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhengqikj.top/gtszjmlrup.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jlsjyb.cn/gtsrqqisfg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fzhhl.top/gtvfizoumk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.smart0.xyz/gtyvfdynhx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.kuanghao11.cn/gtcgtzeitz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangtech.top/gtnbuclgcp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shzxlz.cn/gtwzjvvzvh.html

[E02] 重复字符串
来源：http://hz.xziqi.cn/gtoqsoelxp.html

Py:   "ab" * 3
来源：http://hz.shuidangran.top/gtpbgvodrp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.9152youxi.cn/gtrorbehqi.html

JS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gthblydyhx.html

TS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtqirdnrsx.html

Java: "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtahckoxrd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtniyktljj.html

Ruby: "ab" * 3
来源：http://hz.nanxuanxn.top/gtekquwqcn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.c1oappe.top/gtjecyxsbt.html

[E03] 截取子串
来源：http://hz.hammf.cn/gtkngoqzcy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hongshengwenyu.top/gtfdcuxfgc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.kuanghao11.cn/gtocunczqq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtsbxiiiii.html

TS:   s.slice(1, 4)
来源：http://hz.52xcode.cn/gtauwrwlww.html

Java: s.substring(1, 4)
来源：http://hz.kuanghao11.cn/gttskaoest.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ywan-chungtsiang.top/gtcieiaooe.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.smart0.xyz/gtgybgvgsc.html

C#:   s.Substring(1, 3)
来源：http://hz.yueranfly.top/gtzpohlhnw.html

[E04] 查找子串位置
来源：http://hz.jinqigfzy.top/gtnqwhqofn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.wangdashe.top/gtcspsnchn.html

PHP:  strpos($s, "x");
来源：http://hz.316326.xyz/gtlbubklcd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.316326.xyz/gtumcefrgh.html

TS:   s.indexOf("x")
来源：http://hz.xylfe.cn/gtibwiftey.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gtsoiguqxo.html

Go:   strings.Index(s, "x")
来源：http://hz.daria6918.cn/gttmpsegqr.html

Ruby: s.index("x")
来源：http://hz.zhaomingkeji.xyz/gtomylozdu.html

C#:   s.IndexOf("x")
来源：http://hz.c1oappe.top/gtcievlkyc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yonumen.top/gtklxkqjio.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.svipenyu.cn/gtdrfzhyxk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.vqdsnc.cn/gtilpuusgj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtbgfhruss.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.havefunace.top/gtzznrfnnf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gtwispgvxl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.wangshuangyany.cn/gtrnchisbi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shanyushiyangtech.top/gthtbcgfyb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.guowangkeji.top/gtfcmsrkxk.html

[E06] 替换子串
来源：http://hz.yonumen.top/gtvjorahpq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xziqi.cn/gteooxuwue.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinqigfzy.top/gtvyalwthn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtktbdfwsp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtoxswhwhk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtjmpflcdz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shuidangran.top/gtqolhxrjv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nwbrower.top/gtdizowzpm.html

C#:   s.Replace("a", "b")
来源：http://hz.jianghu66.top/gtvbpkadej.html

[E07] 按分隔符拆分
来源：http://hz.nanxinkj.top/gtgyrebuda.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ivvv.top/gtxonvrvzv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.meibo888.top/gtogjjyguq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yongpay.top/gtcofpsdun.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtpluhjjqv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sweek.top/gtrvezregn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhiwuduotai.top/gtxmriebfq.html

Ruby: s.split(",");  s.split
来源：http://hz.sysykeji.top/gtoithtscz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xuanzx.com/gtgokuwlxk.html

[E08] 数组按分隔符合并
来源：http://hz.chenzaomai.com/gtuojzdrtr.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtyvuajbeo.html

PHP:  implode(",", $items);
来源：http://hz.jqgfzy.top/gtcwvrnvnc.html

JS:   items.join(",")
来源：http://hz.ppjwa.cn/gtfweskwxq.html

TS:   items.join(",")
来源：http://hz.chenlongwang.top/gtpuoqumhx.html

Java: String.join(",", items)
来源：http://hz.pycfn.com/gtffttpvzo.html

Go:   strings.Join(items, ",")
来源：http://hz.hnqzz.top/gtrvqcjczl.html

Ruby: items.join(",")
来源：http://hz.gaohongyu789.top/gtlcgtyqzn.html

C#:   string.Join(",", items)
来源：http://hz.xziqi.cn/gtcdzbyfno.html

[E09] 去除所有空白字符
来源：http://hz.smart0.xyz/gtzqmracpr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258888.top/gtsdivzkmn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.meibo888.top/gtwhvxfpso.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtdvdkllnc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtnsbyeoef.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangshuangyany.cn/gtsjkwmcsp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ybcxt.top/gtswksbeey.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gtdchbpixa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cashguo.top/gtlticmvtp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenzaomai.com/gtbflpobwu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.fengsongda.top/gtaxljkurj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aizwys.cn/gtmxzoveaf.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigufen.top/gtupkluiod.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtyeztkdwq.html

Java: String.format("%03d", 7)
来源：http://hz.chenzaomai.com/gtcxilalkd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtzbgcbchu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtbajpghgs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sweek.top/gtsviwsowr.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gthhlquvty.html

Py:   s[::-1]
来源：http://hz.cdnleiting.top/gtfcwlsljg.html

PHP:  strrev($s);
来源：http://hz.zhaomingkeji.xyz/gteexoqbgg.html

JS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtfrfujpie.html

TS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtkwokcvzo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuetiantiany.cn/gtlcigomio.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnqzz.top/gtvxrfkdpa.html

Ruby: s.reverse
来源：http://hz.hywenlv.cn/gtagxvwcpw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtzvkbiiyj.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gtcwsqlgvv.html

Py:   s.count("a")
来源：http://hz.gogol.net.cn/gtchselcuk.html

PHP:  substr_count($s, "a");
来源：http://hz.jinghuilouyu.cn/gtzijjybgr.html

JS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtsvrjfzgo.html

TS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtaitxrwja.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cucudq.cn/gtsaumcorg.html

Go:   strings.Count(s, "a")
来源：http://hz.cucudq.cn/gtjydanuig.html

Ruby: s.count("a")
来源：http://hz.guannengcc.top/gtjiftuvff.html

C#:   s.Count(c => c == 'a')
来源：http://hz.52xcode.cn/gtuxtfwqxo.html

[E13] 逐字符遍历
来源：http://hz.daxiang520.top/gtqlzjpvum.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtmcdqjrps.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.smart0.xyz/gtwfshkdie.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtxtyndjwt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtsqdbelxz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtxpkozsrz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jlsjyb.cn/gtuetwxyfl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.0kj1m.cn/gtjxfujpcs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yanxiufei.cn/gtfidssesx.html

[E14] URL 编码与 Base64
来源：http://hz.hongshengwenyu.top/gterucmnjp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gotoacloud.top/gtuojuuipp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gteaofcqsd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yueranfly.top/gtwowaghlq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fengsongda.top/gthvkpyuee.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aibaodan.cn/gtfjjzunpx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pengpengdd.cyou/gtqifybffl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangdashe.top/gtdyelkgvn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhongyouzk.top/gtujpolqui.html

[E15] HTML 转义 / 反转义
来源：http://hz.haohaochexian.top/gtlqdvsjuy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dashuyun.cn/gtuibqghrz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guowangkeji.top/gtqltkxele.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sxryk.cn/gtnqxywlgz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.birdmap.top/gtzsfpknwr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yvedp.cn/gtbigkxnyu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nwbrower.top/gtzkojgygj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zycfv.cn/gtwmclttuu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhaomingkeji.xyz/gtzcfozeyo.html

[E16] 数字千分位
来源：http://hz.dianchejie.cn/gtriazjoht.html

Py:   f"{1234567:,}"
来源：http://hz.yj20258888.top/gtfzqmmuec.html

PHP:  number_format(1234567);
来源：http://hz.tanke756.top/gttejmlmsm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtmzzqdcbh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhijiandao.cn/gtayordngy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shzxlz.cn/gtuvvdmiug.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.9152youxi.cn/gtfkflzznb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tanke756.top/gtwddrbbvp.html

C#:   1234567.ToString("N0")
来源：http://hz.vqdsnc.cn/gtgernxmdd.html

[E17] 首字母大写
来源：http://hz.9152youxi.cn/gtsivnrise.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnqzz.top/gtxfqzbtci.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yangfankeji.com/gtkxpxvkvh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tian-w.cn/gtunyjsjrf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtudwtzgai.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xylfe.cn/gtglygybgv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.bjfxy.top/gtvfxytujk.html

Ruby: s.capitalize
来源：http://hz.hywenlv.cn/gtubblrnpw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.snrcjt.cn/gtitnvdbnv.html

[E18] 模板占位符替换
来源：http://hz.gaohongyu789.top/gtjkyiybeg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jyoumei.cn/gtqgxmhenu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cqqwz.cn/gtolrgvuiy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtiyovdujc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtlfqknrau.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nanxinkj.top/gtbddcrseg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.havefunace.top/gtiiervuxk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinqigufen.top/gtwpxabqnc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yvedp.cn/gtpicrcbpy.html

[E19] 多行文本按行拆分
来源：http://hz.xingfuxueyuan.xyz/gtwjwyfbmj.html

Py:   s.splitlines()
来源：http://hz.aizwys.cn/gtegrdlltr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jyoumei.cn/gtnnmchlsl.html

JS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtacskkzmq.html

TS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtyzeoqwly.html

Java: s.lines().toList()
来源：http://hz.jinghuilouyu.cn/gtnqhlcyfu.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangshuangyany.cn/gtaeeatrzf.html

Ruby: s.lines
来源：http://hz.daria6918.cn/gtvhjjfste.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gtxpgbcxvk.html

[E20] 判断字符串是否为空
来源：http://hz.andypj.xyz/gtdccikcjr.html

Py:   if not s:
来源：http://hz.jyoumei.cn/gtzuwtpsux.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shzxlz.cn/gtzokguebd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtspjhsahy.html

TS:   if (s === "") {}
来源：http://hz.kuanghao11.cn/gtpccmdykk.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtvwmiujbq.html

Go:   if s == "" {}
来源：http://hz.gzhubu.top/gteewdgbpo.html

Ruby: if s.empty?
来源：http://hz.dashuyun.cn/gtstqffztv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtlccqrrnu.html

[E21] 超长截断加省略号
来源：http://hz.xinyue.icu/gtfyqykovs.html


<!-- 参考信息 -->