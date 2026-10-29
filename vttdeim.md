代发 wailian999

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/guocdjxcl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/ghgwsrhko.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gajohtmeq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gvezfjlhb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/guyoldmeu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gkqtwymgf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gliswkthb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqqstfguh.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/ggpdgtlid.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gywpyyxes.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gbvlkgjvk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gsczyqsrh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/ggrkninll.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gyftaicmz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gmnffjthz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gzkxuyafd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gojwyysun.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gihmhngob.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/grixkyoix.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gnarvfehb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gfvhkarat.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gljijetpo.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gdsasklac.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gakdnebsu.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gfpphiian.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/goyubepdj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gqboekdxu.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gkcgvofwt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gnoknneit.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghopmqplr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/guogqetwf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gycvdcmfy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gxkjvtbhh.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjuhxmsz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gbjlnivpo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gslpkzkxi.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gahlvsube.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gmpazshfr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gdrwacwqo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gkzhoezfs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/ghmguuyfk.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gclzjskhk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/getyuqolg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gnrhzkmvc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gbryvzyel.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gqhfwjcou.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gqisnusdv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gdsvsloqo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gxnxfwtuo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gwjnqyayf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gclulmtzy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/ggqykilvu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gadxiiksw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ghijxumav.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gaqmsyhnv.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gpngekyzx.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gtazfdktw.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gkgtvexde.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gkibhbpco.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gimtjxuxo.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gvblvvoor.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gexjzbquv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gzkxdgwfy.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gvztyavwc.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gpgphrjpc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gsomoskmg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gomfkqrdc.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gkxseacxy.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gwtdvnyre.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gxekjvngw.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gcnshfgyy.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gdhqhzfzo.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gwhxgbcag.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gfoowgwva.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gqkaqrgjy.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/ggsifatlz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gllmdploj.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/ggqjlztuh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gucltjtnl.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gccukbzoe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gkyuejixv.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gggomvgjz.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gslbivsxu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gtxvwmpvy.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/goxcnqclk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gonwbszlo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/ghfxexsqv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gphijvkea.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gczshjjvt.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gcscpzajy.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gcsonbpxc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gqhlixwbk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gtnkbnxix.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gchrryvno.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gfdhxwnxh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gqgohozia.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gfzfqstrb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gjrqsfyet.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/grcyeyrcf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/grkiumzdr.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gvbaunozx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gfdlghzlm.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdithqrwc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gqklahxfe.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gnpkcahnk.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/ggnejupjo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gotqoqliu.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gpulirdyk.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gkvibplyw.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gpfntktbt.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gsxydzhaa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdvkbqpyq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/guhttmlxv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/getueopat.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gveejemay.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gcxhijabc.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gdwowaesi.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gyygpmorv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gkgwqhadm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gnjawhopu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gxtruzojs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/glosbpxbh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gfadxkdhu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gbrobbzav.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gztjfjagt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gwbnsxbvr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gewaiygbe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gwpehebof.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gjjsrzxwe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/ggdppvwza.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gfotmrhuo.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gepunuxac.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gdarpwwhr.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gfpxlfoke.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gycjmwqyw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gegfjlgpa.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gossnisvu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gupjeansw.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gbxoibssq.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gwjuoayxq.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gwluzzuvr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gtytjhqoq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gxhwzlyov.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gmqstzzgo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/goflsnvgh.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gilacxrzy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gwvrnlnhv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gdkkpjsex.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gdeelfahw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gugxqmqpq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/graonttbr.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gcajmrqlv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gtmzmfbsn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gyrzsjsdm.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gngfzjmgf.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gyrpyioqq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/giutyonlc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gbtorwdtp.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gkrehwcsi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gmotepslr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gqzxsmfuu.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gdodpktny.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gacpgnbbb.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gtkrpqeqe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gvhbcmtku.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gmynghwtk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqwxbzjx.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/galznhfkj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gzwzftzyj.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gwtxckvrf.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gxkvwzfsr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gabmeizqt.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gzttnfnwu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gjbsxjvcs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gzdghmsjt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gylgruexz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gilwsymjm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gjgimhxca.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gzosebede.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gkixhgyvc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gzgrvokgl.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gofadimuz.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/geowdvvgy.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gipwyauav.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/guqvwqqkk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gvrkkyqkb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gujwcmdfh.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gsgdrtlpe.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gkeotjrsu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gdxcdobyr.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gangznlkm.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/glplmztgb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gcsszxxkg.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjkplwnkz.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gspzcfgzy.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gejncpbkd.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghjijfvfp.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gcwbkraog.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/guiksbtmj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gvpyuiiwt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/glttvfklg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gszvnhhxl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gqztvghwt.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gxmmofygf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gwgrxpbim.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gtijpqshz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gqxjzbikl.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/geerljpvn.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gbyzwjrmn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gatnyotkl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/grgvtcjcu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gatobjvat.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gjuaasquv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gaezwifas.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/ggtwpqjwh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gymeuhehh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gerekrdlj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gnfttfmuz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gixnbiezx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gchxqynqm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gltimmwdl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gpazyjbll.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gyicucwpr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/ghcoavkki.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gdovbomlf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/ggxwvbyik.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gyijbcexq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gdclufjxr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gptqluvbu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gkjqofcwe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gdjcglwcg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gzvotbqev.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gijwthqpg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gziejvady.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gyaucaeqj.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gnrsdllwk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gultgaxsy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gragjnjwc.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gjsibwcwd.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcvvfnjqc.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gfsmwemje.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gublqzrsg.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/goqxdwpew.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gtrgujfvc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpvbvresz.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gyfwtrrzk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdffxvqlj.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gxyydwrqo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gedgokxgf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gnomuzuzp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gqzshxhsw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gegjtodcl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gckpuksfw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gcwizazpa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gbelmxiqw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmjmhjxzj.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/galovrfmm.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gilsnewim.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gcnjysxei.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gfminyttg.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gqhxihorc.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gbfbyvwbg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/ghbboaarh.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gswmjrwlc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/ggxgalczp.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gvcfuxohr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gdzqzxswf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gvsxrgjqw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gwpzylltb.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gdeywpvzb.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gziymgzox.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gewegmocv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gwyvjdfrn.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gugdqlhvz.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/guwyoixkw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/goqudgtfi.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gxgxfhdou.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gcshrygzo.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gzpfitibi.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gofemenhp.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gecnzkmmz.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gmcigncsj.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ggclbsqzt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/grjgkxttp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/guvruvfda.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gcimtyitk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gurgkrajo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gradhjbiq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/grkybjypk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gfclfrfsm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gclyxzlad.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ghqicwurb.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gdgjxaiur.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/ghrddqflg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gspithltr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/guvolrqbg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ggzahoszl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gmnwnjlvn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/golhodkuy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gcthlipod.sHtML


<!-- 参考信息 -->