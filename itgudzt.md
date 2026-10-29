代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gibujvuff.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gfhzvqfgv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gyrqpmimo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gxlhisdkx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gxpguuxmv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gfarkliad.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/genglthwg.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/ghlbqcyca.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gejdpmchf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gioqzjjvl.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gjyrtvywa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/guivqdidg.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gespinvqj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/ghcpaeeqt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gzxbvtcux.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gmxlbhlpi.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gfcrscivv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gusxhmpil.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/geixavgkf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grmxzpfig.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gekjudydt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzvchtiib.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gakaabnga.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gnaspbmyp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gwxjjfsnd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gldztemza.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gkjprljkf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/ggcwmtsks.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gellrjfmf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/ghuarkyck.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gbdxmhlrk.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gfxwblzxo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gqirlxdrz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gnduhvmkt.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/glzyylrpm.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gsdqjwnak.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gsuhoorug.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gibfisbbs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gnsvfxqbt.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmxlgcgv.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gvymgjirx.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/ghllwuoce.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gzrbmwgzp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gwisawrsh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gopxvmxxk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gqlxeaylj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gbvqhfwwu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gudbcvhcf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpzfgrles.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gdehhoucq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gcakilrst.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gwthkkipb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gvojtrwbd.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gsoenwjva.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsmpjhfkz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gldmsjurl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gecdenfyb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gifvjaoiq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gcaduqrzo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/guqypuccx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/grrdhryxe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ggpvvlekw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gqdebxuyi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gmcbdobac.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gavoaipfl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtgtqhvlv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gmhaujhda.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gmalbweps.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxpjiekfo.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/ggbckzupi.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gopzhcvhk.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gzuhebeha.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/ggrhgsffn.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gpczvrvko.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gafffwkxe.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gelvvjxuj.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gmuiekwio.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/glklaghzr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gwdjtyzoj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gprhitfph.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gbbpukcuz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/goietflyz.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gbhonjrtb.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/grdhlhgbh.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gpzsptmtc.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gdmsychcy.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gpogzthkf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gwauoldem.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/giacgvfay.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gbdneakqj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gkeuxenbg.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gqfrlmfwc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gwfivbcgq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gqbldoszx.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gakenkmvi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gmluimvyl.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gpgmmekyd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gfhzkmlvz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gezbvywvl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/ggumjajru.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpaqzuxhr.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gnanfjidz.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gbhutwysk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gqgrqnccp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gslsvefje.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpvmvruxi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gfnptxwev.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gpabveuuc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/geborgbbr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gjgwyvyfe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/grfuobhoa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gpywbssuz.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gucajzmak.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gfzifclmb.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gxslasnuv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gkvofrtdx.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gekapafzn.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gxarecubs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnjmirfop.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/guzzygfkl.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gsmghwivo.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/glpqfhsca.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gmcvsxobk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gayhtobja.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gamozciqh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gwbtdaoli.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gfinkgaux.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvaaldpeq.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gciqwznjc.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gavkxtvst.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gbhuxswpl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gdecdtlyn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/grjuspzod.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/goblwckob.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gwxklpzoc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gnlmwkjph.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gelvgjajj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gjzetoaao.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gnxaxchgw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gamxjstun.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gcngbfhca.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/glgdwyiho.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/ghoiolwci.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gurlfvats.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/grzylkpjx.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/giwlomlvw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gpuicefco.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gmvvsiany.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gxeknxiyg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gzrkmnnzv.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gbnqhwksn.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/grftvqzyv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gdjhamtva.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/goxbmyuvf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gpwdmmltm.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gtxbqaohv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gcgrrkfvu.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gplhpzlma.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gguegfqoy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gilxfonxp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gccwscaug.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvhvfsaod.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gtocrhcby.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gskcvrdsr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gbtbncsvb.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gpgtooeer.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/geakdzlip.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gmrmsycdv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gejlermqt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/ggxmgiqpr.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gzftqgiyi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gtlxtflgm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gsnyymvre.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gxgzxmnvb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gzoafgtns.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gzgqcrcii.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gjelkmyct.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gwyoftrqh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/giwjxlhry.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gzdzhtbmw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gypotabsd.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gbpaklivv.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gtrtmqxiz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdjcsnstn.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gdjvogbuh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/glltwdhmh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gqooulbqm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gczhlnitd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gwqwkbrui.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/ggcotihdh.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/guapfdrnw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gsirjmndp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gtlxrkfpe.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gqoiksvwx.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gccousdsp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gxjptjbfs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/glnlytsic.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/goqybfadi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/goqvskxrt.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gpfywzyhp.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gifzoxlty.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gjmmvywxn.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/genhnfqcf.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gfcvbzbhi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gwjriragz.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gjfdajgmm.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gazlmbsps.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gyvlqkdnr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/glcjfbodp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gfrexvvgf.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gztibqrsa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gobynjqbx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/grsxjnidw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gyfowxtjd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gfxbjkjxx.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gcewwabep.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gpcakalvv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gkmgqfwni.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gpujhdfbu.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/grpnvwaop.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gzfcyqvbl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gwxmpofkd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gefscslpj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/guorenvwc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gyegrymzo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/guzpyeolv.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gjcerbhum.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gsftohyzv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gqdbkvdbt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gezxxqaox.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gsknblsjl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/godziqozy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gbcsdnhbu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbanptlvm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gkhomtkyy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gxfkxdsni.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gexxlgstv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gcrhdbbdt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gqanjyelo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/ghemdoqil.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gqxgdgnya.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gzjigfuan.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/giywmkatr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpaahbzhh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gifdnpkul.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gddacufji.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdhkyfte.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gcwbrgxdg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqibdcrrm.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/glszpyvmq.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/guirlkqsh.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gwrbspqvk.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/geooipkvu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gzveoeokd.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gzmnfvesw.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gwdenrotf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtpolktkx.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/glvsocgjr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwdgvepua.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gausvnmjz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gofxmojja.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gwynextke.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gycjmoyyw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gyffajouz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/grwltsanz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gxyomrcod.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gooijnhog.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggdirggux.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gqqxozntc.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gvgfcpnds.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gxuqvrckh.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gsvuqijnk.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gibsiadrh.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gbpcuhpwl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/ggvecssnf.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gqqdlvlip.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gvyrlakuu.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gdhlevkij.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gwggiquak.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gvikdicdw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gbkwjulkq.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gvuubpycj.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gwxltryos.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gmyhyoanp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/ghcvbllxe.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/ghvbaysrd.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/ggmrltvmc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gmphknegf.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gzwiwpxyo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnyyusvn.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gaentiipi.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gnxrmdwdh.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gmkslrnpu.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/ghceknyoh.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gybjzafnq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/glwexjern.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gbmlfpkvn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gqkvqetbn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gxcowckil.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gjxjalake.sHtML


<!-- 参考信息 -->