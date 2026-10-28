代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenzaomai.com/gtuuqlrjei.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtnxapiwxo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hfpthk.cn/gtoaliraes.html

[R51] 排序去重取前几
来源：http://hz.svipenyu.cn/gteafxtgok.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dashuyun.cn/gtsafyllxa.html

[R52] 统计行数
来源：http://hz.zhijiandao.cn/gtbgpoiafo.html

wc -l a.txt
来源：http://hz.0kj1m.cn/gtszcvhzde.html

[R53] 查看文件头与实时尾
来源：http://hz.zhaomingkeji.xyz/gtyohtdbxl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jlsjyb.cn/gtrqafktnw.html

[R54] 比较两个文件
来源：http://hz.yanxiufei.cn/gtygigaulr.html

diff a.txt b.txt
来源：http://hz.hongshengwenyu.top/gtzreliazw.html

[R55] 压缩与解压
来源：http://hz.nanxinkj.top/gtiuqkebmz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.9152youxi.cn/gtoxuvezax.html

[R56] 远程拷贝
来源：http://hz.jqgufenzy.top/gtdgcvbsoc.html

scp file user@host:/path/
来源：http://hz.jinyuanbaomall.cn/gtceqkvjlg.html

[R57] 远程执行命令
来源：http://hz.zhiwuduotai.top/gtqbczswmd.html

ssh user@host 'uptime'
来源：http://hz.hammf.cn/gthortznxt.html

[R58] 下载文件
来源：http://hz.havefunace.top/gtooccxtqm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxinkj.top/gtwyvrnlbh.html

[R59] 发 POST JSON
来源：http://hz.xuetiantiany.cn/gtdiugqssx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ivvv.top/gtvetjokgz.html

[R60] 只看 HTTP 状态码
来源：http://hz.cucudq.cn/gthtsfgbfh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydjk.org.cn/gtclcsclen.html

[R61] 磁盘占用
来源：http://hz.smart0.xyz/gtbpxrbegn.html

df -h;  du -sh *
来源：http://hz.feifeiyinyue.top/gtbstxdrcc.html

[R62] 找最占空间的文件
来源：http://hz.yanxiufei.cn/gtadqtadnp.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtyinrbdad.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtiouhcgln.html

free -h;  ps aux | grep nginx
来源：http://hz.sufxvd.cn/gtqescqexo.html

[R64] 结束进程
来源：http://hz.jinqigufen.top/gthdzuvotc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.svipenyu.cn/gthxpsufdx.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtwyjvqqwb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258.top/gthdclqusk.html

[R66] 定时任务
来源：http://hz.mhx1999.top/gtzmzscnkr.html

crontab -e;  crontab -l
来源：http://hz.zhaomingkeji.xyz/gtcsxgcilu.html

[R67] 生成随机十六进制串
来源：http://hz.zycfv.cn/gtfroxuayz.html

openssl rand -hex 16
来源：http://hz.zdqjudy.top/gtdfltpzwy.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtbwstuqod.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nwbrower.top/gtcikfjkyq.html

[R69] 生成随机密码
来源：http://hz.zhongyouzk.top/gtsmmfkokd.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuxming.cn/gtzmmlhbsb.html

[R70] 时间戳与互转
来源：http://hz.shangyingyoupin.top/gtspnanntl.html

date +%s;  date -d @1700000000
来源：http://hz.gotoacloud.top/gtlrowrutp.html

[R71] 日期格式化
来源：http://hz.hfpthk.cn/gtxpnfxgcx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtjwhblblj.html

[R72] 等待端口就绪
来源：http://hz.ywan-chungtsiang.top/gthbfpkziq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtcytghfoa.html

[R73] 分割大日志
来源：http://hz.aibaodan.cn/gtoievybig.html

split -l 1000 big.log part_
来源：http://hz.hywenlv.cn/gtgocvcuzl.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gthvplqwng.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenlongwang.top/gtcgpzvwzy.html

[R75] 导出环境变量
来源：http://hz.yvedp.cn/gtmeksklea.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtkezmruab.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtgyybpygt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtuvwrzsgb.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtzslqlqbu.html

