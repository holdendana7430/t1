代发 wailian999

find . -name "*.log" -type f
来源：http://hz.jiagoushi.top/gtarfjsrus.html

[R44] 按修改时间查找
来源：http://hz.birdmap.top/gtlinsdtbk.html

find . -mtime -7 -type f
来源：http://hz.jinyuanbaomall.cn/gtchnwanms.html

[R45] 批量删除
来源：http://hz.aizwys.cn/gtlqjdgxiw.html

find . -name "*.tmp" -delete
来源：http://hz.ydjk.org.cn/gtmnukkkfy.html

[R46] 递归替换文件内容
来源：http://hz.jinqigufen.top/gtkghlakze.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cqqwz.cn/gtstyjwcbd.html

[R47] sed 单行替换
来源：http://hz.wangdashe.top/gtzhqubsnt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtyzanhvkp.html

[R48] awk 取指定列
来源：http://hz.ybcxt.top/gtyxkpmusu.html

awk '{print $1, $3}' a.txt
来源：http://hz.guowangkeji.top/gthumiwrvo.html

[R49] awk 带条件
来源：http://hz.zhaomingkeji.xyz/gtaxaxbbwp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fengsongda.top/gtndqwnpya.html

[R50] awk 求和
来源：http://hz.wangdashe.top/gtnzveivci.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ppjwa.cn/gtjzigudwr.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtvaqatozx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dianchejie.cn/gtzzxhteaz.html

[R52] 统计行数
来源：http://hz.meibo888.top/gtecpuurwp.html

wc -l a.txt
来源：http://hz.ivvv.top/gtnerntbjm.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtniccmdcn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jyoumei.cn/gtlsjucizm.html

[R54] 比较两个文件
来源：http://hz.yj202588.top/gtoqvfnoqd.html

diff a.txt b.txt
来源：http://hz.jiagoushi.top/gtboqdxsdg.html

[R55] 压缩与解压
来源：http://hz.ehwqpu.com/gtbkmrvsai.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuxming.cn/gtljtsibxa.html

[R56] 远程拷贝
来源：http://hz.316326.xyz/gtteyqlqbv.html

scp file user@host:/path/
来源：http://hz.wangdashe.top/gtuickzfyo.html

[R57] 远程执行命令
来源：http://hz.quarkkingdee.top/gtenmozcbl.html

ssh user@host 'uptime'
来源：http://hz.redwolf501.top/gtxxsmbplj.html

[R58] 下载文件
来源：http://hz.shanyushiyangtech.top/gtgxkjapxi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuetiantiany.cn/gtvmavanqr.html

[R59] 发 POST JSON
来源：http://hz.chenzaomai.com/gtlmrlesxu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhongyouzk.top/gtufvbnkfi.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtnlyfjtma.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ywan-chungtsiang.top/gtmmojlvnl.html

[R61] 磁盘占用
来源：http://hz.shangyingyoupin.top/gtjmldgujr.html

df -h;  du -sh *
来源：http://hz.shuidangran.top/gtqvinaxio.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gtzvxxmeou.html

du -ah . | sort -rh | head -10
来源：http://hz.hfpthk.cn/gtmlwsboxu.html

[R63] 内存与进程
来源：http://hz.yueranfly.top/gtushibkde.html

free -h;  ps aux | grep nginx
来源：http://hz.hfpthk.cn/gtuzilwuca.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gtfqikkidn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yonumen.top/gtpvffpltn.html

[R65] 查看端口占用
来源：http://hz.dashuyun.cn/gtepwtchgg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xylfe.cn/gtmykmmjyg.html

[R66] 定时任务
来源：http://hz.mhx1999.top/gtrorvbcxf.html

crontab -e;  crontab -l
来源：http://hz.nwbrower.top/gtzwyouwou.html

[R67] 生成随机十六进制串
来源：http://hz.chenjidiqi.icu/gtkvqbhjkd.html

openssl rand -hex 16
来源：http://hz.ppjwa.cn/gtpbqymmqw.html

