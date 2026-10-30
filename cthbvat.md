代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gaojtxqax.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/glonksfrb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/geaqszrkm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/ghmbgxwgb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/ggvoyycvn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gktucubzr.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gyqxenvad.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/ghacwxevh.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/ghtxhsxyh.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gkvxegnri.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gqqlvzghd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gxuwjvxvg.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gujmfyebs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gyxrilebr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gsgddsuqf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gqpqgnmvb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gjizcfifk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/ggtsqfnjc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/grptevtnz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gomldsqvv.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gioxaflml.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwohwbyij.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gpxmcnxqx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gazetzvdg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gzfffatdy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gbvrqgmop.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gngwscymh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gsknbvljm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gqckwoccc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gmiiypgpx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gcxxwjigw.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/glvhfllse.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gxkplfhuj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gskcbkpbm.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gdruotkdw.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gycsyddyc.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwdolgymy.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gekfoupde.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gyuqtzkga.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gkajieuwx.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gzjcgneaf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ggpzejmmm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmeemkj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/ghslkgrge.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gpvbnvyud.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmfsyrogh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gqhhgglos.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/glopmshoa.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/geswqeznk.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gbdcfnrev.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gompsitud.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gnipyxemw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/galspqckx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gtuxyrjte.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gszjqkxxc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gkwsyjdeo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gkngyqoup.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/glfqxjhwt.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gsdytfbov.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gawpekxyp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gnzrgfxaa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gdyxbvtqv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gkiurdmbu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/guqqxlvyi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gsmifhxbt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gxpwfkvhh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gmwxathym.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gswnobawd.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gsgjujvda.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gunneveft.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gvnbnwgxr.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gtmfliwzt.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gungqavao.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gjruesujx.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/ghreytdqw.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gmswdnwih.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/glzifyaud.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gzolkgwae.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/ggtaxkxzr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gxjzghmjb.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/grhwkhlbv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/golkuedow.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/grothifos.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gwgruriyl.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gzjpkygtm.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gzngkuhrz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gxwzmhfbu.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/grydriihi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gywtkbnyv.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gpvmgtuuo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gtydqstwk.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gjqpgzbxg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gdzvgnvcy.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gsnlfbocr.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gihjzevra.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gtbtidcpq.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gusdoyxwx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/ggttusfdb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gzbcjldeb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gsoftgjii.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtnfslxao.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/grhbmkyxb.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gaoznlmrp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/glnjgkctr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gvtovntgs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gdnzticgc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gcqrtsutr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/giwsmafsw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/ggaqtcdnu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gomwredwb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gwlwdmove.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gudirnhyi.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gztjnwysl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gzttckiku.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/grvhamsen.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gergwmdij.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/geteaqjug.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gnptrskya.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbuibyuqo.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/ghjnnsors.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gxgfryvwa.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/grkrcjmtc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gqjrgteey.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/grlcogohh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/girtuasej.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmuzhwwpu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gyckwgmie.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gcqgetxvu.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gpstcnnok.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gqiwvetrq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gaaphscnd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/glbhvutnf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gqnztbxbg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gccgjtzvu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gvbzhaogy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gfsdsrajp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/grozvwzlr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gialavjpq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gtifllems.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gwheacuce.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gqwftufjz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gvmdmlzrs.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gihlztdmo.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gzeamjeia.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/glrymscaa.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gybcijvdu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxmpifyhu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/guibrrvic.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gnpsrgkkf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gdlejslqp.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/goqgyitgt.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gzfaodpou.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gpxhuqhgd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gdhvrlepi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gbwoqqgfv.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gspydbykx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gubfsjemh.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gqyultdcz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gwilfydmh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwvcumqhp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gkbvpyahh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gixtbgqjq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gljbcrldy.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gcsofsddo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gxmjdzqcz.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gnopubscb.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gxcgzvfxj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfxitfuou.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/giqctjfcj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gnnnterpz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gdxpcxapn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gowbyslql.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gwcrtmras.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gnjigwczk.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gfomrxrim.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gqobynped.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gsuzmhllj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gzajxezon.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gdkywvndh.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gfbwyavdh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/grnvyvfll.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gkwxtigoy.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gtkpouiez.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gjoswbmhb.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gtdjnyufi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gfrihkalc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gahwbzeng.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/giilkyuwr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/ghjtraoob.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/grmhvtadp.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/guoojkqgm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/ggorqhayh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gtjxmjznp.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gcqlcfkkj.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gaeoumbuf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gecxcctch.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gcchokppp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/ghlmdsxnk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gtcunejmi.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gjiuoxpup.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gpehdkadt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gulgaxwlj.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/goxweirzj.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gwxntukyj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gdqbxuaza.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gphhbvvzu.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvytqgpds.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gzanckgqc.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gruxxdlmu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/giwcztgnj.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gfxjwkefy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gwttaxqfk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gylfriimo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/grlybfyel.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gwfjnacdo.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gugjpokoe.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzjmatqhk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/glqxckikm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gtmaptlpb.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/ggywaoxay.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/ghtoybxuo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdhfvhwtl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gqartjryy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggvhaanbz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyjqcdxgs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gglpwvmgn.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/grwlpdonl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/ggprzqzvn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gmanikqxr.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gdkngbfcb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gqsmyxwgx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gtzmmnyll.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gcbdhgcth.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjysdwhdl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/giansrfjg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/giriealio.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gxdibhxxx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gcfvbuvvo.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gjtzeyndq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gifjbefma.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gceekgnty.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gqnkonzxf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gkzeaknaq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gxkgzpohx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gfgeihkfz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gdxeicvbk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gynxqroov.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjfcfwofb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gztqcsfys.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gszlodfvi.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gdpdsmxqb.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gmhjdurur.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gyqeqjnhv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gxakgsztp.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gcqzmgahj.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gxsntfcbw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gltpcdmvj.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/grumvaoqq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvgdyzczq.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/guaqkaibo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gnthzvuby.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gbfyiunxp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/glzsrkzil.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gvisktwud.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gqcphehvc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gyjpytcim.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gpcdsiyea.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfxrkkpce.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/glshzkvre.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gedxfcarv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzxgcgjde.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gskmdqxrl.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gkwqibagp.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gvnfoyzst.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gfmycjcjh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gfyjpjwdx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gxazplcpr.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/glqjmltvb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gtbnsqrqp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gcnxchjqt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnryitakg.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gqtyrfwvd.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/givtsfrog.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gpdlqizar.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gjyadougu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gztvkydys.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gggorajtv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/ganbvhhre.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gqpvlzjib.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gdrtascsi.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/glmgcvott.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gpwewnsca.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/ginsykqfj.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gdjuytrsp.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ghqpcpfeh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gvrkifgbl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gyzjwveru.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gcxthokdh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gcngbkilk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gufwfdyaj.sHtML


<!-- 参考信息 -->