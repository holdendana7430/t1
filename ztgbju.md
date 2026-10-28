代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tianlin.xyz/gtvfustrml.html

[R50] awk 求和
来源：http://hz.zhijiandao.cn/gtshdegacf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtfuciuipi.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtxwumwter.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yonumen.top/gtuvhqgwby.html

[R52] 统计行数
来源：http://hz.zycfv.cn/gtdslanuxv.html

wc -l a.txt
来源：http://hz.yj202588.top/gtehveqlhu.html

[R53] 查看文件头与实时尾
来源：http://hz.dashuyun.cn/gthnaiqdlh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.kuanghao11.cn/gtnmksvyvb.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtxxebaelz.html

diff a.txt b.txt
来源：http://hz.jqgfzy.top/gtfumvmjyr.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gtwhgolfrj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhaomingkeji.xyz/gtbtweyyjm.html

[R56] 远程拷贝
来源：http://hz.jyoumei.cn/gtkfpffxop.html

scp file user@host:/path/
来源：http://hz.xziqi.cn/gtjntnepmc.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtftxvunth.html

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtencbnkja.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtakwuhrha.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shuidangran.top/gthegepfmz.html

[R59] 发 POST JSON
来源：http://hz.ybcxt.top/gtzzrtjqpo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhijiandao.cn/gtkwzchwdx.html

[R60] 只看 HTTP 状态码
来源：http://hz.daxiang520.top/gttpqxgtnr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.snrcjt.cn/gtcyfjkcan.html

[R61] 磁盘占用
来源：http://hz.xingfuxueyuan.xyz/gttwantzzb.html

df -h;  du -sh *
来源：http://hz.pengpengdd.cyou/gtthdfiyni.html

[R62] 找最占空间的文件
来源：http://hz.jqgfzy.top/gtmdrxhayn.html

du -ah . | sort -rh | head -10
来源：http://hz.yvedp.cn/gtnjwfitgu.html

[R63] 内存与进程
来源：http://hz.jinghuilouyu.cn/gteuvsquiz.html

free -h;  ps aux | grep nginx
来源：http://hz.snrcjt.cn/gtgeiexrve.html

[R64] 结束进程
来源：http://hz.yj20258888.top/gtqxtxqdcu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.havefunace.top/gtcfuyramz.html

[R65] 查看端口占用
来源：http://hz.fengsongda.top/gtshkiddjo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangtech.top/gttziwfoqk.html

[R66] 定时任务
来源：http://hz.ehwqpu.com/gtjdygzqol.html

crontab -e;  crontab -l
来源：http://hz.aizwys.cn/gtbmlzgzde.html

[R67] 生成随机十六进制串
来源：http://hz.xylfe.cn/gtohikjxsw.html

openssl rand -hex 16
来源：http://hz.bjfxy.top/gtaggpykie.html

[R68] 计算文件校验值
来源：http://hz.nwbrower.top/gtnkrjpiwd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtexahfzhd.html

[R69] 生成随机密码
来源：http://hz.c1oappe.top/gtzyqavhqt.html

head -c 16 /dev/urandom | base64
来源：http://hz.sysykeji.top/gtxahqrpvx.html

[R70] 时间戳与互转
来源：http://hz.shzxlz.cn/gtujsxcoqy.html

date +%s;  date -d @1700000000
来源：http://hz.jinyuanbaomall.cn/gtdigbngbn.html

[R71] 日期格式化
来源：http://hz.birdmap.top/gtyrsrzpxc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.andypj.xyz/gtnabycqyg.html

[R72] 等待端口就绪
来源：http://hz.sufxvd.cn/gtycgvqgqc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj202588.top/gthzofohto.html

[R73] 分割大日志
来源：http://hz.sufxvd.cn/gtioupdxnb.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gtsqsnicpl.html

[R74] 批量重命名
来源：http://hz.gotoacloud.top/gtxlbvkxta.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gthdfqknat.html

[R75] 导出环境变量
来源：http://hz.gaohongyu789.top/gtjdyprnil.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.mhx1999.top/gtatrsrkrc.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtbvnkrhyx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtaitrylwz.html

[R77] 读取用户输入
来源：http://hz.daxiang520.top/gtebjffycu.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gtsnvaqcba.html

[R78] 交互式菜单
来源：http://hz.shangyingyoupin.top/gtarnatvzx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.quarkkingdee.top/gtrexadcfw.html

[R79] 解析命令行选项
来源：http://hz.nwbrower.top/gtfhzrjhup.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtlgtauuqk.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtpxpcwran.html

time ./run.sh
来源：http://hz.jiagoushi.top/gtiaiithmm.html

