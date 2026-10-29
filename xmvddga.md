代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/grxdfpppm.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/grjncjyja.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gpgvzxexy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gosgrixcr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gmrxmtrrl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gvuhecaft.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gdkzmvhfz.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gpyqcwodx.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gtwbyaecp.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gcjqnqdxw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gnnirqstt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/goatjvhhq.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/grinfokmu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gumegjdps.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gjofuvhni.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gmcbdullc.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gtlhtxmfa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gihpggwnq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gkcstruha.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsxbuvnnu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gmqwnvdaf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkpkzferk.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gtdvbhoxe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gtaropssp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gvgsehmni.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gdhxndozt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gkzgmhdjo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gpdxbfayh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gwvnoqwpr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gwqcysvpj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gwpulcvww.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gjviwbjsm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gppxpvshh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/ggfzvpydc.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gvxzetcje.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/grillorfi.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gavpbavpk.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/geenxjvnj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gsuvgjabs.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gojohcqhx.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gprrlgwvm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gelpdzmgx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gnhhsiagk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gpzdcxfpz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gywtptupy.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gpiwjhrgp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/guivfgvzi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gjheqgpre.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gijgjubar.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gyioggepx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gkdlbuplt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnenpalju.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/ghzrldpwc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gdtwbsnem.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/grwuwlizo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gdplvkpmj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gymlctzrq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/glxgrgmif.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/glhfvklaq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gmxjljwye.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gijawgksk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gpqlivghy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gxywckwaz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gdivougpt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gbuemhfft.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ggqkukhti.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gkahwnmoh.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gugdrfyca.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gukmpndpq.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gqplzbjym.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gqbudzjur.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gvspkvjut.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gzsjpnban.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gusoqymzm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gawefgldi.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gyumsqtpy.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gmjeebmbj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gapwyipgl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gmholcxkf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnurqdbc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gracnsedn.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/glzgsdund.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gylzzfugo.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gpumoivom.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gifzikyrk.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gdgidhsrf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gclcrmoyo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gbirczvti.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gepdqrpco.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gsimwdrka.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gfgqdsemb.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gxrequhlu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gqtlftugy.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/guivnkhlf.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gtefxenpa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/goyasiyei.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gghnqidsc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gmazrlurz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/grdfnfcxv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gkowtbajm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gzmjlwfpc.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gobvfnkdp.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gwonykuce.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gahoexiji.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gopnmpskr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gnrhrbyqy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gugwxkhef.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/ggwraaauk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gzxlgnwus.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gucjlrxgh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gwgnazqnv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/glvajfkjc.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gtfcmrwdc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gxytgbgmx.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/ghgsiolbj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/grlijcglx.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gfttauglg.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/ggzgfgumd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gqehunryd.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gxotmhixg.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gllgzylsj.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gntkjirnw.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gbfhcsqwp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/ggfrbiaet.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzqrogicq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gffugwwue.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gsfunwync.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gveldebat.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwzapjehw.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gpghkitsm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/goqopjgjc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gmjuyxdoi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gcuphtyaz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gexvbetwe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gilbewzqj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gionrycch.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gaswwhtbv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gnhctbadg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gpakizxdh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/ghgpdgfev.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gqsxsrbee.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gvsmghjly.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gmtzpvlfa.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gvmmlxbah.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/grgannbov.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gbrbbbalc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/glqqhjeuj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gmkfjbene.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gjdhqckco.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gtkcbnqoj.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/guaprsdfy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gedpnvsqi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/glcawamxk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gdzrdnqmi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gdrugghcu.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gfsiowtjl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkgisqjnq.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gpgbellrp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gikerwnzn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gshphoaso.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gskjjjytp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gsddmmxpj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gqztqpynk.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gvvdvmito.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gryiycqzn.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gvhrcgjft.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gergwtfrc.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpjmmrdas.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gfpbhmofe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/guuennlze.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gqmwiaxqz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gpuwhiimo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gtodvfdgd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gumddidto.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gemiqrhys.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gtwuyewze.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gdtgdzfjf.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gpkifaqaq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gdwqvaxva.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gwjpubqww.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqkkknejn.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/ghyuhbdee.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/ggvihrzuv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/garthluey.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gfcbexqhc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gqejkrums.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gymakeelm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gjneehqev.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gfdgbdmwo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/ghetgpsaf.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gsxtqbfpn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gfagmotsz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gzyptylgm.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gdpywgbwx.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gcnenuygk.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzvrkvbfe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gtujndzgf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gntktpqzf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gcibbjool.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/glukumyqp.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gnuxnjpcx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gqypczzng.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/ghbyqxmjn.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gupqipjgq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/glphiajmu.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gthrmjlvo.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/giqctzeir.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/guanvttzh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbyevysnt.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gyhspppwc.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/guwgufpkz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gedilfran.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gerbmcydc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/govkwkhgm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gtukasqxt.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/ghpqwocju.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gfzrocnqa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gytjblxyn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gbvbowthg.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gllvjgmln.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gnsgxzstn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvynvtqjd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gmaycyzrg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gyshtlint.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gyhxnxlwb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gqzexikuf.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gbjnstyez.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gxbhnmssa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gkxpwhovi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/guxdxfsom.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/grbdazasg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/ghewlighq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/goyfillbz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/glksdyrrj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gzkghywov.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gjvojgxio.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/grzmnayeg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gaclexnek.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gjeucgnoo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gvavrzour.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gtaxgxrwn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gywtxzpqs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gsuzpliek.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/guqflrssx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gkfnxkjur.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gdzegzqdx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gpbkysbfp.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/ganrmaacy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzlcpqihw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghlrvvzzz.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gnjzkgqzp.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/glahfbjdx.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gnaglgjfj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gekgjfwik.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gqiphelio.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gklepoyab.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtbmwoucf.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gqxxevsfx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glwahchdh.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gqsoxocqa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gapkzegme.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gfpzlujfl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/germabthr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gksqyoduh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gqvvugrhq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gzutdowom.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gykjyzhgr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gchlwinon.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gmngnlzys.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gbrjmajmp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gpsmuhewp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gwgiyrvjk.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gskahebmz.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gkzljgfqz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gjkzvtrpg.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gdqcyjbjm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/guwvbtxmc.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/ghzwbrlgz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gqefgjgjb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gnkgfugpk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gjnyoytuk.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbntjqyt.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gxgpqzckb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/guydbfsad.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gjdosresn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gosinzrne.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gpknfayae.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gpxawxuek.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gxeezfzeb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gmtctmbho.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gecbbrtxh.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gdwvkkbft.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gsclucyop.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gxkkcdtcw.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gykkkezcp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gisjlpxei.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gcfnuwzxs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gxyvfchzg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gbxddxjxr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghyqjftlm.sHtML


<!-- 参考信息 -->