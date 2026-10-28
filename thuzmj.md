代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtlieiicmo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.bjfxy.top/gtwlzuwhcz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinqigfzy.top/gtyzcyzrru.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangkeji.top/gtngwgdqoj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yonumen.top/gtvqewgkht.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenzaomai.com/gteuskekzj.html

[D17] 最大值与最小值
来源：http://hz.yj202588.top/gtbkxvtpmw.html

Py:   max(arr);  min(arr)
来源：http://hz.pengpengdd.cyou/gtukucktfn.html

PHP:  max($arr);  min($arr);
来源：http://hz.shangyingyoupin.top/gtcvobwecc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xuetiantiany.cn/gtsepiibii.html

TS:   Math.max(...arr);
来源：http://hz.jqgfzy.top/gtwodantlm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.c1oappe.top/gtztcidaom.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.fengsongda.top/gtftwdfiav.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgfzy.top/gtwuxkugmy.html

C#:   list.Max();  list.Min()
来源：http://hz.jinyuanbaomall.cn/gtzeqergle.html

[D18] 扁平化嵌套数组
来源：http://hz.havefunace.top/gtshxjnvlu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.birdmap.top/gtkftpapqp.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gthfpjfoxq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.c1oappe.top/gtdenkbmkp.html

TS:   nested.flat();
来源：http://hz.xinyue.icu/gtujpftupy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guannengcc.top/gtylchrdmk.html

Go:   // 手写双层循环
来源：http://hz.iojbl.cn/gtzbhxedcz.html

Ruby: nested.flatten
来源：http://hz.cdnleiting.top/gtjfbftaoe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sxryk.cn/gtwjxkebos.html

[D19] 按字段分组
来源：http://hz.yuanzhike.top/gtlbdmdgvj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cheryme.top/gtxlsxdedl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinqigufen.top/gtbdefhdyb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sysykeji.top/gtuyvvlzqb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.kuanghao11.cn/gtqcekatxn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtkrguuxvy.html

Go:   // 手写 map[string][]T
来源：http://hz.yuxming.cn/gtxadtxfoa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gzhubu.top/gtdtrcmmng.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.9152youxi.cn/gtrmiegmyx.html

[D20] 统计每个元素出现次数
来源：http://hz.hnqzz.top/gtacqoztff.html

Py:   Counter(arr)
来源：http://hz.fengsongda.top/gtdqmucadf.html

PHP:  array_count_values($arr);
来源：http://hz.cashguo.top/gtapijnkyb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nwbrower.top/gtxqitpkpo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cheryme.top/gtkwyyujxd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.fengsongda.top/gtbkrnyhww.html

Go:   // 手写 map[T]int
来源：http://hz.chenjidiqi.icu/gtzlgpsacy.html

Ruby: arr.tally
来源：http://hz.ydjk.org.cn/gtxaqnvdqv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fzhhl.top/gtpuzwcftd.html

[D21] 判断是否包含某元素
来源：http://hz.sweek.top/gtnnpgiooq.html

Py:   x in arr
来源：http://hz.gogol.net.cn/gtpfhpwbhd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aibaodan.cn/gtytanvkbs.html

JS:   arr.includes(x)
来源：http://hz.yvedp.cn/gthmoatoee.html

TS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtxlsthwhv.html

Java: list.contains(x)
来源：http://hz.zhixingplan.top/gtqfuwnhha.html