================================================================================
来源：http://hz.quarkkingdee.top/gtiptcelyo.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtjncjoaos.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtjtpzuchy.html

[S01] C：Hello World
来源：http://hz.cashguo.top/gtmxktxdeq.html

#include <stdio.h>
来源：http://hz.jlsjyb.cn/gtsnrkklqo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.redwolf501.top/gtskalavdy.html

[S02] C：变量与格式化输出
来源：http://hz.fengsongda.top/gtfigusfqn.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnxiangtu.top/gtaqynhqwx.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtjnyhjqlr.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtoylsgjky.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtpqewjeor.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hongshengwenyu.top/gtovywavuu.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtsomgjclh.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtyzyibrlj.html

[S06] C：字符串比较
来源：http://hz.fengsongda.top/gtfynfwyzy.html

strcmp(a, b) == 0
来源：http://hz.xylfe.cn/gtwdiisfmt.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtqfiyzhqf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xingfuxueyuan.xyz/gthrdmlfxk.html

[S08] C：动态内存分配与释放
来源：http://hz.chenlongwang.top/gtxvccrngk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.vqdsnc.cn/gtfvqzvtwm.html

[S09] C：结构体定义与初始化
来源：http://hz.cqqwz.cn/gtjwmloqag.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sysykeji.top/gtmaurjstl.html

[S10] C：指针与解引用
来源：http://hz.yj20258888.top/gtkgbzzyxe.html

int *p = &a;  *p = 5;
来源：http://hz.cashguo.top/gtdjjpjreu.html

[S11] C：逐行读文件
来源：http://hz.xuanzx.com/gtthmyyhmi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtyrcwktrs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gaohongyu789.top/gtxkufzwtr.html

fclose(f);
来源：http://hz.shuidangran.top/gtwtlxzcap.html

[S12] C：写文件
来源：http://hz.wangshuangyany.cn/gtvwcyclpy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.quarkkingdee.top/gtkuhgjttt.html

[S13] C：宏定义
来源：http://hz.tanke756.top/gtfqbsfdiw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.aizwys.cn/gtcgxqlmdz.html

[S14] C：枚举
来源：http://hz.aibaodan.cn/gtnzhubrdi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtlxjvzjne.html

[S15] C：类型转换
来源：http://hz.yj202588.top/gtmjrrzxuj.html

(double) a / b
来源：http://hz.zhixingplan.top/gtsdlypgrs.html

[S16] C：位操作置位
来源：http://hz.cheryme.top/gtzjturjxq.html

x |= (1 << 3);
来源：http://hz.jlsjyb.cn/gtmmjfzxeh.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtdncmafcn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxuanxn.top/gtjtupttro.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtclqbpwzw.html

int main(int argc, char **argv)
来源：http://hz.ydjk.org.cn/gtfdtgxoqk.html

[S19] C：快速排序
来源：http://hz.yuxming.cn/gtvfeqweel.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtzwdqrclo.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtsscapvdl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtmwrjikhc.html

[S21] C：字符类别判断
来源：http://hz.mhx1999.top/gtripccgpc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shanyushiyangtech.top/gtyewycjxu.html

[S22] C：字符串转数字
来源：http://hz.jlsjyb.cn/gtubzbzqvn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fzhhl.top/gtpbdoarbf.html

[S23] C：随机数
来源：http://hz.gotoacloud.top/gtplslegxy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nanxuanxn.top/gtilnaxzvr.html

[S24] C：获取本地时间
来源：http://hz.hysaishi.cn/gtijxcaqjz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangshuangyany.cn/gtgoildunq.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtpoxxucgf.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtvlewsqcn.html

[S26] C：内存清零
来源：http://hz.daria6918.cn/gtymokbcdn.html

memset(a, 0, sizeof a);
来源：http://hz.hnqzz.top/gttqbjidxk.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtqgerwrbt.html

const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtpzzkwjxt.html

[S28] C：静态变量
来源：http://hz.vqdsnc.cn/gtytswkqgz.html

static int counter = 0;
来源：http://hz.yj202588.top/gtwxulyffo.html

[S29] C：变参函数
来源：http://hz.tian-w.cn/gteipboikg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangshuangyany.cn/gtabjuyuap.html

[S30] C：头文件保护
来源：http://hz.cashguo.top/gtyratyczl.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gtnxebgsft.html

#define X_H
来源：http://hz.jinqigfzy.top/gttwnubxcl.html

#endif
来源：http://hz.zhiwuduotai.top/gtiitfphpc.html

