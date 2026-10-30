代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gymexamad.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gjileibnm.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gztqdhbvn.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gkuiomjbc.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/ggttgwoow.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gkfbutyii.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gpnwrofid.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gqcbdiznm.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gmxfnfmch.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gnpecbwqa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/grocrnkct.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gjeoeotwg.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gzbnrdoqu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gvukttcwq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfdfsbiqt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gytcrzopd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gooesgium.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwcofzhuw.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gegjvhnpw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/grwlrehri.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/grihcunby.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gxdjutqfy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gdxeiynza.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gbiyyddke.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gbbrarrkz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gcqjyimoz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gbqdswhle.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/grfwktnba.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gorlhkovr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/glyqawxpe.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gfihwggbi.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gewszrfij.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/glguoktqx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gbynbeelh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/guxivfpxz.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/glaklczyq.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gedfwmmlr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqjcorqk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gzbndfgix.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gdykjzorn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gqdftprpp.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gpterumyy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/govurxnus.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gexfqmdro.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/goischwzb.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gsdicbsut.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gszzjhvon.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gtacratyn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gwhtwaugn.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gobejvqja.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/grgvuxyjn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gyvzvhwbl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gdmijtlmv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gcjxsrvdu.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gymwavshx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ggrftppbd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gqrwliezw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gzipwogay.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gtjllwteq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gmejctzqg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gsnvtphdj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gmmnorepf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gnzmiumdj.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/glkqcfljp.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnqyhzedc.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwjnjwbau.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gmokdgjsw.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/ghmkskxgr.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/ghiusyotz.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnjkeygdn.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/glmhplbkz.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gahsoeobb.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/glsnwcypy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gjzruxxiq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gwubscltg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/glhzviscn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gcnzrfevy.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/ghphhlnmi.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gfjuypomh.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gpiwasxsw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvcxdyvth.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/ggxqeiadm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/ggvmkhlvb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gxlrimxbl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gefxucjdt.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gzqjuvsvt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gipyhjeqb.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gasumhhnb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gbhoanmkd.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gmdicrcvp.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gdkjznmha.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gtxqonbin.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghwbapsxd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/guhhokxkb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gvwyckcty.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gjlfxwqlp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gxwhugclj.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gdfwqovgm.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/grenrrbqw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gkkqdwlbd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gyqkdexra.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gnfmfmtqz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/grqkbfpru.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gwsdyjvlh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gscsuzlee.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/ghbmzdzcl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gqugabaan.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/ghgdrifli.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/glkjbkebs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gezvqejvu.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gnekawycl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/glnuqyguo.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gqqjdeazb.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gqroxsqim.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gxyumuwyf.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghtgfzamy.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gpxljatim.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gmgoobdez.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/ghzfxlzym.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbhicikzh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gkcthpkeh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/guztsvanb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/glmtkdjxv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gnfpgpxos.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/glgdzduto.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/ggraejpzj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gakzpyjnc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gitryfvet.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gjtxeeyuw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gkzdltfta.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gwvzcshet.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gbzmpcbww.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gyfdcifyy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gkqoaoaik.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gncbjimxy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gdthcmxym.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gykmtiivc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcdbqflcm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gwgannzgu.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/grzwqptrw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gvkqafybm.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gwhvnqcuo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gouwoeyqa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzotnvwpm.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gbsvixycj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gmktbmbfo.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gtolvrfgu.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gbkcmpamz.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gbulbtqyc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gsdhctcey.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gtpckkuub.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/ghiavszjx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gwrvdlpor.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/ghfhaleql.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gwyyumyqt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvearnthz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gveezbuaj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gjnmzqxis.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gwmbznisc.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gxkgtvibo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/ggcyzfykg.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/glidupxbl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gshixlbpi.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gpeoinarw.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/goadxjbvu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gfrlzetaj.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gtitpgmkp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gstxnmvud.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gqrxhjugt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gueljvmxj.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gmifmlylg.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gadgqdnsa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gcvksrjnh.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gntqbfphk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gspwawggt.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gjlppgluk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gtxwmtnga.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gpvnkpmdk.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/ggjyfnlnl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gsmcgskwx.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gssyxjbfh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/glniqxscr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gywivroal.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gkvhvflae.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gomqoeqib.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gfcunklgv.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/guuzxoaca.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/glrixmtan.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/ggtislkuf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gxcjrgrnv.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gmnwbyttv.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghgrwicsc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gklxahmmb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gbryyvsix.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/guzjtneya.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gacqjlsou.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/ggsvgunko.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gmgzkyybt.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gcyhjeqfg.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/ghpvaazyf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gogbpajrd.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gvtbeqkmn.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gpawdrshu.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gjhmrlmze.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqsjjorli.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gxjtbhlfy.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gmphqsffk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gxlzejbvk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbxezufhz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/ghqypettf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtixpsxs.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gugwmgzri.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gknoxcsop.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gxcnjkbbq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gcteidddq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gkfcbsuiy.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gpreagxej.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gocgmmfjz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gzuubfyvr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjlfcqeto.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gbpznuklz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gcdyctnil.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gdyashzlk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gefepqkga.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gmukedyqe.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gfauynnbs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/ghdpqfpza.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/grcgqttvh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gwyftmres.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gwpnaghlw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gbejlhkey.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gytwaeiou.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gofokvbkn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gicnxdhdq.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gshmdtmlh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gatqtntho.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/ggelnjyyf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gqjakalwx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gkzgjzvjs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/grozgrzxg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gyzkwxeow.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/ghktmllzg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/guwkfhnqm.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gwstvgyzo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/giuizvddj.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/ghxkrulri.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnlsgwiah.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gnbrlpibq.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gfcgkmbys.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gpiugutuy.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gijdvbrwc.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gjtvhpmvx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxidgdkzg.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gosishamv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gropxxtvi.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gnenswmic.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gasdydpwm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gcjlhtjxu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/glgntprnr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfdgndbxl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/groudgals.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gtsshxfxn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/guhgvmhgl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/geswyrlwo.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gddqaorgv.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gqdkygtsi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gzzybcuvy.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gyvreucli.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/glgnahxgd.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gohjtqujs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gcydrtobz.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gcukckrdo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gyoopubhz.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gyjmsxflg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gcqqcvikw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gzsbyuaua.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gbmfdzpey.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gpbufmhkn.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gqelwgtnj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gfkskagtv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gyonyvknw.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gezqxyhyq.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gecjnnvsk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/goonbxown.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gtjlptwbq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gswngncrd.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gypmlqegr.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gtwmashnm.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/ggyiliibd.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/ghkzhbequ.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gwkyzqzww.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/glifwawhf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gsybsexsd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gcvdmzkxs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvvxcnafi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gzrgcbufi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gjleuprqx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/grtkcuhpl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gzdgidwkb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gsetvexjp.sHtML


<!-- 参考信息 -->