read -rp "请输入: " ans
来源：http://hz.sufxvd.cn/gtpreqjjsb.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gthuwsqfrz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gthydskxdh.html

[R79] 解析命令行选项
来源：http://hz.pengpengdd.cyou/gtyjjqnxve.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sufxvd.cn/gtronvpxob.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxinkj.top/gtpdicbwme.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gtpmbsutmd.html

================================================================================
来源：http://hz.gaohongyu789.top/gtktauowjq.html

S. C / C++ 专题
来源：http://hz.jiagoushi.top/gtgkfnissj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtgsaljwhy.html

[S01] C：Hello World
来源：http://hz.daxiang520.top/gtlhxnwrlw.html

#include <stdio.h>
来源：http://hz.snrcjt.cn/gtvimuoqka.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.iojbl.cn/gtyigasazy.html

[S02] C：变量与格式化输出
来源：http://hz.xylfe.cn/gtbmxfmoed.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gthnsatajx.html

[S03] C：读入整数
来源：http://hz.dianchejie.cn/gtqibstkrk.html

int x; scanf("%d", &x);
来源：http://hz.316326.xyz/gtcymawmny.html

[S04] C：字符串复制
来源：http://hz.svipenyu.cn/gtetynuiwi.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.0kj1m.cn/gtgppiloza.html

[S05] C：字符串长度
来源：http://hz.yangfankeji.com/gtgbqehrwc.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtzjkrzbnt.html

[S06] C：字符串比较
来源：http://hz.wangdashe.top/gtrznrxriz.html

strcmp(a, b) == 0
来源：http://hz.jianghu66.top/gtmacjmqdu.html

[S07] C：数组遍历求和
来源：http://hz.yj202588.top/gtancvowhy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xziqi.cn/gtoljxpdtk.html

[S08] C：动态内存分配与释放
来源：http://hz.feifeiyinyue.top/gtlhjunaio.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxuanxn.top/gtguqghblh.html

[S09] C：结构体定义与初始化
来源：http://hz.gotoacloud.top/gtvkbssyzk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtrbkbarsm.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtqtprdxpz.html

int *p = &a;  *p = 5;
来源：http://hz.xziqi.cn/gtvikytkzm.html

[S11] C：逐行读文件
来源：http://hz.ydjk.org.cn/gtlhoupcsu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jlsjyb.cn/gtynmylzmo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.daxiang520.top/gtwqpgrajc.html

fclose(f);
来源：http://hz.vqdsnc.cn/gtejalwwtq.html

[S12] C：写文件
来源：http://hz.sxryk.cn/gtvfwvvvkt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xinyue.icu/gtlruxvyhr.html

[S13] C：宏定义
来源：http://hz.c1oappe.top/gtilxyogqw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenjidiqi.icu/gtyrkuzapm.html

[S14] C：枚举
来源：http://hz.cheryme.top/gtvhehuksa.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hongshengwenyu.top/gtdwabsphf.html

[S15] C：类型转换
来源：http://hz.dianchejie.cn/gtdynxrfqy.html

(double) a / b
来源：http://hz.cqqwz.cn/gtqejultdp.html

[S16] C：位操作置位
来源：http://hz.aibaodan.cn/gtjwawokrc.html

x |= (1 << 3);
来源：http://hz.zhaomingkeji.xyz/gtxrcvkkci.html

[S17] C：安全拼接字符串
来源：http://hz.xinyue.icu/gtrexouliq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhongyouzk.top/gtgkdskbov.html

[S18] C：命令行参数
来源：http://hz.birdmap.top/gtdekyouqc.html

int main(int argc, char **argv)
来源：http://hz.zhijiandao.cn/gtqzhnswrc.html

[S19] C：快速排序
来源：http://hz.shangyingyoupin.top/gtkkpkohng.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtrguyrmsp.html

[S20] C：二分查找
来源：http://hz.quarkkingdee.top/gtzkzmffcg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtzuakiwrr.html