[S31] C++：Hello World
来源：http://hz.hfpthk.cn/gtpyfljmyv.html

#include <iostream>
来源：http://hz.jqgfzy.top/gtwknmdowa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtkkjbksqc.html

[S32] C++：字符串
来源：http://hz.ydzc1.top/gtxggbwbpo.html

std::string s = "hi";  s += "!";
来源：http://hz.zhixingplan.top/gtdrotfnhn.html

[S33] C++：vector 增删
来源：http://hz.yongpay.top/gthjwxraju.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tanke756.top/gtdidodmrg.html

[S34] C++：遍历 vector
来源：http://hz.quarkkingdee.top/gtgzybqxdq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guannengcc.top/gtbfaqeudi.html

[S35] C++：map
来源：http://hz.zhijiandao.cn/gtwmjfwcro.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtmlvzzhcv.html

[S36] C++：unordered_map
来源：http://hz.pengpengdd.cyou/gtndxkurbs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gttiadxfgc.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gtjugltlhs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.dianchejie.cn/gtchrkorxq.html

[S38] C++：排序
来源：http://hz.316326.xyz/gtcvhhsbnq.html

std::sort(v.begin(), v.end());
来源：http://hz.bjfxy.top/gtbwbebfaa.html

[S39] C++：自定义比较器排序
来源：http://hz.smart0.xyz/gthvnussrs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtfssduvxz.html

[S40] C++：查找元素
来源：http://hz.quarkkingdee.top/gtotjigktr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.316326.xyz/gtnsduiyad.html

[S41] C++：类与构造函数
来源：http://hz.yongpay.top/gtpyxulfxm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtkznxuplq.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gtzuxsxzbb.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gthogojsvc.html

[S43] C++：智能指针
来源：http://hz.nanxinkj.top/gtttihvikk.html

auto p = std::make_unique<int>(5);
来源：http://hz.jianghu66.top/gtpdkgrlyd.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangkeji.top/gtndosteze.html

void inc(int &x) { ++x; }
来源：http://hz.yonumen.top/gtaruufmlf.html

[S45] C++：lambda
来源：http://hz.yanxiufei.cn/gtwveokbwb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhaomingkeji.xyz/gtiqkcafwk.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gtuxbktvsg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtegohxvjr.html

[S47] C++：结构化绑定遍历
来源：http://hz.nanxuanxn.top/gtwajbelei.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gtsohchupn.html

[S48] C++：逐行读文件
来源：http://hz.shzxlz.cn/gtsvwvmkob.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.52xcode.cn/gtjpvgeaxp.html

while (std::getline(in, line)) { }
来源：http://hz.quarkkingdee.top/gtrpgdiajp.html

[S49] C++：写文件
来源：http://hz.ivvv.top/gtbodmhqob.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xinyue.icu/gtsprefovt.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtghsvgymo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ehwqpu.com/gteapssvcd.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangtech.top/gtwjgndtms.html

static_cast<double>(a) / b
来源：http://hz.chenlongwang.top/gtelfyzree.html

[S52] C++：const 与 noexcept
来源：http://hz.wangdashe.top/gtckpwjcbq.html

int size() const noexcept { return n_; }
来源：http://hz.52xcode.cn/gtmixfmqxj.html

[S53] C++：移动语义
来源：http://hz.hnxiangtu.top/gtkowmrdcl.html

std::vector<int> w = std::move(v);
来源：http://hz.hfpthk.cn/gtuilscaea.html

[S54] C++：异常处理
来源：http://hz.ehwqpu.com/gtofbmflid.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shuidangran.top/gtupglmrvy.html

[S55] C++：结构化绑定
来源：http://hz.c1oappe.top/gtxnmcfbyo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aizwys.cn/gtxfdxpzqu.html

[S56] C++：optional
来源：http://hz.birdmap.top/gteyabubkn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ppjwa.cn/gtwfqdajnm.html

[S57] C++：编译期常量
来源：http://hz.cashguo.top/gtpyzknezt.html

constexpr int N = 10;
来源：http://hz.jinghuilouyu.cn/gtoebqmxeb.html

[S58] C++：命名空间
来源：http://hz.9152youxi.cn/gtmkzlllwg.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuanzhike.top/gtsrbrrvsg.html

[S59] C++：静态断言
来源：http://hz.cqqwz.cn/gtlrqnsdor.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ehwqpu.com/gtyzgkkukd.html

[S60] C++：遍历并删除元素
来源：http://hz.svipenyu.cn/gtvafgnyvt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gtnlywynlw.html

================================================================================
来源：http://hz.bjfxy.top/gtnnoblzaq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtdklcjmhu.html