Go:   slices.Contains(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtwdmyhncf.html

Ruby: arr.include?(x)
来源：http://hz.ydzc1.top/gthqzxajyr.html

C#:   list.Contains(x)
来源：http://hz.jqgfzy.top/gtlnvevbuq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zdqjudy.top/gtianqzfwx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zdqjudy.top/gtscqzppke.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jianghu66.top/gtjtpnkjwd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.smart0.xyz/gtwbgxmuux.html

TS:   [...arr];
来源：http://hz.guannengcc.top/gtixwbcgpm.html

Java: new ArrayList<>(list);
来源：http://hz.hongshengwenyu.top/gtawzqnppn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhijiandao.cn/gtimbbdxiw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangkeji.top/gtickvhrve.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gtrojjycmk.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangkeji.top/gtyysfzjpp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhengqikj.top/gteymbzdyj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhixingplan.top/gtoztfuoeh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtzgzdeaga.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gtarupuwvc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shanyushiyangtech.top/gtpernnipx.html

Go:   // 手写循环
来源：http://hz.zhijiandao.cn/gtikdsvkhd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gttjpszkby.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.andypj.xyz/gtupebrswz.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhengqikj.top/gtdpacycev.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.quarkkingdee.top/gtipncgrzt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.vqdsnc.cn/gtguhmdquv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gttdfkfswg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtigguldjj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tanke756.top/gtrgqdykey.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinyuanbaomall.cn/gtwdhnjdhn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtwvioqefn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigufen.top/gtvyvakqan.html

[D25] Set 集合去重与交并差
来源：http://hz.svipenyu.cn/gtmrjvskbk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.birdmap.top/gtdfacckwg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhongyouzk.top/gtcztkbdkr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jqgufenzy.top/gtxszpnhfq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.9152youxi.cn/gtpgovjzdc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sweek.top/gtkhcmbcqe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinghuilouyu.cn/gtnpnjihbo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtxuqwfyih.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuanzhike.top/gtfozrmhrj.html

[D26] 数组转字符串
来源：http://hz.aibaodan.cn/gtzhmmtbml.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuxming.cn/gtspzmptjo.html

PHP:  implode(", ", $arr);
来源：http://hz.bjfxy.top/gtyohygvdm.html

JS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtocxyvhce.html

TS:   arr.join(", ")
来源：http://hz.ydzc1.top/gttdiqqjir.html

Java: String.join(", ", list)
来源：http://hz.ppjwa.cn/gtesupyaxs.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yueranfly.top/gtyacjssyk.html

Ruby: arr.join(", ")
来源：http://hz.xziqi.cn/gtmwoabkho.html

C#:   string.Join(", ", list)
来源：http://hz.nwbrower.top/gthpjsfgcx.html

================================================================================
来源：http://hz.smart0.xyz/gtpfohcvpj.html

E. 字符串处理
来源：http://hz.ehwqpu.com/gtxxvojqgy.html

================================================================================
来源：http://hz.shzxlz.cn/gtgvenpwli.html

[E01] 拼接字符串
来源：http://hz.xylfe.cn/gtkwxiravs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.svipenyu.cn/gtgorhglmt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj202588.top/gtmnsrhmof.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yanxiufei.cn/gttvpontcv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dianchejie.cn/gtbxcsxolo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.0kj1m.cn/gtnvijotfb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtcnqzlbdx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhongyouzk.top/gtvwqswocv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yuanzhike.top/gtmpomwrmp.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtrhuqaqtt.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gtlxpicmlo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cqqwz.cn/gtkhyeeghk.html

JS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtshvxhffx.html

TS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gtmducajry.html

Java: "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtidctbxhv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.9152youxi.cn/gthexbqbnj.html

Ruby: "ab" * 3
来源：http://hz.jlsjyb.cn/gtdbhxgypu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ybcxt.top/gtmjkabjxw.html

[E03] 截取子串
来源：http://hz.52xcode.cn/gteiiaoltd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xinyue.icu/gtzishcuvg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuetiantiany.cn/gteewnbszw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtmbbtuhhr.html

TS:   s.slice(1, 4)
来源：http://hz.tanke756.top/gtvlzbtrqg.html

Java: s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gtfsbczvxw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhoulong.xyz/gtghutmtlw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinyuanbaomall.cn/gtkptqoryq.html

C#:   s.Substring(1, 3)
来源：http://hz.yuxming.cn/gtxlvmrjei.html

[E04] 查找子串位置
来源：http://hz.yangfankeji.com/gtyuunyiql.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhoulong.xyz/gtjbfyxeph.html

PHP:  strpos($s, "x");
来源：http://hz.daria6918.cn/gtgdabhkrj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hammf.cn/gtynjzscqh.html

TS:   s.indexOf("x")
来源：http://hz.tian-w.cn/gtwuvmbozx.html

Java: s.indexOf("x")
来源：http://hz.cucudq.cn/gthmeacnwo.html

Go:   strings.Index(s, "x")
来源：http://hz.shangyingyoupin.top/gtbjdpzhpn.html

Ruby: s.index("x")
来源：http://hz.jinqigufen.top/gttlzocbvi.html

C#:   s.IndexOf("x")
来源：http://hz.xinyue.icu/gtozikxmwj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hywenlv.cn/gtvioygawn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhongyouzk.top/gtauktlgwi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj20258888.top/gtyqcqxfnr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtpejmsczm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pycfn.com/gtmaychmwr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhixingplan.top/gtjwlmaxve.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.havefunace.top/gtcizwavnm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daria6918.cn/gtkfktssrj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgufenzy.top/gtskqbtrom.html

[E06] 替换子串
来源：http://hz.tanke756.top/gtjveqwcsi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.9152youxi.cn/gtcyjzhzfn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zycfv.cn/gtubpqbjjb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtjkgcnzar.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gthodbyjet.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtftkvpkfv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.iojbl.cn/gtvpheiong.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenlongwang.top/gtytoltfyj.html

C#:   s.Replace("a", "b")
来源：http://hz.tanke756.top/gtecczrrxt.html

[E07] 按分隔符拆分
来源：http://hz.ydjk.org.cn/gttwfbtknc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.daria6918.cn/gtxnwfkbkf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yueranfly.top/gtaljotgfq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gtowpcnmct.html

TS:   s.split(",")
来源：http://hz.fzhhl.top/gtjvsujmfh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.andypj.xyz/gtberkvunc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tanke756.top/gteybzikan.html

Ruby: s.split(",");  s.split
来源：http://hz.jiagoushi.top/gtlvmgvrev.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.birdmap.top/gtdzzcyids.html

[E08] 数组按分隔符合并
来源：http://hz.cqqwz.cn/gtisdsenda.html

Py:   ",".join(items)
来源：http://hz.zdqjudy.top/gtrugoeoim.html

PHP:  implode(",", $items);
来源：http://hz.yangfankeji.com/gtkcoypscx.html

JS:   items.join(",")
来源：http://hz.cucudq.cn/gttjshaewb.html

TS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtcelfiruu.html

Java: String.join(",", items)
来源：http://hz.chenzaomai.com/gtesiwlnls.html

Go:   strings.Join(items, ",")
来源：http://hz.pycfn.com/gtihjphxgq.html

Ruby: items.join(",")
来源：http://hz.daxiang520.top/gtyrofevic.html

C#:   string.Join(",", items)
来源：http://hz.havefunace.top/gtkrzuiqru.html

[E09] 去除所有空白字符
来源：http://hz.sufxvd.cn/gteorcagaj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sufxvd.cn/gthzmkfyuw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gzhubu.top/gtfuuizkzg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtdozquvmx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ivvv.top/gtsdhsmoke.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hysaishi.cn/gtkvfnqbbf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shangyingyoupin.top/gtzahzgerj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ywan-chungtsiang.top/gtljgepdlk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.svipenyu.cn/gtvhfnpfzr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinyuanbaomall.cn/gtolmaurqg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangdashe.top/gtgbpztysx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gogol.net.cn/gtlbdrctba.html

JS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gtayyokgwo.html

TS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtrephmrdd.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtfnkovick.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cheryme.top/gtwwzbekds.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtwomjieqh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hfpthk.cn/gtexqzayur.html

[E11] 反转字符串
来源：http://hz.fengsongda.top/gtlctjzpsq.html

Py:   s[::-1]
来源：http://hz.guowangkeji.top/gtsnamdnxo.html

PHP:  strrev($s);
来源：http://hz.nwbrower.top/gtotjbyzuo.html

JS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtpxavpgll.html

TS:   [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtdhzuwxdl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hywenlv.cn/gtjuwlfrts.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.fzhhl.top/gtgaayolpx.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtmvoydbpx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gtjsfptgzu.html

[E12] 统计某字符出现次数
来源：http://hz.chenjidiqi.icu/gtczvjbxok.html

Py:   s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtrxfysser.html

PHP:  substr_count($s, "a");
来源：http://hz.tian-w.cn/gtkqtxtpbq.html

JS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtkxclpnfx.html

TS:   s.split("a").length - 1
来源：http://hz.jinyuanbaomall.cn/gtczmdlbkz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xingfuxueyuan.xyz/gtrmftlres.html

Go:   strings.Count(s, "a")
来源：http://hz.xinyue.icu/gtmlpkzict.html

Ruby: s.count("a")
来源：http://hz.316326.xyz/gtnetoulav.html

C#:   s.Count(c => c == 'a')
来源：http://hz.0kj1m.cn/gtievofgtc.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangkeji.top/gtbyjcktzv.html

Py:   for ch in s: print(ch)
来源：http://hz.kuanghao11.cn/gtaakuxmam.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shuidangran.top/gtxicwmbnn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtnscdlipx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtwlxjfflf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.havefunace.top/gtlovjqkzc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gaohongyu789.top/gthtoikwuu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guowangkeji.top/gtbdywuyuq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangdashe.top/gtaoxwtaig.html

[E14] URL 编码与 Base64
来源：http://hz.daria6918.cn/gttjymwfyk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtqfrhvnrf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtowdsyscc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ppjwa.cn/gtferdxgyn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yuxming.cn/gtmmxewlcn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sweek.top/gtqfcywipr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sweek.top/gtdpltvtxs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.meibo888.top/gtxoksuspa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangshuangyany.cn/gtrbgweaqf.html

[E15] HTML 转义 / 反转义
来源：http://hz.yongpay.top/gtqricpkdq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhongyouzk.top/gtdzujhtkc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinqigfzy.top/gtwbnqpcbd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hywenlv.cn/gtqfmgyymj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinqigfzy.top/gtvscjbxqk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.mhx1999.top/gthdrvqmkm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuxming.cn/gtahkfqpmp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fengsongda.top/gtndyaplhs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jqgufenzy.top/gtjeypobkm.html

[E16] 数字千分位
来源：http://hz.jinqigfzy.top/gtigszifgu.html

Py:   f"{1234567:,}"
来源：http://hz.xziqi.cn/gtcdqmhlmy.html

PHP:  number_format(1234567);
来源：http://hz.mhx1999.top/gtlonabehx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtojzmssyn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtjygqwwka.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinghuilouyu.cn/gtetxgdngs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.haohaochexian.top/gtlomtocjf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sxryk.cn/gtjvqdppxl.html

C#:   1234567.ToString("N0")
来源：http://hz.pengpengdd.cyou/gtzjsshmwo.html

[E17] 首字母大写
来源：http://hz.smart0.xyz/gttmbqrsmf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhongyouzk.top/gtfpiozgym.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yvedp.cn/gtnrjmzuko.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gteglhgexa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtmrhqsdez.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nwbrower.top/gtoylvkgnc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xingfuxueyuan.xyz/gtekxdvfej.html

Ruby: s.capitalize
来源：http://hz.shanyushiyangkeji.top/gtezxsbyia.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.52xcode.cn/gtxbunbmtn.html

[E18] 模板占位符替换
来源：http://hz.yuanzhike.top/gtacgegqlz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yueranfly.top/gtfcxnegju.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhongyouzk.top/gtakmqqecd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.guannengcc.top/gtvynhktoi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gtjgjnrwjj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yueranfly.top/gtwldyphru.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.mhx1999.top/gtsqicbvfz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ppjwa.cn/gtameeddaq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gttecjtakb.html

[E19] 多行文本按行拆分
来源：http://hz.haohaochexian.top/gtndyfwxon.html

Py:   s.splitlines()
来源：http://hz.iojbl.cn/gtlvzfiyid.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gtoeojosuj.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtixifkuhw.html

TS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtpzecqlns.html

Java: s.lines().toList()
来源：http://hz.ppjwa.cn/gtqhhooghv.html

Go:   strings.Split(s, "\n")
来源：http://hz.jlsjyb.cn/gtwkthyslt.html

Ruby: s.lines
来源：http://hz.cqqwz.cn/gtnmndyddp.html

C#:   s.Split('\n')
来源：http://hz.nanxuanxn.top/gttriycuga.html

[E20] 判断字符串是否为空
来源：http://hz.52xcode.cn/gtknhhrnsd.html

Py:   if not s:
来源：http://hz.dashuyun.cn/gtdluangfe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinghuilouyu.cn/gtfgunufak.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.vqdsnc.cn/gtdysaqgoh.html

TS:   if (s === "") {}
来源：http://hz.yj202588.top/gtmhhvkojj.html

Java: if (s.isEmpty()) {}
来源：http://hz.andypj.xyz/gtgmdwvxxg.html

Go:   if s == "" {}
来源：http://hz.tianlin.xyz/gtpzhfecmc.html

Ruby: if s.empty?
来源：http://hz.cashguo.top/gtesvvnsao.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gaohongyu789.top/gtannprgie.html

[E21] 超长截断加省略号
来源：http://hz.jinyuanbaomall.cn/gtlratpfzv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnqzz.top/gtbutlgtqa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shuidangran.top/gtxshzrbup.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtuoardzlp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtrnghdzyb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtxuhlucwr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cqqwz.cn/gtdwplkgkn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgfzy.top/gtevpxkcey.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258888.top/gthxjsfsbb.html

[E22] 字节长度与字符长度
来源：http://hz.yueranfly.top/gtwfmdaiyq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dianchejie.cn/gtqetxikpr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtbcncvios.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtqwgdohuq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gthhfjulck.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.bjfxy.top/gtmiugnapd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgufenzy.top/gtlvnlortn.html

Ruby: s.bytesize;  s.length
来源：http://hz.hywenlv.cn/gttegndyia.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.birdmap.top/gtalbdyboc.html

================================================================================
来源：http://hz.hnxiangtu.top/gtihnupnxf.html

F. 文件与目录
来源：http://hz.havefunace.top/gtwrzcirvw.html

================================================================================
来源：http://hz.yonumen.top/gtmvnahxeh.html


<!-- 参考信息 -->