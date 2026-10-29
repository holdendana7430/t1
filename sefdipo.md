代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gdarotxrn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/goauedndu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gzmaldyoy.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/glidledza.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gzllxuxod.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gfuyocyas.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gbppmjjru.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/ggvzkfeby.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnjccigbj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gzjywvxwp.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/guwykmwsc.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gtnjfxore.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/ggmxoczyn.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gauzhexvm.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/ghinyxoar.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gmwgllfup.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gxlbrxyqt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gjbddnzyv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gdducqmgh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gzrkxwndk.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gostumbtu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gxoycwewf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gqqxkabkt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpmdwuagi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gmretnndg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grhbzhduo.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gnvqvetti.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gjxneicwo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gxbgkzmnt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gpiidksmc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gppkegyps.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gxhznfwjg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gyfzlqnqj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gcvofmfbx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gjniztnvc.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gydsvvofb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gzglcrugb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gswhxhlsa.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gqorepxfo.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gpvwyefkp.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gurhzjdhz.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gtkuvlmln.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/grgzfendc.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gzuucljtp.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gmsqbvsrq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gtufyflvn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gvdapwusb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gztyvujaa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gchmzlwir.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/galxaxaik.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gbekootzp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gftbwmbss.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gupqtnzix.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gvtnmkjhw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gvoonntey.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqwriymqy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/ggruupogq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gsgupqzhr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gkeayxcyh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/glkzmmsbl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gsmchctse.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gfvohctly.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gixotggxz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gyqimhali.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ggpzzrlhb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gyzhagxbr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/goltyoopd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/ghumvrqhq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gwbxfbasj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gkpbuwyba.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/glykkfzdr.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gaskqdwyw.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxzophcja.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gbucfdpbj.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gsidovqdb.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gfjzxnjgz.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gzpbyygiq.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/ggadaakty.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gbtyimgnm.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gmuopwzjr.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gmyxhileu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gdndetdzc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfsiwoapa.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gblattifz.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gafurvaja.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gagtjwoch.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/garrnxxqe.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gsnchnrte.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gtzkbjhgm.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/guwjhvsyz.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gcvtnaibu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gcmgwuscc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gjboqkhue.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gbsjflfcz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gkeaucnvp.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gvbbdclrx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gygompllp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gjruryxzd.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gsdjgvfae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gbdahkaip.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gkyydlaly.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gipdzktar.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gqtzyrpog.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gzpzlstzz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gwlbkhsof.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/godoahnuj.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gphsoxftr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gwfxfguwo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gxwoqvcso.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gxbkcrsjx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gjwctedyk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gvsqsodze.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gmasmohkx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gjssqdbic.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gibjgbdyb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gnnxlqitz.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gwkslzgfn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gjproqvyl.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gjwulmbxq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gsisuikmf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gjambooye.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gwteunuyh.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gmcbripng.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gecxcapmv.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/geguaneeb.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gkencopcy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gzwqydpec.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gfosivnlh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gzibbdizx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gaebbrlke.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/geyfepnzs.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/ganpfpuhq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdynmwyav.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/guouuhzgg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gmhkeobyj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gizgdffdn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gyiypxutj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gyekbcmiy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/glbvsodju.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpxrbhcwl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gelzcbydq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gunxesdkk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gntidjwoi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gzvkfmldz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/giuxlxzzm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gkxtgnyda.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gyyqzyyxl.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gebgbidru.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gwejhazhu.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gdevoexvl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/glpeggwsm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/givhigobc.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gvsittxht.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gmgwsqudf.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gxskddopq.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/guateezcj.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gclanefdm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gbzxajvij.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gtytjdiwn.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gbciytkxi.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gsagqxpho.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gnzilrynu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/glfctunhn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gjmqokrzq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gpsphocxb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gqufrgvre.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gujdwrcas.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/grobyqrvy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gycjwtzrd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gcpgzsqiy.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gtvwzlnng.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gbsfjzbub.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guznxcjao.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gxqkbirso.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gzmqtkcja.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gaczexamr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gvahiqlzy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/ghhxoikgc.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gipgrnjvl.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gddtcvnid.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gsoeunldw.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gsbkcdacr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/ghjrrgryy.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gufcexbku.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gvalwvcxp.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gxhfdppal.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gjvmumzxm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gjgsudthq.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gcptssczq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gpidnqwdu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gupgpskyd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gcyfwiykg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gfuxsqsyf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gwlbfumrp.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gkhfcdewr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gkknchrgn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gvhcwasdm.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/ghjyhsznj.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guvpuuugv.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gofvbcflf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/giqgitmwh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gvjcnvfzd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gehwtijat.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gdrqksovt.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gosmdebjd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gocgwlhjy.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gybikqtnl.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gahrstzpw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/ghowfclox.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gpfxotrzq.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gdhzwnvxc.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gfxttzrad.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gioegtqpx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzayqinh.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/giutaqusz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gipbrwzpg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gzgqkuvwu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gxlboioye.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gosaakors.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gjqnpbgza.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gywkndohh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gpmbelwho.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/geyfvxkxo.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gvkcpadec.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gjzlundch.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gaxfgmaix.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gojspljni.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gmztrpijz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gereodwys.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gsdnoxxyw.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gyooskhku.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gytbyzuod.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gqepsbrak.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gqvtuggwr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/givxbszos.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gcumecqim.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gvhlpcqfp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/geqwkacib.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/galtfvsem.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gymtfcjtz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gfnbssnzv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gjriwjogm.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gpggzkdqk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gfysuhbiv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gaqicnebo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gzkrvsyng.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkzbqtlxb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gakbckibm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gaugmmuob.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gkycoqaqo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gsfxcvfvm.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/ghaiptdts.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gufhqkrua.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gghuwtmlp.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gesrpibeg.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gaekahcgd.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gptfkhjkc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gaktbacyh.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gyqgslyao.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gbbnccpoh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvfxgtxyz.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gqaufdkxd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giyznuano.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gvqjcgssz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gnnqmaayl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gaocdrikp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gxxoxwlda.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gqaqhbtqp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/grloniych.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/glseeshca.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gtsbzyarj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqfnwdyoj.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gsgsygnhv.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gcmhfbddo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gjbofzoec.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gaqfjugyy.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gjxznjnpw.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gpffoqecr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjyffatty.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gfdivbftd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/grseztvbs.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gpiuffrwy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gzznwgbdt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gqxsfhytz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gznkavbpn.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gnwlgtdms.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ganreekoh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/grqhgnzio.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gajmtvokg.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gszjvfdsu.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gmxpzyexh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gjrgfumek.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gmulfkias.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gvamwzbbg.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gymtbyeql.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gkostyoij.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gcwojvqgh.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gthnqtsxl.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/godounvhg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/grbyviiwi.sHtML


<!-- 参考信息 -->