[R68] 计算文件校验值
来源：http://hz.yj20258888.top/gtrjzvrzui.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtiwiftcww.html

[R69] 生成随机密码
来源：http://hz.kuanghao11.cn/gtetjtopeq.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtmlrihxhn.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtxeoaqmdb.html

date +%s;  date -d @1700000000
来源：http://hz.chenlongwang.top/gtqiionevf.html

[R71] 日期格式化
来源：http://hz.shangyingyoupin.top/gtlvnrbyty.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.vqdsnc.cn/gtfzujdoav.html

[R72] 等待端口就绪
来源：http://hz.sxryk.cn/gtpbegtxfj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cdnleiting.top/gtgznuosrf.html

[R73] 分割大日志
来源：http://hz.dashuyun.cn/gtewbfeszr.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtmoloudwl.html

[R74] 批量重命名
来源：http://hz.havefunace.top/gtnlumegfp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hongshengwenyu.top/gtfocrxqqe.html

[R75] 导出环境变量
来源：http://hz.hnxiangtu.top/gtxljhkgii.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daxiang520.top/gtfxttoewl.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtttsjiqro.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtdejzaybx.html

[R77] 读取用户输入
来源：http://hz.tanke756.top/gtlriedzoq.html

read -rp "请输入: " ans
来源：http://hz.xuanzx.com/gtmdkezkyt.html

[R78] 交互式菜单
来源：http://hz.xuanzx.com/gtkxijffse.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.iojbl.cn/gtowedfnfb.html

[R79] 解析命令行选项
来源：http://hz.gaohongyu789.top/gttodxkadm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.vqdsnc.cn/gtjisynpdj.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangkeji.top/gtaedwsowp.html

time ./run.sh
来源：http://hz.xinyue.icu/gtxmnspmmt.html

================================================================================
来源：http://hz.daxiang520.top/gtbkvlwigh.html

S. C / C++ 专题
来源：http://hz.zhaomingkeji.xyz/gtaqtadvnb.html

================================================================================
来源：http://hz.c1oappe.top/gtzadabxta.html

[S01] C：Hello World
来源：http://hz.9152youxi.cn/gtdbsawihf.html

#include <stdio.h>
来源：http://hz.52xcode.cn/gtnwhshscq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jlsjyb.cn/gtenmzzcxw.html

[S02] C：变量与格式化输出
来源：http://hz.yuxming.cn/gtzayuwppa.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnqzz.top/gtfuaxxxpe.html

[S03] C：读入整数
来源：http://hz.zycfv.cn/gtdobynbqm.html

int x; scanf("%d", &x);
来源：http://hz.xuanzx.com/gtnblpglud.html

[S04] C：字符串复制
来源：http://hz.dianchejie.cn/gtetvbxxuu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinyuanbaomall.cn/gthxffxdxe.html

[S05] C：字符串长度
来源：http://hz.shuidangran.top/gtcczswjmg.html

strlen(s)
来源：http://hz.ydzc1.top/gtlseduxxw.html

[S06] C：字符串比较
来源：http://hz.yonumen.top/gtpjxmvhyt.html

strcmp(a, b) == 0
来源：http://hz.sysykeji.top/gtrrxrhpaj.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtqdyzqdlf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yuanzhike.top/gtlmkmwpmm.html

[S08] C：动态内存分配与释放
来源：http://hz.ehwqpu.com/gtkbacedop.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258888.top/gtnikauwze.html

[S09] C：结构体定义与初始化
来源：http://hz.yangfankeji.com/gtvegjfdke.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pycfn.com/gtjlfdngoe.html

[S10] C：指针与解引用
来源：http://hz.tianlin.xyz/gtzmjqkdoc.html

int *p = &a;  *p = 5;
来源：http://hz.birdmap.top/gtbqcqyfkq.html

[S11] C：逐行读文件
来源：http://hz.nanxinkj.top/gtmkxonjxv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sweek.top/gtyptgibcb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.316326.xyz/gtbbcscryj.html