================================================================================
来源：http://hz.shangyingyoupin.top/gttqeqswun.html

[T01] Kotlin：Hello World
来源：http://hz.xinyue.icu/gtmcdakczh.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtqscdnazg.html

[T02] Kotlin：变量
来源：http://hz.ehwqpu.com/gtofapnggn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuetiantiany.cn/gtpbtzkeex.html

[T03] Kotlin：字符串模板
来源：http://hz.nwbrower.top/gtmsosnsxg.html

"值: $b"
来源：http://hz.9152youxi.cn/gtinvhtoez.html

[T04] Kotlin：空安全
来源：http://hz.sufxvd.cn/gtxclsdvqn.html

val n: String? = null;  n?.length
来源：http://hz.sufxvd.cn/gtrxvmgatp.html

[T05] Kotlin：when 表达式
来源：http://hz.sxryk.cn/gtaklcuavo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhengqikj.top/gtqjlhfsmm.html

[T06] Kotlin：集合映射
来源：http://hz.andypj.xyz/gtrskpuppx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gtldijkcgy.html

[T07] Kotlin：集合过滤
来源：http://hz.sysykeji.top/gtymxhcvtj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.daxiang520.top/gtveipoitz.html

[T08] Kotlin：数据类
来源：http://hz.mhx1999.top/gtlexmmvcn.html

data class User(val name: String, val age: Int)
来源：http://hz.sweek.top/gtyditqzyx.html

[T09] Kotlin：扩展函数
来源：http://hz.chenlongwang.top/gtdmfmkknu.html

fun String.exclaim() = this + "!"
来源：http://hz.ydzc1.top/gtkbdejlro.html

[T10] Kotlin：默认参数
来源：http://hz.ydzc1.top/gtyzukffsb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.meibo888.top/gtwnccszgm.html

[T11] Kotlin：协程
来源：http://hz.yj202588.top/gtaeminmym.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pengpengdd.cyou/gtihngezcx.html

[T12] Kotlin：解构声明
来源：http://hz.jinghuilouyu.cn/gtopfvhudq.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gttbrwoasn.html

[T13] Kotlin：只读 Map
来源：http://hz.9152youxi.cn/gtphnxadpv.html

val m = mapOf("a" to 1)
来源：http://hz.ehwqpu.com/gtzurglrgh.html

[T14] Kotlin：循环
来源：http://hz.yj202588.top/gtbqeyseco.html

for (i in 1..10) println(i)
来源：http://hz.jinghuilouyu.cn/gthgnadsbl.html

[T15] Kotlin：接口
来源：http://hz.yueranfly.top/gtcnsxrhar.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtcyyoxlzc.html

[T16] Swift：Hello World
来源：http://hz.jyoumei.cn/gtznabicff.html

print("Hello")
来源：http://hz.jqgfzy.top/gtlsvftybt.html

[T17] Swift：变量与常量
来源：http://hz.jqgfzy.top/gtipuoxwzy.html

var a = 1;  let b = 2
来源：http://hz.ivvv.top/gtpaotwnxx.html

[T18] Swift：字符串插值
来源：http://hz.fzhhl.top/gteoucwcfw.html

"值: \(b)"
来源：http://hz.chenzaomai.com/gtnseutgfc.html

[T19] Swift：可选绑定
来源：http://hz.xuetiantiany.cn/gtwficxgxo.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gtfpnieilb.html

[T20] Swift：数组操作
来源：http://hz.cdnleiting.top/gtqpfvfrsg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jlsjyb.cn/gtxwwzpyjg.html

[T21] Swift：遍历
来源：http://hz.kuanghao11.cn/gtugkcnptc.html

for x in a { print(x) }
来源：http://hz.zhoulong.xyz/gtdqqyoejk.html

[T22] Swift：字典
来源：http://hz.cdnleiting.top/gtyowxnndd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.haohaochexian.top/gtixlgwybz.html

[T23] Swift：函数
来源：http://hz.gogol.net.cn/gtncmtxsvb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xziqi.cn/gtcdaaejti.html

[T24] Swift：闭包
来源：http://hz.zhiwuduotai.top/gtnurfszej.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nwbrower.top/gtxqfmixax.html

[T25] Swift：结构体
来源：http://hz.yj20258888.top/gtwjciwtme.html

struct P { var x: Int }
来源：http://hz.jyoumei.cn/gtnxckhxye.html

[T26] Swift：类与重写
来源：http://hz.yongpay.top/gtutzctuqi.html

class A: Base { override func f() {} }
来源：http://hz.hywenlv.cn/gtqagmvbal.html