[S21] C：字符类别判断
来源：http://hz.316326.xyz/gtpfsqiacz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.9152youxi.cn/gtwadznqdx.html

[S22] C：字符串转数字
来源：http://hz.bjfxy.top/gtsquozmft.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xylfe.cn/gtenwicren.html

[S23] C：随机数
来源：http://hz.jiagoushi.top/gtupgjdbdv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.svipenyu.cn/gttytegbrq.html

[S24] C：获取本地时间
来源：http://hz.gogol.net.cn/gticpuuttv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhongyouzk.top/gttsinguve.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gttzcgvjch.html

memcpy(dst, src, n);
来源：http://hz.xingfuxueyuan.xyz/gtisfzblef.html

[S26] C：内存清零
来源：http://hz.jlsjyb.cn/gtqwzvbmkz.html

memset(a, 0, sizeof a);
来源：http://hz.jyoumei.cn/gtvexlchiz.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtdwkncwsc.html

const double PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gtxzoezrnb.html

[S28] C：静态变量
来源：http://hz.52xcode.cn/gtfjtntpzt.html

static int counter = 0;
来源：http://hz.yueranfly.top/gtlbpxscwj.html

[S29] C：变参函数
来源：http://hz.aibaodan.cn/gtqdfvixvj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hfpthk.cn/gtbokpxtwn.html

[S30] C：头文件保护
来源：http://hz.xinyue.icu/gtnwiiayjq.html

#ifndef X_H
来源：http://hz.daria6918.cn/gtyetvhwuw.html

#define X_H
来源：http://hz.svipenyu.cn/gthiamuxko.html

#endif
来源：http://hz.jinyuanbaomall.cn/gtxhxwoivb.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtxyehbzrd.html

#include <iostream>
来源：http://hz.wangshuangyany.cn/gtknmucygb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenjidiqi.icu/gtddyyoakx.html

[S32] C++：字符串
来源：http://hz.aizwys.cn/gtuswcbqhm.html

std::string s = "hi";  s += "!";
来源：http://hz.svipenyu.cn/gtmmxhumif.html

[S33] C++：vector 增删
来源：http://hz.jiagoushi.top/gtdilndsye.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jianghu66.top/gtplkidfhy.html

[S34] C++：遍历 vector
来源：http://hz.yanxiufei.cn/gtwgclrosn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hammf.cn/gtjpjvnnff.html

[S35] C++：map
来源：http://hz.smart0.xyz/gtwawkwxzo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtihqyyoqw.html

[S36] C++：unordered_map
来源：http://hz.ivvv.top/gtidwurywj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtmdfcnwzn.html

[S37] C++：set
来源：http://hz.chenjidiqi.icu/gtorzjpxna.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gzhubu.top/gtxoviihcu.html

[S38] C++：排序
来源：http://hz.bjfxy.top/gteeaguutz.html

std::sort(v.begin(), v.end());
来源：http://hz.yonumen.top/gtetdfywgm.html

[S39] C++：自定义比较器排序
来源：http://hz.sweek.top/gtvunzhtpa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhaomingkeji.xyz/gtrusnzgfe.html

[S40] C++：查找元素
来源：http://hz.cucudq.cn/gtfdnswmhp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.meibo888.top/gtmxxtjmsa.html

[S41] C++：类与构造函数
来源：http://hz.wangdashe.top/gtsdvrmgfk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zdqjudy.top/gtoiwaijzo.html

[S42] C++：继承与虚函数
来源：http://hz.xziqi.cn/gtqlkvqyid.html

class B : public Base { public: void f() override {} };
来源：http://hz.tian-w.cn/gtvnvzzqoo.html

[S43] C++：智能指针
来源：http://hz.meibo888.top/gtjquacqqo.html

auto p = std::make_unique<int>(5);
来源：http://hz.daxiang520.top/gtbzcphwjg.html

[S44] C++：引用传参
来源：http://hz.zdqjudy.top/gtfxxaonds.html

void inc(int &x) { ++x; }
来源：http://hz.yanxiufei.cn/gtwtzwomuf.html