fclose(f);
来源：http://hz.shanyushiyangkeji.top/gtuvdwuwtx.html

[S12] C：写文件
来源：http://hz.hywenlv.cn/gtosrnebuk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.havefunace.top/gtepsxfroh.html

[S13] C：宏定义
来源：http://hz.guowangkeji.top/gtxhomfcxd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.c1oappe.top/gtuddvslit.html

[S14] C：枚举
来源：http://hz.52xcode.cn/gtbjolmlkx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gotoacloud.top/gtgbhxfgyd.html

[S15] C：类型转换
来源：http://hz.ehwqpu.com/gtsnzliozo.html

(double) a / b
来源：http://hz.tian-w.cn/gtdcggftis.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gtlgajlgka.html

x |= (1 << 3);
来源：http://hz.hammf.cn/gtoeaeebls.html

[S17] C：安全拼接字符串
来源：http://hz.9152youxi.cn/gtdrapkuoi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258888.top/gtmpibellw.html

[S18] C：命令行参数
来源：http://hz.chenlongwang.top/gtpaobwqcf.html

int main(int argc, char **argv)
来源：http://hz.dianchejie.cn/gtmjmogowt.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gtkhkhtnao.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtdfkyakyq.html

[S20] C：二分查找
来源：http://hz.zhaomingkeji.xyz/gtnsusbcid.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gteacygwap.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtswrbshmc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gtdnithlsm.html

[S22] C：字符串转数字
来源：http://hz.ehwqpu.com/gtqqbquqyk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sxryk.cn/gtfqqiofgy.html

[S23] C：随机数
来源：http://hz.hysaishi.cn/gtpqptwmhz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xinyue.icu/gtvubbwnme.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangtech.top/gtyhfgfcxv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hfpthk.cn/gtytcqjozg.html

[S25] C：内存拷贝
来源：http://hz.fengsongda.top/gtuwwpsidz.html

memcpy(dst, src, n);
来源：http://hz.yj20258888.top/gtsqwwugfn.html

[S26] C：内存清零
来源：http://hz.gzhubu.top/gtdaqnoqbl.html

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangtech.top/gtawtbtynl.html

[S27] C：定义常量
来源：http://hz.hnqzz.top/gtmnamwfck.html

const double PI = 3.14159;
来源：http://hz.bjfxy.top/gtrephzsug.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gtkmbimwij.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtbtfjtxwg.html

[S29] C：变参函数
来源：http://hz.ydzc1.top/gtkrjpuuhp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.mhx1999.top/gtjapadwen.html

[S30] C：头文件保护
来源：http://hz.jlsjyb.cn/gttjyqkimy.html

#ifndef X_H
来源：http://hz.xuetiantiany.cn/gtsqnvggyn.html

#define X_H
来源：http://hz.feifeiyinyue.top/gtudrrlfvx.html

#endif
来源：http://hz.yuxming.cn/gtebmvdxpp.html

[S31] C++：Hello World
来源：http://hz.svipenyu.cn/gtmhvlwxwo.html

#include <iostream>
来源：http://hz.cqqwz.cn/gtrsegzbqb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jiagoushi.top/gtazasyrxi.html

[S32] C++：字符串
来源：http://hz.cdnleiting.top/gttxgmhmlc.html

std::string s = "hi";  s += "!";
来源：http://hz.ivvv.top/gtvnynurqi.html

[S33] C++：vector 增删
来源：http://hz.hnqzz.top/gtcispfjua.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xylfe.cn/gtsjvuputl.html

[S34] C++：遍历 vector
来源：http://hz.gogol.net.cn/gtnnzvnikc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangshuangyany.cn/gttdwubmcc.html

[S35] C++：map
来源：http://hz.yj20258.top/gtvvkfmlth.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtqhlbuacw.html

[S36] C++：unordered_map
来源：http://hz.ivvv.top/gtbxiimbdy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtjnbjaseu.html