[T27] Swift：错误处理
来源：http://hz.yanxiufei.cn/gtcuwfmczk.html

do { try f() } catch { print(error) }
来源：http://hz.shangyingyoupin.top/gtnghcrlqi.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gthobbadui.html

enum Color { case red, green }
来源：http://hz.sweek.top/gtffcbkzgp.html

[T29] Swift：guard 提前返回
来源：http://hz.jianghu66.top/gtblftasnn.html

guard let x = opt else { return }
来源：http://hz.aizwys.cn/gtgdptdbws.html

[T30] Swift：协议
来源：http://hz.sxryk.cn/gtkugsosii.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gthoyxqbun.html

[T31] Lua：Hello World
来源：http://hz.ivvv.top/gtuamoguuy.html

print("Hello")
来源：http://hz.fzhhl.top/gtcninhtwi.html

[T32] Lua：局部变量
来源：http://hz.daxiang520.top/gtjyetpvyf.html

local a = 1
来源：http://hz.yonumen.top/gtewgxqiis.html

[T33] Lua：表（数组）
来源：http://hz.guowangkeji.top/gtuomricbm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.pycfn.com/gttfnibhxl.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gtwqsjqfsf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shzxlz.cn/gtulsyzkkn.html

[T35] Lua：字典表
来源：http://hz.meibo888.top/gtgiplxvbl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gogol.net.cn/gtbgksomwn.html

[T36] Lua：函数
来源：http://hz.aizwys.cn/gtbvpysnwo.html

function add(a, b) return a + b end
来源：http://hz.kuanghao11.cn/gtqoeqzfko.html

[T37] Lua：字符串拼接
来源：http://hz.aizwys.cn/gtlmaexkek.html

"a" .. "b"
来源：http://hz.zhongyouzk.top/gtlaugrdrn.html

[T38] Lua：条件
来源：http://hz.zhijiandao.cn/gtjofgdobt.html

if x > 0 then print("正") end
来源：http://hz.wangdashe.top/gtvwnfnbzq.html

[T39] Lua：模式匹配
来源：http://hz.pengpengdd.cyou/gtxdswgzaq.html

string.find(s, "%d+")
来源：http://hz.yangfankeji.com/gtnonognjm.html

[T40] Lua：元表
来源：http://hz.chenlongwang.top/gtkncqekud.html

setmetatable({}, { __index = base })
来源：http://hz.316326.xyz/gtfxschrdz.html

[T41] Perl：Hello World
来源：http://hz.shuidangran.top/gtemqngefc.html

print "Hello\n";
来源：http://hz.xuanzx.com/gteyxleeyp.html

[T42] Perl：变量类型
来源：http://hz.yanxiufei.cn/gtwbypfgyh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.52xcode.cn/gttwrhlzyu.html

[T43] Perl：字符串插值
来源：http://hz.hysaishi.cn/gtfurokdcp.html

"值: $a"
来源：http://hz.xinyue.icu/gtzwqjmfnr.html

[T44] Perl：条件
来源：http://hz.sweek.top/gttalovnqs.html

if ($a > 0) { print "正"; }
来源：http://hz.hammf.cn/gtjpnfvzfk.html

[T45] Perl：数组遍历
来源：http://hz.jqgfzy.top/gtznwgpjvy.html

for my $x (@arr) { print $x; }
来源：http://hz.jiagoushi.top/gtzcuzzdxi.html

[T46] Perl：哈希操作
来源：http://hz.yj20258888.top/gtcnttbpkg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.svipenyu.cn/gtlxngpgzf.html

[T47] Perl：正则捕获
来源：http://hz.jinghuilouyu.cn/gtepohpocr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hfpthk.cn/gtrdndswun.html

[T48] Perl：正则替换
来源：http://hz.tianlin.xyz/gtzhxxekjz.html

$s =~ s/old/new/g;
来源：http://hz.cqqwz.cn/gtdlrmbpgg.html

[T49] Perl：函数
来源：http://hz.yvedp.cn/gtxrtqlqpt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yuxming.cn/gtxcdqasqg.html

[T50] Perl：逐行读文件
来源：http://hz.xuetiantiany.cn/gtoeuuixex.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhengqikj.top/gtxsrzvjor.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tianlin.xyz/gtyqgbnhuw.html

[T51] Scala：Hello World
来源：http://hz.chenlongwang.top/gtroysepfv.html

println("Hello")
来源：http://hz.gzhubu.top/gtzpitinnx.html

[T52] Scala：变量
来源：http://hz.cashguo.top/gtytbosgvz.html


<!-- 参考信息 -->