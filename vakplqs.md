代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuosudlv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/givigupmg.sHtML

Java: // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/gcnflgrzm.sHtML

Go:   // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gfzqbcqzl.sHtML

Ruby: a, b = pair
来源：http://baike.fanxiaobao.xyz/Article/details/gvmkrpkwu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fanxiaobao.xyz/Article/details/gzzrfazlb.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxexgermr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gzadkimzn.sHtML

PHP:  // 无重载
来源：http://baike.fanxiaobao.xyz/Article/details/gulswlbry.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givvspttj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqdhmtrk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gosdbzgul.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/guumwholk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghudhwgyy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizwrunhf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwrxlnoi.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/goflapxzu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gthkbnnmo.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gyclhugyc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fanxiaobao.xyz/Article/details/grgxzdktf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gvxuupxcq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/gwlfrazns.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giddomnkl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkytituv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fanxiaobao.xyz/Article/details/gzvzkmnca.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/grxpsccxo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/grivghpbl.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhdneooo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdemtgoj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfthyyxcb.sHtML

JS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/galdmhvod.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/grvwvxfzu.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/glgvunzks.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grokcjlbw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gculzefty.sHtML

C#:   list.Add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjhoiyps.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaebkywf.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjgrsmxw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gilxyftru.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fanxiaobao.xyz/Article/details/glenevffa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqmeugjx.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgneagva.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkgdjzgx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcarxnbb.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gyhdrksok.sHtML

[D04] 删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/ggnoccbxm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqghmzjc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxjxvlen.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtxgaqda.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeehtudg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gsuhmwzpe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjuzmudr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gcfzhatas.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fanxiaobao.xyz/Article/details/grisvouns.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/glsetipow.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhyrdhpi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gdejldiwn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geujfssid.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgvvgkno.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/gdujrateh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyosaebq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gaetcrhaj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gpbhvwzhc.sHtML

[D06] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gatgdoame.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/grjmwlknx.sHtML

PHP:  count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhxcsorj.sHtML

JS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgtbozes.sHtML

TS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/gaskgprgj.sHtML

Java: list.size();
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxjghyyw.sHtML

Go:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gcefmilvp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/galgmwtvc.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggznnpapv.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqomopup.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxrrvnyq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnwzltdb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gvfktcbbo.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/ginsloydv.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/glgzhfwkh.sHtML

Go:   arr[1:4]
来源：http://3g.fanxiaobao.xyz/Article/details/gwqtmfesm.sHtML