[S37] C++：set
来源：http://hz.c1oappe.top/gtktjrljuq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtazkakuzi.html

[S38] C++：排序
来源：http://hz.hammf.cn/gtsciuorzv.html

std::sort(v.begin(), v.end());
来源：http://hz.aibaodan.cn/gtysatiugj.html

[S39] C++：自定义比较器排序
来源：http://hz.xinyue.icu/gtnhchwcyh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.9152youxi.cn/gtzljvabnd.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtymjbsuic.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sysykeji.top/gtvgzljaki.html

[S41] C++：类与构造函数
来源：http://hz.xylfe.cn/gtrnipjrax.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gzhubu.top/gtbvoeadfp.html

[S42] C++：继承与虚函数
来源：http://hz.shanyushiyangkeji.top/gtvwqtxgml.html

class B : public Base { public: void f() override {} };
来源：http://hz.sweek.top/gtwrrcswgh.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gtylckpvze.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj202588.top/gtwftaxfel.html

[S44] C++：引用传参
来源：http://hz.daria6918.cn/gtjoqoeuxp.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gtgriqqgyc.html

[S45] C++：lambda
来源：http://hz.sweek.top/gtxpofwesz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cheryme.top/gtjndmyscf.html

[S46] C++：函数模板
来源：http://hz.jiagoushi.top/gthilzhots.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xingfuxueyuan.xyz/gtxjnveark.html

[S47] C++：结构化绑定遍历
来源：http://hz.jyoumei.cn/gtoucxzphv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtebyepqrw.html

[S48] C++：逐行读文件
来源：http://hz.aizwys.cn/gtvhhkzely.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gtykjopkrg.html

while (std::getline(in, line)) { }
来源：http://hz.wangshuangyany.cn/gtqdlwodvg.html

[S49] C++：写文件
来源：http://hz.yuanzhike.top/gtemgdwhap.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtnavracjj.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtimadwelc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnxiangtu.top/gtbxowqtdd.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gttchzqrbo.html

static_cast<double>(a) / b
来源：http://hz.jlsjyb.cn/gtftwmmzyl.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258.top/gtrtifrhbg.html

int size() const noexcept { return n_; }
来源：http://hz.nanxuanxn.top/gtjrditbyg.html

[S53] C++：移动语义
来源：http://hz.yanxiufei.cn/gtibrhehax.html

std::vector<int> w = std::move(v);
来源：http://hz.gogol.net.cn/gtbtmntntj.html

[S54] C++：异常处理
来源：http://hz.ybcxt.top/gtsmnwzwpj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gotoacloud.top/gtetrumbny.html

[S55] C++：结构化绑定
来源：http://hz.yvedp.cn/gthelpwwff.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnxiangtu.top/gtmwxnjptc.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtfprfpdxn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtsnpeozsg.html

[S57] C++：编译期常量
来源：http://hz.zhixingplan.top/gthsoavhcb.html

constexpr int N = 10;
来源：http://hz.52xcode.cn/gtcskunlxe.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gtmcbdvcac.html

namespace ns { int f() { return 1; } }
来源：http://hz.yonumen.top/gttnnkpitc.html

[S59] C++：静态断言
来源：http://hz.tanke756.top/gtlgvjheok.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nwbrower.top/gtqknvvfcr.html

[S60] C++：遍历并删除元素
来源：http://hz.shuidangran.top/gtveskmeyy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangshuangyany.cn/gtrodzxjhh.html

================================================================================
来源：http://hz.chenlongwang.top/gtwxqjcexi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtcdazgmol.html

================================================================================
来源：http://hz.zdqjudy.top/gtccfkjgzb.html

[T01] Kotlin：Hello World
来源：http://hz.jianghu66.top/gtjohiztmr.html

println("Hello")
来源：http://hz.yj20258.top/gtwqxwwydf.html

[T02] Kotlin：变量
来源：http://hz.guannengcc.top/gtenlfmsxw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cheryme.top/gtuxckrjyu.html

