代发 wailian999

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gbxvfywuk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gnnzmuxxl.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/groimnzro.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gsostmhmm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/ggwhyoefp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gwmhyfnps.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gghtdpluj.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gisvvymqu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/glhqksgph.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gzofpfzae.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gjsirwmap.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/grthecwxn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsscgxtir.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gmhueokct.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gnpatwbfw.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gxkcvkhbz.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gqcrvvbvc.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gsxaazqve.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/glmyrizzg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/glubgwoxk.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/ghoppfibb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gvzfdsifp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/guncqzgtu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gevheauwl.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gtcnxewpm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gbxxggcdx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gdptqfpdd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvhfeiejz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gibycdrzw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glwhrhfgw.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gnfkeoovb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/grfftwehp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gwtgudfpt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gpjdumlur.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gjlxnhenc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gejyxupsb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gdkozfzuj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gihbpfiet.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gawvcmscp.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gsvzqfiox.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gxeiktrnn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gcyltfvvr.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gczlaqwzp.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gjjzvcdxm.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gwybcxevs.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/grutcgefp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gqgahwhxk.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gyljtroik.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gtyssxgqv.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/glwzebfuk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gztybeylm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gppkvpxyj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gzcvknmas.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqzyczgpt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtrblyre.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/guickhjgz.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkbjocecc.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gqsgolbhf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gpzzrfxaq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gyjsnxrhs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gsbvhczrg.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gulqcfteg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gnsruoudo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gxugzeyik.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gzqqtzwku.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gpflrrljq.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/glncihsjs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gfnhqpjmc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/guckznwcc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gvumlwiim.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gbfajwnrb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/govtncduo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/ggpcrvsem.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gryiozeks.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gfixyxdlb.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/govcuqeey.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxuespxzw.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gfaqzbpyj.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gigjxfqha.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gqiummpwt.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/glrdjnrrk.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxcjrflee.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/ggluqwdbw.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/ghvipmxbe.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/giuxlqrex.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/geyucpnhw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gvxmoxycd.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gveozyolr.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gkxszgosv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/ggyflpbvs.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gaiukxdyk.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/ggggqssdv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gvuwiakkh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gucnqvmcu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gopidsghz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gwnbrjdyu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gddsyznvg.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gmrcunzho.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvqnpdane.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gxohjqwzh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gmnvwbvbq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/grdrvohla.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gbucvnviy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/ggtctpjdf.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gcywajine.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gatkwprsk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/ghmwcuhsx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/ggxfnjjho.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gwhofthtw.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gacjaaeyj.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gksdprsep.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/goabaunjk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/grqceltoj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/ghfgjdqqo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/guwgyiwpr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gklhimncj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gchkfedtd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gsuuskfkz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gaeoccvvv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gxkqfhxzp.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gezmgpvxr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gzjrkyrdf.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gznttjgis.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gtsbzxpit.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gknqisvra.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkvfrjigs.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gsygeewef.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gckntshnu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gumiflahl.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gvbuqeicy.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gmlffusvv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwlddpgdn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gedkkbcbi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/ghyrraolo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/grnofcdka.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzbnzdymn.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gnftdnqhh.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/goxbuxkoc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gfgdnfeed.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/grtcsclao.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gzgvcglzk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gktgomckd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gjyjbkiov.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/grompzbql.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gvdqyqxxb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gqrgjdclv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/glfwijqrg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gyqljxkuc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/glrlpxsgq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gpmjakzzc.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gfazkvdpe.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gjqiptyhg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gaqwiagaf.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gwmiwshmm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/ggwxgwhlw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gkcnaysev.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gmmxixblw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gaosdmoxn.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gafbmrnno.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gyvoiyrwj.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/ghdpfdahh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gsiultngf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gwyipgtuu.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/ghkutiwzf.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gpfoutxnh.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gbfaaroda.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/grkdxlduy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvljnuijn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbvjbwtzz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/grbpwomfs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gixwwokxh.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gdiuuviay.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/geghoyjxt.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gobecgtxv.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/glqasawxy.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/ganewfjfp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkgbgnkdc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gcrhhidgu.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gztaeggce.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/grcnxhhsd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbsqvvgzn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gozernyue.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gdveemrud.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gwkmjlkfy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/glmtwrmxg.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/grwxbjdjr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gwaldaiew.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gqkbrwmzx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzpeehffi.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gmdzxkcky.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gebmyqful.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/guazfunkc.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gnngfsaam.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gtduhyued.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/grruarjuw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gjbsuiqid.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gmnwtwshu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gijwofitg.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/guybtvrmj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gsltskrya.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gyycxgeaj.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gukvpcjbk.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdkllxtlp.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbwyspgvw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gmyzcdwbd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gxlgjlgro.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gtacjjbbu.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gfdajcuhe.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gaglkjjyi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gzvmcwvbz.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gfolzrhhe.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gukaznogb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gesqhojoz.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/genhakdfj.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ggxyeztsd.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gmkqfkedr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvbkrfmle.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/grfhbtlee.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gszhbnfaj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/ggbltfrkh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gtuquxaqe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gqlkxotyd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gitbujjoo.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gnbszhtvg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gjgmepcbd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gtplaqpqn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gxaedphdf.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gpiqkdgoi.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gkydetjfy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gbctxzovi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gymxzbgwh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gghnivrvn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gdojeeeds.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gkhzeuddv.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ghvdcxynv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gnazbabwp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gdybkqweh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/ggybaccex.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gojbbmprl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gxdmakcyx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/guvsezylh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gwsyqckwl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gmomghdil.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/grewrvexs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gfgftqrcp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gidnjnusb.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/givkkzeap.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gudbmnnxa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gucgsuhkv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gohhdsouu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gdqelxnam.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gsdovtbfe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gxdqpwwvl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gozzgknke.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/guaiasffd.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gqzrtmeoh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gufigcodw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyqhbzngh.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gjzwwxrwx.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gnesrkati.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gcitnunld.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gnmmzfohe.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gyttqspbn.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gqpdsrobf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gutjqmezg.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gprqljmlo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geapwsifj.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gyyyjgxll.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gzhufefgx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmektldgw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/glihcfuca.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gbvevajpy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gjxryarus.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/geoshnncn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/ggvpowpoe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwhigmdlh.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gwksrsdez.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gfrhmqrsq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/guskvkkpr.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/geceeowtn.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gxesdgfnb.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gyvchzntw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gfkwggpao.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gyyaqapxr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gkxfezrjg.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gblmwwbde.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gkibgkkfh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gaswaaloc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gkmljioch.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/godxzxtzt.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gwaxbmptc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gbdxzqxyh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gvkqcuxje.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gvrnnbzra.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gtgcidzgw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gclmfeguz.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gbzlojmtb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gdwktpcwt.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/guxursykp.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gmjvhqnpq.sHtML


<!-- 参考信息 -->