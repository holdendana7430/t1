代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhoulong.xyz/gtfssnuxwm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtqzybazrl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sweek.top/gtzebhnqmh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtugaehrbg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gotoacloud.top/gtfniuolsg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sysykeji.top/gtteweuwia.html

JS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtejcjhhct.html

TS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gtvmhqmmsq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.iojbl.cn/gtdjokwekj.html

Go:   // 手写循环
来源：http://hz.jiagoushi.top/gthnmayuaf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ydjk.org.cn/gtfpyzyuxh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hywenlv.cn/gtexfhziok.html

[D15] 去重
来源：http://hz.zhijiandao.cn/gtyekszpqp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gtirpuodiw.html

PHP:  array_unique($arr);
来源：http://hz.tian-w.cn/gttqtcjoeo.html

JS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtrvqpoffu.html

TS:   [...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtedzbtkbf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jianghu66.top/gtofhtvsmv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zycfv.cn/gtwbrzzhqo.html

Ruby: arr.uniq
来源：http://hz.xingfuxueyuan.xyz/gtvzribgzq.html

C#:   list.Distinct().ToList()
来源：http://hz.cqqwz.cn/gtkspsjwzb.html

[D16] 求和与平均值
来源：http://hz.9152youxi.cn/gtbwjnmlqv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gogol.net.cn/gtiuzrrxsl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.meibo888.top/gtxlxjwsnu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.316326.xyz/gtbnsppdoy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gtihtzqtao.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenzaomai.com/gtrpkwwylc.html

Go:   // 手写循环累加
来源：http://hz.sweek.top/gtirlxucoy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yangfankeji.com/gtzjnefrls.html

C#:   list.Sum();  list.Average()
来源：http://hz.jiagoushi.top/gtfnmetjbh.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtafjuednl.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxuanxn.top/gtsleteucv.html

PHP:  max($arr);  min($arr);
来源：http://hz.shzxlz.cn/gtcjktbqkm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.bjfxy.top/gtwlmijpxp.html

TS:   Math.max(...arr);
来源：http://hz.jqgufenzy.top/gthpvypqll.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtwennvjqa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sysykeji.top/gtvkoruarb.html

Ruby: arr.max;  arr.min
来源：http://hz.jiagoushi.top/gtniyiqhvv.html

C#:   list.Max();  list.Min()
来源：http://hz.gzhubu.top/gtipcqneuf.html

[D18] 扁平化嵌套数组
来源：http://hz.zhijiandao.cn/gtfmpuwrhz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258.top/gtxekajjzv.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigfzy.top/gtalqykmxj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yueranfly.top/gtxhmvazwx.html

TS:   nested.flat();
来源：http://hz.pycfn.com/gtwgegmzsr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gzhubu.top/gtsmwhgepq.html

Go:   // 手写双层循环
来源：http://hz.cashguo.top/gtcqwhsbfq.html

Ruby: nested.flatten
来源：http://hz.jqgfzy.top/gtjoujuhto.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zycfv.cn/gtftdlwffn.html

[D19] 按字段分组
来源：http://hz.quarkkingdee.top/gtahspokxr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangtech.top/gtoukhsyda.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gaohongyu789.top/gtxlffijtz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.andypj.xyz/gtutgwfoan.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gtiuuxgyrw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj202588.top/gtaisdjvgz.html

Go:   // 手写 map[string][]T
来源：http://hz.chenlongwang.top/gtqcrnpxzx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhijiandao.cn/gtmmiegkik.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinghuilouyu.cn/gtldotfayq.html

[D20] 统计每个元素出现次数
来源：http://hz.hnqzz.top/gtjuxlvzbt.html

Py:   Counter(arr)
来源：http://hz.yangfankeji.com/gtcmbjgmct.html

PHP:  array_count_values($arr);
来源：http://hz.sysykeji.top/gtkxolkdyj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtsijfyzgd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sweek.top/gtkqohaxwm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gtacbnffhd.html

Go:   // 手写 map[T]int
来源：http://hz.wangshuangyany.cn/gthcbjbpgg.html

Ruby: arr.tally
来源：http://hz.zhijiandao.cn/gtvccsurho.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dashuyun.cn/gtvghoekxs.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtnvaqqsmf.html

Py:   x in arr
来源：http://hz.ybcxt.top/gtehkmuloz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yueranfly.top/gtosbyhahv.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtyicksebp.html

TS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtusvrrlri.html

Java: list.contains(x)
来源：http://hz.kuanghao11.cn/gtkszjfkjz.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhongyouzk.top/gtjbxhzniq.html

Ruby: arr.include?(x)
来源：http://hz.sweek.top/gtjoqizmme.html

C#:   list.Contains(x)
来源：http://hz.bjfxy.top/gtkatcfvvf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtpcbhbloc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.daria6918.cn/gtkayuwkwi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuanzx.com/gtiqqciovq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pycfn.com/gtsffwathz.html

TS:   [...arr];
来源：http://hz.wangdashe.top/gtgtgxtmsg.html

Java: new ArrayList<>(list);
来源：http://hz.vqdsnc.cn/gtxwutucoh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgufenzy.top/gtmrxidvob.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtkwugroih.html

C#:   new List<int>(list);
来源：http://hz.yanxiufei.cn/gtlpkyiczt.html

[D23] reduce 累积计算
来源：http://hz.fengsongda.top/gtcqkuzibi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhiwuduotai.top/gtyspicbcc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xziqi.cn/gtqbkhchdn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtavvwbyue.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xingfuxueyuan.xyz/gtixdzolby.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhixingplan.top/gtnfohxxqt.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtijcmbpey.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.bjfxy.top/gtpbpjtnrk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ybcxt.top/gtnmzgfggf.html

[D24] 字典 / Map 基本操作
来源：http://hz.xuetiantiany.cn/gtcvsdpvkd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.52xcode.cn/gtirhohwah.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ppjwa.cn/gtrodjqlds.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangtech.top/gtqpinaqat.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hongshengwenyu.top/gtlcoqkjsz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.9152youxi.cn/gtscgcydzu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuxming.cn/gtvomecoyt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhongyouzk.top/gtbwwcwuoj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuanzhike.top/gtcdygocpa.html

[D25] Set 集合去重与交并差
来源：http://hz.tian-w.cn/gteuhprioo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.bjfxy.top/gtenerdeis.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.vqdsnc.cn/gtkihtftmr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj202588.top/gtoiwtgcib.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shangyingyoupin.top/gtckkmxpvc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.0kj1m.cn/gtnotykgoa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnxiangtu.top/gtntoeeqwo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangdashe.top/gtrwfazero.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gtedzbbbac.html

[D26] 数组转字符串
来源：http://hz.pengpengdd.cyou/gtaqvqhakp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yangfankeji.com/gtafimwwtq.html

PHP:  implode(", ", $arr);
来源：http://hz.cashguo.top/gtucxtyiit.html

JS:   arr.join(", ")
来源：http://hz.cashguo.top/gtqbktlige.html

TS:   arr.join(", ")
来源：http://hz.ivvv.top/gtozatluls.html

Java: String.join(", ", list)
来源：http://hz.chenzaomai.com/gtlaozizqq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigufen.top/gtwqhfrrau.html

Ruby: arr.join(", ")
来源：http://hz.guowangkeji.top/gttnftncxc.html

C#:   string.Join(", ", list)
来源：http://hz.guannengcc.top/gtorajeziv.html

================================================================================
来源：http://hz.hnqzz.top/gtguxkldfk.html

E. 字符串处理
来源：http://hz.hnxiangtu.top/gtqyoegsvx.html

================================================================================
来源：http://hz.snrcjt.cn/gtxoofsczs.html

[E01] 拼接字符串
来源：http://hz.yueranfly.top/gtxgunvfjh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhixingplan.top/gtqtgoouyd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.quarkkingdee.top/gtzigmrnfz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xylfe.cn/gtvihqjzww.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtncpifrll.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj20258888.top/gtcstqvnak.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tanke756.top/gthsjhyrrn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtghhyixkt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.havefunace.top/gtlyysbosi.html

[E02] 重复字符串
来源：http://hz.52xcode.cn/gtbqijuyvr.html

Py:   "ab" * 3
来源：http://hz.zhengqikj.top/gtqezgjajg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtberryolp.html

JS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtqaheeluu.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtvypoggww.html

Java: "ab".repeat(3)
来源：http://hz.yj20258888.top/gtbvjtplmx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ppjwa.cn/gtxneryobq.html

Ruby: "ab" * 3
来源：http://hz.cqqwz.cn/gtlzkiszwc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxinkj.top/gtmzhksixg.html

[E03] 截取子串
来源：http://hz.pengpengdd.cyou/gteeuiaiax.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xylfe.cn/gtudhaczcu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtwamjchvd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.iojbl.cn/gtzfpzxvns.html

TS:   s.slice(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtnwtzijds.html

Java: s.substring(1, 4)
来源：http://hz.yueranfly.top/gtsdccueeb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gzhubu.top/gtdkognhqh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cqqwz.cn/gtoyzcvdqe.html

C#:   s.Substring(1, 3)
来源：http://hz.hammf.cn/gtsxmhmqlk.html

[E04] 查找子串位置
来源：http://hz.chenjidiqi.icu/gtgcqdchot.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cucudq.cn/gtwwyqefqu.html

PHP:  strpos($s, "x");
来源：http://hz.yj20258888.top/gtmhnqviqa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtnixuaabm.html

TS:   s.indexOf("x")
来源：http://hz.cdnleiting.top/gtdjhnjcmz.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangtech.top/gtfcshkkuq.html

Go:   strings.Index(s, "x")
来源：http://hz.316326.xyz/gtctxxbtnl.html

Ruby: s.index("x")
来源：http://hz.havefunace.top/gtybpynqhi.html

C#:   s.IndexOf("x")
来源：http://hz.chenlongwang.top/gtteshxfzl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yangfankeji.com/gtquidvesz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258888.top/gtawwqewul.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.316326.xyz/gtqietntfs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shangyingyoupin.top/gthxvgppcw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.snrcjt.cn/gttyxdhxcd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtkcxhvqir.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.wangshuangyany.cn/gtiiaiqbux.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yanxiufei.cn/gtsrmaczii.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ybcxt.top/gtjpquguaf.html

[E06] 替换子串
来源：http://hz.sufxvd.cn/gtttsyhavm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cdnleiting.top/gtyrvhcqhb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yuanzhike.top/gtuxebocgn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtfahrvugd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtqaubfzkn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtrifuktpt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shanyushiyangtech.top/gtfjyhrhjj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydzc1.top/gtdqksofrk.html

C#:   s.Replace("a", "b")
来源：http://hz.hysaishi.cn/gtvpfoxgzp.html

[E07] 按分隔符拆分
来源：http://hz.hfpthk.cn/gtwatohysq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.iojbl.cn/gtrrgjusoy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zdqjudy.top/gtpcsxhjnx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.havefunace.top/gtyirzgdia.html

TS:   s.split(",")
来源：http://hz.wangshuangyany.cn/gtgzcblhdm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shangyingyoupin.top/gtdxpgyalc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shzxlz.cn/gtvpctpkvf.html

Ruby: s.split(",");  s.split
来源：http://hz.andypj.xyz/gtijsaginv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xylfe.cn/gtruinntyz.html

[E08] 数组按分隔符合并
来源：http://hz.gaohongyu789.top/gtppwkucuu.html

Py:   ",".join(items)
来源：http://hz.cqqwz.cn/gthaxpwstg.html

PHP:  implode(",", $items);
来源：http://hz.nanxuanxn.top/gtwbpxpolg.html

JS:   items.join(",")
来源：http://hz.yonumen.top/gtgkicihrz.html

TS:   items.join(",")
来源：http://hz.jlsjyb.cn/gtfksqnomi.html

Java: String.join(",", items)
来源：http://hz.yj20258.top/gtmjazrijm.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangkeji.top/gtzvrypsev.html

Ruby: items.join(",")
来源：http://hz.sysykeji.top/gtwvxqhsao.html

C#:   string.Join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtosluraio.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtxokaxabt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj202588.top/gtunzxbpap.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xuetiantiany.cn/gtznepxkpe.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtzikjyhgz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.wangdashe.top/gtiexqyvcc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.smart0.xyz/gtacupsotv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.0kj1m.cn/gtfdmnlvbl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hywenlv.cn/gtncurlmrh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xinyue.icu/gtphqgarzf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ywan-chungtsiang.top/gtqibuflqd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gtmkegrfna.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtomvhzbxp.html

JS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gteolqkwqh.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtjxbqphcl.html

Java: String.format("%03d", 7)
来源：http://hz.ydzc1.top/gtltbxjdve.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.quarkkingdee.top/gtyetzzhww.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.iojbl.cn/gtqildpzva.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigfzy.top/gtmfaxfkay.html

[E11] 反转字符串
来源：http://hz.quarkkingdee.top/gthbaazfrp.html

Py:   s[::-1]
来源：http://hz.zhixingplan.top/gtbksmitfv.html

PHP:  strrev($s);
来源：http://hz.mhx1999.top/gtoujnuuvz.html

JS:   [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtjtlvjknq.html

TS:   [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtuqcupltr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gtbthmvjcp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ppjwa.cn/gttcympckn.html

Ruby: s.reverse
来源：http://hz.jinqigfzy.top/gtpcfyuopz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtyyluqwcn.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gttibjobor.html

Py:   s.count("a")
来源：http://hz.gogol.net.cn/gtnpozxwtg.html

PHP:  substr_count($s, "a");
来源：http://hz.haohaochexian.top/gtudkygiix.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtnbiinlre.html

TS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtzilkvpxi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xylfe.cn/gtrwutaeqm.html

Go:   strings.Count(s, "a")
来源：http://hz.aibaodan.cn/gtmuzqgrpy.html

Ruby: s.count("a")
来源：http://hz.chenjidiqi.icu/gtmfnphnhm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nanxinkj.top/gtfajktmpc.html

[E13] 逐字符遍历
来源：http://hz.shuidangran.top/gthewardcm.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258.top/gthhbisbtt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigfzy.top/gterrdufip.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gtduejjupm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtfrklghjc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tanke756.top/gtrhzdgmfd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.0kj1m.cn/gteswdynlx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.svipenyu.cn/gtylwnsmpu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.meibo888.top/gtowxwqnpj.html

[E14] URL 编码与 Base64
来源：http://hz.zhongyouzk.top/gtcfwbfhue.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtzvjmsqvl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jyoumei.cn/gtsqvkcwyy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangdashe.top/gtfsnfvarb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jlsjyb.cn/gtfcrexqan.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fengsongda.top/gtzorcaruj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jqgfzy.top/gtmqxhxeig.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gthnrbqkml.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnqzz.top/gtciwyngvz.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtfkhvrwrv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhaomingkeji.xyz/gtzxlsursi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cheryme.top/gtbdvvaxgm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhiwuduotai.top/gtpstccbfo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.kuanghao11.cn/gtgbujadvt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gzhubu.top/gtbqnhdblu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gtbumwlfhi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pengpengdd.cyou/gtarxlucdl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dianchejie.cn/gtnaytdveq.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gtuutzcjsp.html

Py:   f"{1234567:,}"
来源：http://hz.cucudq.cn/gtnovikjxb.html

PHP:  number_format(1234567);
来源：http://hz.wangshuangyany.cn/gtbzmzaglt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.mhx1999.top/gtwljtllmj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gttpvgdagl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtrmiuqbbo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cashguo.top/gtkgtiiyqq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.52xcode.cn/gtxdehaumz.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgfzy.top/gtzkybondg.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gtyjynbaqu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhijiandao.cn/gtsexfwxno.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aizwys.cn/gtykyyojyv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gthhtyaqpt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtrtrbqwxd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shangyingyoupin.top/gtcyvebakv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shuidangran.top/gtfemppoli.html

Ruby: s.capitalize
来源：http://hz.jiagoushi.top/gtobflceyf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.guowangkeji.top/gtdvfrjsxe.html

[E18] 模板占位符替换
来源：http://hz.nanxinkj.top/gtgookhasp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xinyue.icu/gtqyyebdrj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yueranfly.top/gtbjznxtex.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtyazhbxcd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gthbqnlqtx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fzhhl.top/gtawdfdvlt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangtech.top/gtcdjahklh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cashguo.top/gtscgyhlvg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtwfmbygwn.html

[E19] 多行文本按行拆分
来源：http://hz.hongshengwenyu.top/gtprewrnia.html

Py:   s.splitlines()
来源：http://hz.0kj1m.cn/gtmukvkeyq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuxming.cn/gtyqdamdks.html

JS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtizdfsxci.html

TS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtwxisppsk.html

Java: s.lines().toList()
来源：http://hz.havefunace.top/gtwypjmqem.html

Go:   strings.Split(s, "\n")
来源：http://hz.cdnleiting.top/gtuavkjuhr.html

Ruby: s.lines
来源：http://hz.vqdsnc.cn/gtxkzmemrx.html

C#:   s.Split('\n')
来源：http://hz.yj20258888.top/gtdzwbjjge.html

[E20] 判断字符串是否为空
来源：http://hz.zhongyouzk.top/gtzndebigz.html

Py:   if not s:
来源：http://hz.jiagoushi.top/gtsouwtbep.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.9152youxi.cn/gtuurzwvjf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guannengcc.top/gtckpuwfnr.html

TS:   if (s === "") {}
来源：http://hz.zhiwuduotai.top/gtynxccema.html

Java: if (s.isEmpty()) {}
来源：http://hz.yongpay.top/gtjvhtkkqr.html


<!-- 参考信息 -->