[T03] Kotlin：字符串模板
来源：http://hz.gzhubu.top/gtynlgvywt.html

"值: $b"
来源：http://hz.xuetiantiany.cn/gtomirisut.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gtnecoxser.html

val n: String? = null;  n?.length
来源：http://hz.zhengqikj.top/gthadsxvma.html

[T05] Kotlin：when 表达式
来源：http://hz.yonumen.top/gtnouzipzj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daria6918.cn/gtnzeeukiy.html

[T06] Kotlin：集合映射
来源：http://hz.xinyue.icu/gtkkjpzolx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenzaomai.com/gtexxnrcaz.html

[T07] Kotlin：集合过滤
来源：http://hz.gotoacloud.top/gtxoexugjd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhengqikj.top/gtjttpagpq.html

[T08] Kotlin：数据类
来源：http://hz.aizwys.cn/gtfuzdevtq.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtcfcxmajy.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigfzy.top/gtdqzimbmn.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gtdfcldnyg.html

[T10] Kotlin：默认参数
来源：http://hz.tanke756.top/gtnaheimtf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtrazbxapl.html

[T11] Kotlin：协程
来源：http://hz.fengsongda.top/gtijgnxcim.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydjk.org.cn/gtiurtxris.html

[T12] Kotlin：解构声明
来源：http://hz.jinqigfzy.top/gtlnfrzdpc.html

val (a, b) = Pair(1, 2)
来源：http://hz.hnxiangtu.top/gtqcrglykz.html

[T13] Kotlin：只读 Map
来源：http://hz.jlsjyb.cn/gteokujybi.html

val m = mapOf("a" to 1)
来源：http://hz.quarkkingdee.top/gtudbkkarz.html

[T14] Kotlin：循环
来源：http://hz.zhixingplan.top/gtcxdoxnrq.html

for (i in 1..10) println(i)
来源：http://hz.daria6918.cn/gttlmtttqw.html

[T15] Kotlin：接口
来源：http://hz.tanke756.top/gttjrzbnxn.html

interface Shape { fun area(): Double }
来源：http://hz.zhengqikj.top/gttpmhiwvq.html

[T16] Swift：Hello World
来源：http://hz.gogol.net.cn/gtmeaiislz.html

print("Hello")
来源：http://hz.pycfn.com/gtblpifsph.html

[T17] Swift：变量与常量
来源：http://hz.fengsongda.top/gtgjgvqotp.html

var a = 1;  let b = 2
来源：http://hz.jiagoushi.top/gthqotgqqy.html

[T18] Swift：字符串插值
来源：http://hz.zhoulong.xyz/gtjgervcsy.html

"值: \(b)"
来源：http://hz.ehwqpu.com/gttxqmziqg.html

[T19] Swift：可选绑定
来源：http://hz.gaohongyu789.top/gtuojxvxwg.html

if let n = opt { print(n) }
来源：http://hz.zhaomingkeji.xyz/gtrmfkordq.html

[T20] Swift：数组操作
来源：http://hz.cqqwz.cn/gtctrszgaz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jlsjyb.cn/gtonbvodfv.html

[T21] Swift：遍历
来源：http://hz.chenzaomai.com/gtllrmofqn.html

for x in a { print(x) }
来源：http://hz.316326.xyz/gteaseppnd.html

[T22] Swift：字典
来源：http://hz.c1oappe.top/gtcygdokic.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gtqwxalxpl.html

[T23] Swift：函数
来源：http://hz.fzhhl.top/gtzslskrqr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cucudq.cn/gtjfoavtgt.html

[T24] Swift：闭包
来源：http://hz.daxiang520.top/gtyxlyocsw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xziqi.cn/gtivkudfbg.html

[T25] Swift：结构体
来源：http://hz.chenzaomai.com/gtlouoqqif.html

struct P { var x: Int }
来源：http://hz.cheryme.top/gtbcqcbsoh.html