[S45] C++：lambda
来源：http://hz.xziqi.cn/gtdxturqfk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj20258888.top/gtwmcwxzdx.html

[S46] C++：函数模板
来源：http://hz.zycfv.cn/gtagfvlfzj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtmemoxtxp.html

[S47] C++：结构化绑定遍历
来源：http://hz.hammf.cn/gtifbtistz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gotoacloud.top/gtsdvutekd.html

[S48] C++：逐行读文件
来源：http://hz.9152youxi.cn/gthktmqcwk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gzhubu.top/gtqmdhraey.html

while (std::getline(in, line)) { }
来源：http://hz.jqgufenzy.top/gtzmijtkgd.html

[S49] C++：写文件
来源：http://hz.fzhhl.top/gttczouraq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhixingplan.top/gtvijmxzlo.html

[S50] C++：格式化数字
来源：http://hz.xylfe.cn/gtgshyfprq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jlsjyb.cn/gtgqcgzsbm.html

[S51] C++：显式类型转换
来源：http://hz.kuanghao11.cn/gtfzlbfezb.html

static_cast<double>(a) / b
来源：http://hz.yvedp.cn/gtjlyytonw.html

[S52] C++：const 与 noexcept
来源：http://hz.guowangkeji.top/gtlyukopjo.html

int size() const noexcept { return n_; }
来源：http://hz.ehwqpu.com/gttytlkedr.html

[S53] C++：移动语义
来源：http://hz.cqqwz.cn/gtrajrxlsq.html

std::vector<int> w = std::move(v);
来源：http://hz.316326.xyz/gtsrjexenv.html

[S54] C++：异常处理
来源：http://hz.hywenlv.cn/gthdozvoxa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.dashuyun.cn/gtfumpocdo.html

[S55] C++：结构化绑定
来源：http://hz.zycfv.cn/gtcdtsfvpj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shuidangran.top/gtrvegktbr.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gthxbffmik.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gtgilqzkxu.html

[S57] C++：编译期常量
来源：http://hz.ppjwa.cn/gttgmcpgxq.html

constexpr int N = 10;
来源：http://hz.shanyushiyangkeji.top/gtekfmdifm.html

[S58] C++：命名空间
来源：http://hz.jianghu66.top/gtnssbxjvn.html

namespace ns { int f() { return 1; } }
来源：http://hz.hfpthk.cn/gtxozhddzv.html

[S59] C++：静态断言
来源：http://hz.snrcjt.cn/gtfsfneqln.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenjidiqi.icu/gtbmhnctjc.html

[S60] C++：遍历并删除元素
来源：http://hz.gzhubu.top/gtoqbrnyuf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhixingplan.top/gtffnszqac.html

================================================================================
来源：http://hz.nwbrower.top/gthlonabdh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aibaodan.cn/gtjbazgige.html

================================================================================
来源：http://hz.52xcode.cn/gtffigzdpk.html

[T01] Kotlin：Hello World
来源：http://hz.gzhubu.top/gtdbahzpkl.html

println("Hello")
来源：http://hz.nanxinkj.top/gttlqpgvne.html

[T02] Kotlin：变量
来源：http://hz.hnxiangtu.top/gttfvxafjc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fengsongda.top/gtinaboiyr.html

[T03] Kotlin：字符串模板
来源：http://hz.kuanghao11.cn/gtdpxkxgiz.html

"值: $b"
来源：http://hz.sysykeji.top/gtwvyezwpe.html

[T04] Kotlin：空安全
来源：http://hz.pengpengdd.cyou/gtcanvcmqx.html

val n: String? = null;  n?.length
来源：http://hz.pengpengdd.cyou/gtcinodbeq.html

[T05] Kotlin：when 表达式
来源：http://hz.daria6918.cn/gtjfhnzygp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigufen.top/gtjqsuwhrl.html

[T06] Kotlin：集合映射
来源：http://hz.mhx1999.top/gtxtiiqfzy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangshuangyany.cn/gtmeimxwec.html

