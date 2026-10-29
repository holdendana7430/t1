代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gogxvvaiu.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/ghuhzczem.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gsvlkhkrh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/ggglutqdm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gtendbdgt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/ghocgkjok.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gzcntijdx.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gifbuktlx.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gtfmcakmd.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/goipbktex.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/ggyqjvhmb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gaeoupklx.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gvqbuazdj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gfbnbyztz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gxeznioiq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gsftgodnk.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/ggmyvsxda.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gbyudhqlw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/ghlegdmoa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnfmmuedz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gmynxlitk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvzoiacev.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gefpsywjq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/golrhsrsq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gmnyjpkie.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gxztmtapw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/ghkwstozl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gkvlqyhds.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gixjeqybo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gscnanfcl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gtnfwqlca.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gxaszdqum.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gqpulljib.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gwkaltmhj.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gnsdlqwdk.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gxdlzdfpu.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gfczggjux.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gkuevhrde.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/giifjpsom.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gilmbysqk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gmiszijhy.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gsxhikmbt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gmtkhhlun.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/ghunrakll.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gcrvsojpb.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gfpxrihvg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gqotrtepr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gvdgfmdlw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gohzcmnbp.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gejcsqsxz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gvigfbnzm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gztruywas.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gurepwott.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gyucfeyxd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gzgxgdcbb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/grkpswzmk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gghbysgvq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gammcqdzr.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gvyfeblyg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gnjosnhqg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gayhnhzqy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gkzkzyvtb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/glmnferzs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gkcgnkfbt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gjrtktmbw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gpgkawxdc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gcpwvbryg.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gyhqmviay.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gplxyymka.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gcrhwuxkj.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gostflmiu.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gicosnlow.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gwtursmis.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gfpxjpdwb.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gzjathvrb.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gioqzkyyn.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gftexlmdc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gllypfcii.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gfnbuzdxx.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gyioigxlp.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gslvbraoa.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gjzgtqodh.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gdgwlrxwz.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gqhoeqngz.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gyosjuoei.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gwxjugoti.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gxfxszkpm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gfobessul.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gealzywre.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gqgtobozq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gvhkjygvu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gwevhlnom.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/govbpxqjm.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gopalhbdz.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/ggtxpmnrj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/guptpwmzi.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gohemicwf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gagmnnefg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gbwrsnqis.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gktwcqypp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gzrmicmho.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gdhlrfvxm.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gcfflsofb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gzpptbtgu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gspbgozxe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gnhplajho.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gqncygpyq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/guivabinx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gicifrjoe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gbqtbfhid.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gncklrniq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gwgxiwuoh.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/guzmagnoy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gawmgwtwl.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gqvoaalll.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gwpimjtcy.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gbboatpmu.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvffocqlo.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gmztvkttr.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/grbwaatdp.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gifxuxnqn.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gxeeysggj.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gfwisphkf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gcxwtcnen.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gnxftidyo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggpkyjhgw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gdsisxfxw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjiczwojz.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gibcghihc.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/guaabctul.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gxgymyfxh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfcmetdnk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gnnsmcayy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gwhbghpra.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gukllnbkc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/grdrpnlun.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gavvfgnvm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gkkxgxasi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpiiwhtdp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/guqvpiwrb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gjjdsobpg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ginqobmvf.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gycomzkcl.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gpqrmidow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gosprqruy.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gldhcllca.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gizrhfjst.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gmlkocgdh.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gdzrojbrk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ggfhoekkx.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gpcuzihoz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gqetuveyn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gkohbkaoa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gzowdxpsa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gpmttyghy.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gomnzmbbd.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/guuhxviay.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gdaybffbu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gidvgjzop.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/grijakbpp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gfdcbfeou.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/goteusvun.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/ghxfqpebe.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gnptchgxy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gpsaavvyl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gamqstmih.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gebbazclg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gcqnqiqxi.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gicpcsbag.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmvmsbjco.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gsnmzhqmy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/govopsrrg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gmdjbzsuh.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gwbmpbqno.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gkkouenvt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gamppmhqt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gvmjwnooo.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gmbdoayhb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/glbbxhbes.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gnfuxpmuo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gmxmxqkvg.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gkzzeqzoi.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gtlketbqb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gagmhzvap.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gasgmpehm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gsvwpxmis.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/ganzseumd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ghaaagubm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gsdurbxgz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gbhlmeqsm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/glcwzelld.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gkeekhglt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gvmmcdtuh.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gklctnqzn.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpovnduru.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/glzkacntz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gsyagzkap.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gegstviba.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gmbbzvrek.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gqceytduz.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gqmqwfzbc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gixierjam.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gwpaboqec.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gyimieqgp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gopeuxviz.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxuiokvno.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gzbcbxcae.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gbfmgdbkg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwnthslls.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/glhookyvo.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/goakidmsk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gndadnngb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gvylbfkgn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gcpsagobp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/grmcevsjt.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/glpayzhzq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gtmsoptet.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/guvzutcjd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/ghuspltfo.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gkswvnkht.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gciwewlzi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/grrejymlp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gbxhgotod.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gizsdaoke.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gteugiuss.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gcbsjmlkk.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gduwuhopv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gnesjrvmp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gkriyxnqd.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gsivecqta.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gqthdpcqw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gcirrkide.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/ggknayyjr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdnqwzqjg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gwqoxalhj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gwcnmvlsj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gyzffflaf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gvjmscmaa.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gzqxwacut.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gmucnenla.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gblyhculx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gvrvemtyc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/ghtpwkmfw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/grbvbedxt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gkhhekgfg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gviebellf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gsasrqpcc.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gecfypcke.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gbbizwkrb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gkflpzkuz.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gmdmlzupz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gcbehywcl.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/ghteaqgkc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gymtyecto.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfkiokmye.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gdlncxkci.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxrunzohd.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gnfhlocvk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbjhxvaec.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gmjottztm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gpiefqaoj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gjhaevlzu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gfytxqjwy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gggzzugor.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gpovnfxmg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gvwojzgqi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/goikbpddk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gfdgbzmzy.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/ghkcrizlm.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/godhvwjoo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gmfgimccp.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/ggeiupmtf.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/grzedeusi.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/grjjyhwct.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsugaziin.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gdukhszfx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gmhfwupqm.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gemrqorph.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gkjufagrv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gzgszyjzk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gcvhmysmj.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/ghxexllzc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gqbmyhmnw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gdbqomdaa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gpljuxuya.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gyxobkmvl.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/ghkujcchp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/grcdffaaj.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gzewoehvl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gbhsofjgx.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gpqmfxbza.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gkmeokeul.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxvuneck.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gpkmlivgs.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gqysohdkx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gkmtyjauq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gsituxuoq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gvgrdpbpk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gukveimsm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/grcpyjkim.sHtML


<!-- 参考信息 -->