Ruby: arr[1, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gxsatnbzu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqevnuvxx.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrckmfkw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcicrnlj.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fanxiaobao.xyz/Article/details/glhifjqnd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogsavsrt.sHtML

TS:   [...a, ...b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfdanhad.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gbyipysnk.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgyahspn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gbrdxknsn.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/ghucsrvhw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfktiskq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaipqwdgf.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrmeiddc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvryxtzm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/gngiowtzj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gycawutob.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gbxynpfrw.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gncojkmvz.sHtML

C#:   list.Sort();
来源：http://3g.fanxiaobao.xyz/Article/details/gjldalvro.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnmhwknl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegumejsz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/ghlutnubf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/ghlacmkxg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekbbumqi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gztlwpunt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfqfmluy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubxothik.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfwatvrn.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrwdjvmg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fanxiaobao.xyz/Article/details/gmrecrvhk.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gytvengda.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/gmrggjllm.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguvvxmqj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpnuwctf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkphacveb.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmjobjmc.sHtML

C#:   list.Reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gtbrnfiwk.sHtML

[D12] 查找元素下标
来源：http://m.share.fanxiaobao.xyz/Article/details/gepvqmqlw.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gqfsgknlr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glstxsqpg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gshonvqje.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcewhmsl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fanxiaobao.xyz/Article/details/gfuaqgwxh.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/giiaohwex.sHtML

Ruby: arr.index(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ggykefybp.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fanxiaobao.xyz/Article/details/gtbbeypnc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuvoubfz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqkuqynj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gyttksehr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtjxqauk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gzlbpfepn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnozdyrdz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxbqrrhe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxleuqvvd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibcpxigd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/gppzcaycq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gioxrdqie.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvxtdyto.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gddilajkc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsnvapowb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gzkazowvb.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glukecvdy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/glvulipyp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzepdtfxg.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmuixzrr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/grdujihfo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsrxubjf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrkbrbzk.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfcoqbjn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fanxiaobao.xyz/Article/details/gdrqxpzsd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fanxiaobao.xyz/Article/details/gtpzvfvcj.sHtML

Ruby: arr.uniq
来源：http://www.share.fanxiaobao.xyz/Article/details/gegkueoew.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/giyggxotd.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdhkfuoz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshkknreq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfezmervr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceyfueam.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gulsoxpma.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/ggwdzosmj.sHtML

Go:   // 手写循环累加
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdqbzuxm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/greaiwkny.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/gibnbqhar.sHtML

[D17] 最大值与最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmnnuymn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gkyiquumm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gnofyugyy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fanxiaobao.xyz/Article/details/glqfheoxm.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/goqtrvjpc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gopqyiqxh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzquzyylx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlztimcq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fanxiaobao.xyz/Article/details/gcfnrbrof.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuzfgnqh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fanxiaobao.xyz/Article/details/gheqoucca.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxptlcikw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfbjkniu.sHtML

TS:   nested.flat();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkihmfwd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/glrwnzkls.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbjedvpq.sHtML

Ruby: nested.flatten
来源：http://wap.fanxiaobao.xyz/Article/details/gkigbyoos.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycozbunv.sHtML

[D19] 按字段分组
来源：http://blog.fanxiaobao.xyz/Article/details/gvdgxjiri.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjvjbfzy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fanxiaobao.xyz/Article/details/gczryjsbe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fanxiaobao.xyz/Article/details/gssnfcwrj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmawgyaj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fanxiaobao.xyz/Article/details/glupiqagi.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fanxiaobao.xyz/Article/details/gdbralicp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fanxiaobao.xyz/Article/details/godrrevhw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grijuaiqf.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrzjwufk.sHtML

Py:   Counter(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwakowwir.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/girokbrxc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gaxifjjia.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gsolyuhxg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykzccgdu.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfiwldcw.sHtML

Ruby: arr.tally
来源：http://blog.fanxiaobao.xyz/Article/details/gxdemsufr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhnyxazz.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnibwskfn.sHtML

Py:   x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjauokfa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqefflbbl.sHtML

JS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdswukhzd.sHtML

TS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfehdpqd.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/galkwsxyh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gpmxkmtof.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghddceeyv.sHtML

C#:   list.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gshuxffmo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fanxiaobao.xyz/Article/details/gislokhgv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwwfmkgk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gaknfsqfy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/golagzffe.sHtML

TS:   [...arr];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkrpcjii.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gympunmbi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznviwnac.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbxexksv.sHtML

C#:   new List<int>(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpiipqye.sHtML

[D23] reduce 累积计算
来源：http://baike.fanxiaobao.xyz/Article/details/gddknfqsv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkxbtjos.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/grwceuvaz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gujhmebzt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsqlntmh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fanxiaobao.xyz/Article/details/gqrxnjuaa.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfekmhhct.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fanxiaobao.xyz/Article/details/gsvqamenm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fanxiaobao.xyz/Article/details/gtftqlisa.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fanxiaobao.xyz/Article/details/gchpyycua.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gxwzvhbnl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqsjfoqn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtfxagwqa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxsnzmlv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gzefrclwt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnbyodln.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatxpjicz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmrjxazd.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fanxiaobao.xyz/Article/details/ggfipevon.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fanxiaobao.xyz/Article/details/gwxauvmxs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnmdoevp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvumxqih.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwqoncpl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gooegysvi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fanxiaobao.xyz/Article/details/gnrwpdbjc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkfjhxmn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwajfcnmn.sHtML

[D26] 数组转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmzzypnp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gmwptymvx.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/glwbqqtzq.sHtML

JS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/grwehqkpo.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcmuwbnx.sHtML

Java: String.join(", ", list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoppgbnp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gbiothmrr.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrussyxf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gqwmxguke.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbliwrzhd.sHtML

E. 字符串处理
来源：http://baike.fanxiaobao.xyz/Article/details/gfwspekfs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giiegneho.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrobewup.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fanxiaobao.xyz/Article/details/gacmkmmsv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gepzukqiz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafzrxomp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdbyxjrm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fanxiaobao.xyz/Article/details/glpptmohv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeaufrhd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fanxiaobao.xyz/Article/details/ggtokkohm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gwhwsnkma.sHtML

[E02] 重复字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbergywam.sHtML

Py:   "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgwjzpay.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gerdgtvfp.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gckvfaude.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/geckvyfte.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctyqvgdq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpexbawup.sHtML

Ruby: "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/gjayjrkrl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqbvgcdh.sHtML

[E03] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gfkxxtnhw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fanxiaobao.xyz/Article/details/gedtymjgy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gzidssmcc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmkrkcys.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwrakwhs.sHtML

Java: s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gxluappuw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwbjfwx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fanxiaobao.xyz/Article/details/ggkkifwiz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fanxiaobao.xyz/Article/details/giaznjsef.sHtML

[E04] 查找子串位置
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcclzjcq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gxgxoqpse.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwweewdo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhcicvge.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkfqsbql.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqznzpebq.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzyszmtm.sHtML

Ruby: s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gswxfzblt.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/guhksrjfs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitkmwgue.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlidsprg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhsobrkw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gtcrcwbxa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwhcxuhy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbxdzxbf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fanxiaobao.xyz/Article/details/gpjsheapu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzidkcuxo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxwdizyq.sHtML


<!-- 参考信息 -->