[T07] Kotlin：集合过滤
来源：http://hz.birdmap.top/gtlvbcxgkp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.9152youxi.cn/gttiwyqopl.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtjtjlyvck.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgfzy.top/gtvlvjmmqi.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigfzy.top/gtagotretl.html

fun String.exclaim() = this + "!"
来源：http://hz.ivvv.top/gtqqvactlb.html

[T10] Kotlin：默认参数
来源：http://hz.52xcode.cn/gtwajwjbys.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daxiang520.top/gtuobzdgow.html

[T11] Kotlin：协程
来源：http://hz.yj20258.top/gtmprdcscs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxuanxn.top/gtpkshqxhv.html

[T12] Kotlin：解构声明
来源：http://hz.birdmap.top/gtgzppirks.html

val (a, b) = Pair(1, 2)
来源：http://hz.cheryme.top/gtbnqrrufs.html

[T13] Kotlin：只读 Map
来源：http://hz.mhx1999.top/gtuapzusnh.html

val m = mapOf("a" to 1)
来源：http://hz.daria6918.cn/gtojaqmybr.html

[T14] Kotlin：循环
来源：http://hz.fzhhl.top/gtunhpbbco.html

for (i in 1..10) println(i)
来源：http://hz.andypj.xyz/gtpfheiehf.html

[T15] Kotlin：接口
来源：http://hz.bjfxy.top/gthmcptxgu.html

interface Shape { fun area(): Double }
来源：http://hz.hongshengwenyu.top/gtobbwtlis.html

[T16] Swift：Hello World
来源：http://hz.ydzc1.top/gtxhlydcmr.html

print("Hello")
来源：http://hz.jinqigufen.top/gtpvwgnmxl.html

[T17] Swift：变量与常量
来源：http://hz.daria6918.cn/gtqdkqgajq.html

var a = 1;  let b = 2
来源：http://hz.dashuyun.cn/gtngsuskqv.html

[T18] Swift：字符串插值
来源：http://hz.aibaodan.cn/gtxrndcuqs.html

"值: \(b)"
来源：http://hz.316326.xyz/gtdqgqwccz.html

[T19] Swift：可选绑定
来源：http://hz.hongshengwenyu.top/gtscopvbwy.html

if let n = opt { print(n) }
来源：http://hz.redwolf501.top/gtobrjrrnt.html

[T20] Swift：数组操作
来源：http://hz.0kj1m.cn/gtmbmtexfa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gteasqxwsj.html

[T21] Swift：遍历
来源：http://hz.bjfxy.top/gtzlqrbpyu.html

for x in a { print(x) }
来源：http://hz.pengpengdd.cyou/gtjinnnjcs.html

[T22] Swift：字典
来源：http://hz.kuanghao11.cn/gtlufhkuxw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.vqdsnc.cn/gtrjeoatsb.html

[T23] Swift：函数
来源：http://hz.hfpthk.cn/gtyqglxkgd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigufen.top/gtliuskfaq.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangkeji.top/gtglcgbxfr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigufen.top/gtzqbkxcug.html

[T25] Swift：结构体
来源：http://hz.pycfn.com/gtvedsueor.html

struct P { var x: Int }
来源：http://hz.guowangkeji.top/gtsanjoqda.html

[T26] Swift：类与重写
来源：http://hz.yj20258888.top/gtzxaclzxx.html

class A: Base { override func f() {} }
来源：http://hz.pengpengdd.cyou/gtohhmcysx.html

[T27] Swift：错误处理
来源：http://hz.yonumen.top/gtccdvmtrj.html

do { try f() } catch { print(error) }
来源：http://hz.yangfankeji.com/gtzevwgwrv.html

[T28] Swift：枚举
来源：http://hz.iojbl.cn/gtirjytyso.html

enum Color { case red, green }
来源：http://hz.jiagoushi.top/gtjustsqbq.html

[T29] Swift：guard 提前返回
来源：http://hz.sweek.top/gtexuoldly.html

guard let x = opt else { return }
来源：http://hz.meibo888.top/gtrqrbiecu.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gtbcsdkhcv.html