[T26] Swift：类与重写
来源：http://hz.xingfuxueyuan.xyz/gttkapxett.html

class A: Base { override func f() {} }
来源：http://hz.9152youxi.cn/gtwgetbhth.html

[T27] Swift：错误处理
来源：http://hz.52xcode.cn/gtdkrokstm.html

do { try f() } catch { print(error) }
来源：http://hz.sufxvd.cn/gtwxpcbnmh.html

[T28] Swift：枚举
来源：http://hz.jinqigufen.top/gtknmbflof.html

enum Color { case red, green }
来源：http://hz.yueranfly.top/gtzomohrhi.html

[T29] Swift：guard 提前返回
来源：http://hz.52xcode.cn/gtkhhttedl.html

guard let x = opt else { return }
来源：http://hz.hysaishi.cn/gtjnqpcply.html

[T30] Swift：协议
来源：http://hz.shzxlz.cn/gtrofcdkwc.html

protocol Shape { func area() -> Double }
来源：http://hz.zhengqikj.top/gtgraxyyyh.html

[T31] Lua：Hello World
来源：http://hz.yanxiufei.cn/gtqhigpfbi.html

print("Hello")
来源：http://hz.shuidangran.top/gtdvoxkcgp.html

[T32] Lua：局部变量
来源：http://hz.jyoumei.cn/gtczzpcmxt.html

local a = 1
来源：http://hz.yvedp.cn/gtaafbpgqt.html

[T33] Lua：表（数组）
来源：http://hz.birdmap.top/gtiyvvfgig.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hywenlv.cn/gtxwbssmil.html

[T34] Lua：遍历表
来源：http://hz.chenlongwang.top/gtckplnbjz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj20258888.top/gtdmzqdewv.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gttwhatlhh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zdqjudy.top/gtedbnelqv.html

[T36] Lua：函数
来源：http://hz.xuanzx.com/gtvvazasag.html

function add(a, b) return a + b end
来源：http://hz.havefunace.top/gtfquuwprg.html

[T37] Lua：字符串拼接
来源：http://hz.nwbrower.top/gtfueozbxi.html

"a" .. "b"
来源：http://hz.xuetiantiany.cn/gttjkrfsxm.html

[T38] Lua：条件
来源：http://hz.vqdsnc.cn/gtmbnxnwji.html

if x > 0 then print("正") end
来源：http://hz.nanxinkj.top/gtooeomiry.html

[T39] Lua：模式匹配
来源：http://hz.sxryk.cn/gtraxmonbo.html

string.find(s, "%d+")
来源：http://hz.0kj1m.cn/gtvmbljooq.html

[T40] Lua：元表
来源：http://hz.ywan-chungtsiang.top/gtwpesaxqj.html

setmetatable({}, { __index = base })
来源：http://hz.smart0.xyz/gtpbqyuxtk.html

[T41] Perl：Hello World
来源：http://hz.zhijiandao.cn/gtdnyxywym.html

print "Hello\n";
来源：http://hz.snrcjt.cn/gtxxvqqwbk.html

[T42] Perl：变量类型
来源：http://hz.ppjwa.cn/gthiakfvla.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ehwqpu.com/gtbsqbsbqj.html

[T43] Perl：字符串插值
来源：http://hz.chenzaomai.com/gtxbztjymf.html

"值: $a"
来源：http://hz.316326.xyz/gthurjsqbc.html

[T44] Perl：条件
来源：http://hz.shanyushiyangkeji.top/gtyejqpmum.html

if ($a > 0) { print "正"; }
来源：http://hz.birdmap.top/gtfoewuncl.html

[T45] Perl：数组遍历
来源：http://hz.jqgufenzy.top/gtjetiesub.html

for my $x (@arr) { print $x; }
来源：http://hz.dianchejie.cn/gtrojfnrtf.html

[T46] Perl：哈希操作
来源：http://hz.0kj1m.cn/gtgrxrpwja.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shanyushiyangkeji.top/gtydwnpjnf.html


<!-- 参考信息 -->