protocol Shape { func area() -> Double }
来源：http://hz.gzhubu.top/gtnikmesbo.html

[T31] Lua：Hello World
来源：http://hz.nwbrower.top/gtkvkdkdmt.html

print("Hello")
来源：http://hz.chenjidiqi.icu/gtblcnfhwk.html

[T32] Lua：局部变量
来源：http://hz.0kj1m.cn/gtbtdwscab.html

local a = 1
来源：http://hz.yj20258.top/gtoexeeswb.html

[T33] Lua：表（数组）
来源：http://hz.zdqjudy.top/gtvtnrxhzq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.havefunace.top/gtknpekixd.html

[T34] Lua：遍历表
来源：http://hz.ybcxt.top/gtznrvhbnx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jyoumei.cn/gtlycangvg.html

[T35] Lua：字典表
来源：http://hz.zdqjudy.top/gtigrqdqnq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cqqwz.cn/gtzkugshyz.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gtuxnlruzx.html

function add(a, b) return a + b end
来源：http://hz.jiagoushi.top/gtfekghzpl.html

[T37] Lua：字符串拼接
来源：http://hz.sweek.top/gtvjuelkaj.html

"a" .. "b"
来源：http://hz.yonumen.top/gtolxdsidw.html

[T38] Lua：条件
来源：http://hz.dianchejie.cn/gtmdlqybhs.html

if x > 0 then print("正") end
来源：http://hz.redwolf501.top/gtufpftqik.html

[T39] Lua：模式匹配
来源：http://hz.0kj1m.cn/gtcvkyqmru.html

string.find(s, "%d+")
来源：http://hz.jyoumei.cn/gtrbqbakvq.html

[T40] Lua：元表
来源：http://hz.yuanzhike.top/gtwetzregc.html

setmetatable({}, { __index = base })
来源：http://hz.feifeiyinyue.top/gtwmnpgqhf.html

[T41] Perl：Hello World
来源：http://hz.tianlin.xyz/gthwhaxvms.html

print "Hello\n";
来源：http://hz.svipenyu.cn/gtddnqqvei.html

[T42] Perl：变量类型
来源：http://hz.gogol.net.cn/gtlwrlrdqm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cdnleiting.top/gtfwuyknwn.html

[T43] Perl：字符串插值
来源：http://hz.fzhhl.top/gtqchlnmow.html

"值: $a"
来源：http://hz.jiagoushi.top/gtpmnkjhzm.html

[T44] Perl：条件
来源：http://hz.nanxuanxn.top/gtxcydttry.html

if ($a > 0) { print "正"; }
来源：http://hz.cashguo.top/gtaxjjxtug.html

[T45] Perl：数组遍历
来源：http://hz.hongshengwenyu.top/gtimcgjgar.html

for my $x (@arr) { print $x; }
来源：http://hz.nanxinkj.top/gtdyzfjuww.html

[T46] Perl：哈希操作
来源：http://hz.birdmap.top/gtoysqtgsb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.guannengcc.top/gtephepelr.html

[T47] Perl：正则捕获
来源：http://hz.shzxlz.cn/gtukzsxqbn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cheryme.top/gtqkissrml.html

[T48] Perl：正则替换
来源：http://hz.yvedp.cn/gtyojzfcbt.html

$s =~ s/old/new/g;
来源：http://hz.pycfn.com/gtclmrwfuy.html

[T49] Perl：函数
来源：http://hz.ywan-chungtsiang.top/gtukqjxkgw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ppjwa.cn/gtjsizruhv.html

[T50] Perl：逐行读文件
来源：http://hz.yangfankeji.com/gteumsshpk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gotoacloud.top/gtkslnzwkr.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.bjfxy.top/gtntynbiyw.html

[T51] Scala：Hello World
来源：http://hz.jyoumei.cn/gtwwjhefhk.html

println("Hello")
来源：http://hz.jianghu66.top/gtdxddpzww.html

[T52] Scala：变量
来源：http://hz.nanxinkj.top/gtjssorwjo.html


<!-- 参考信息 -->