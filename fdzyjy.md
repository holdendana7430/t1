代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ppjwa.cn/gtivhegcan.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gtpibhuvqu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gzhubu.top/gtfttgvhla.html

[R37] 把输出赋给变量
来源：http://hz.meibo888.top/gtmrwzqjue.html

files=$(ls -1)
来源：http://hz.9152youxi.cn/gtqpntcywe.html

[R38] 管道串联
来源：http://hz.jinyuanbaomall.cn/gtfqmezlfz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tanke756.top/gtkxraigov.html

[R39] 重定向标准输出与错误
来源：http://hz.zhijiandao.cn/gthxepnqoz.html

cmd > out.log 2>&1
来源：http://hz.vqdsnc.cn/gtejwiyoml.html

[R40] 追加写日志
来源：http://hz.bjfxy.top/gtkhtsoisf.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gtaosrpobx.html

[R41] 丢弃输出
来源：http://hz.zhixingplan.top/gtqigeqaln.html

cmd >/dev/null 2>&1
来源：http://hz.jinyuanbaomall.cn/gtsjbeipuh.html

[R42] 输入重定向
来源：http://hz.chenjidiqi.icu/gtufjuwrtm.html

wc -l < a.txt
来源：http://hz.hywenlv.cn/gtykmwtkqs.html

[R43] 按名字查找文件
来源：http://hz.ehwqpu.com/gtumremqyz.html

find . -name "*.log" -type f
来源：http://hz.hysaishi.cn/gtrxasjyqb.html

[R44] 按修改时间查找
来源：http://hz.jinqigfzy.top/gtlnjdmiam.html

find . -mtime -7 -type f
来源：http://hz.zhengqikj.top/gtjjjgjcfe.html

[R45] 批量删除
来源：http://hz.shanyushiyangkeji.top/gtydfefpwn.html

find . -name "*.tmp" -delete
来源：http://hz.yuanzhike.top/gtxujkzcnl.html

[R46] 递归替换文件内容
来源：http://hz.yanxiufei.cn/gtmcjykypt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hfpthk.cn/gtrvswazue.html

[R47] sed 单行替换
来源：http://hz.ivvv.top/gtmpkgbibu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydzc1.top/gtfgcfzivh.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gtvdalnvan.html

awk '{print $1, $3}' a.txt
来源：http://hz.tianlin.xyz/gtotccttal.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtfuvulsiv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.svipenyu.cn/gtkzaeatlj.html

[R50] awk 求和
来源：http://hz.bjfxy.top/gtlmmkonni.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.feifeiyinyue.top/gttnovrolx.html

[R51] 排序去重取前几
来源：http://hz.gaohongyu789.top/gtdoyiynam.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ivvv.top/gtfhxknwbc.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtynktvpbw.html

wc -l a.txt
来源：http://hz.hnqzz.top/gtvuilwbrd.html

[R53] 查看文件头与实时尾
来源：http://hz.tanke756.top/gtrbwspjyc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydzc1.top/gtpsnlisgq.html

[R54] 比较两个文件
来源：http://hz.nanxinkj.top/gtdqozrzgb.html

diff a.txt b.txt
来源：http://hz.guowangkeji.top/gtnnuotvtd.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gtnqiuebkf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuxming.cn/gtxuxmcnge.html

[R56] 远程拷贝
来源：http://hz.ppjwa.cn/gttusfqsxr.html

scp file user@host:/path/
来源：http://hz.fengsongda.top/gtlnvcgssh.html

[R57] 远程执行命令
来源：http://hz.zhiwuduotai.top/gtjesjqtxw.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gtrhaqnitw.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gtbxprquxg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.feifeiyinyue.top/gtheljqiad.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gtmdkiaoze.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gtnkrdcjqp.html

[R60] 只看 HTTP 状态码
来源：http://hz.yonumen.top/gtlulxpraw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hnqzz.top/gtsxwcgoat.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtgnitkxuk.html

df -h;  du -sh *
来源：http://hz.chenlongwang.top/gtziudyoeo.html

[R62] 找最占空间的文件
来源：http://hz.zhengqikj.top/gtcihechuq.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtojdwvmzb.html

[R63] 内存与进程
来源：http://hz.zhixingplan.top/gtpoghuyhx.html

free -h;  ps aux | grep nginx
来源：http://hz.tanke756.top/gtejtbnurq.html

[R64] 结束进程
来源：http://hz.dashuyun.cn/gthztladtw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtzgnbavku.html

[R65] 查看端口占用
来源：http://hz.shzxlz.cn/gthihurkzr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jianghu66.top/gtyvqplgbp.html

[R66] 定时任务
来源：http://hz.haohaochexian.top/gtqvmwmest.html

crontab -e;  crontab -l
来源：http://hz.bjfxy.top/gtgwjosjde.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gtasyhawhw.html

openssl rand -hex 16
来源：http://hz.zhixingplan.top/gtrmuxxnfi.html

[R68] 计算文件校验值
来源：http://hz.hammf.cn/gttpvyvdry.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hfpthk.cn/gttrbkxxer.html

[R69] 生成随机密码
来源：http://hz.hammf.cn/gtxmenminc.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gtuefywgpl.html

[R70] 时间戳与互转
来源：http://hz.sufxvd.cn/gthjjswmcm.html

date +%s;  date -d @1700000000
来源：http://hz.zhoulong.xyz/gtxrsqxlaw.html

[R71] 日期格式化
来源：http://hz.zhongyouzk.top/gtcszjlrct.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydjk.org.cn/gtknzxkwue.html

[R72] 等待端口就绪
来源：http://hz.52xcode.cn/gtolxrvjua.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgufenzy.top/gthzqcutoe.html

[R73] 分割大日志
来源：http://hz.feifeiyinyue.top/gtfvteopdv.html

split -l 1000 big.log part_
来源：http://hz.tian-w.cn/gtpucatuwk.html

[R74] 批量重命名
来源：http://hz.nanxuanxn.top/gtxbcypwat.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xinyue.icu/gtlqgmrptr.html

[R75] 导出环境变量
来源：http://hz.ydjk.org.cn/gtnecxfpwa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydjk.org.cn/gtbfkibqpo.html

[R76] 使用临时文件
来源：http://hz.tanke756.top/gtgursifmc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gtwjgfdtlg.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtmjitmsom.html

read -rp "请输入: " ans
来源：http://hz.xingfuxueyuan.xyz/gtkkdihwpm.html

[R78] 交互式菜单
来源：http://hz.jinqigfzy.top/gtczothluv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.9152youxi.cn/gtlljffukh.html

[R79] 解析命令行选项
来源：http://hz.andypj.xyz/gtzpjokona.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shuidangran.top/gtxjityero.html

[R80] 查看脚本执行耗时
来源：http://hz.dianchejie.cn/gtuenkrzgi.html

time ./run.sh
来源：http://hz.yueranfly.top/gtfbovhckf.html

================================================================================
来源：http://hz.daxiang520.top/gtxolsrhmn.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtesemiqwn.html

================================================================================
来源：http://hz.birdmap.top/gtrfqbibqz.html

[S01] C：Hello World
来源：http://hz.c1oappe.top/gtdwtokvan.html

#include <stdio.h>
来源：http://hz.cqqwz.cn/gtdgjkendx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yangfankeji.com/gtnnhfqijv.html

[S02] C：变量与格式化输出
来源：http://hz.cashguo.top/gtdimsqmmj.html

int a = 10; printf("%d\n", a);
来源：http://hz.sufxvd.cn/gtnrfbwnwv.html

[S03] C：读入整数
来源：http://hz.52xcode.cn/gtqycbtghu.html

int x; scanf("%d", &x);
来源：http://hz.9152youxi.cn/gtudeeuhhm.html

[S04] C：字符串复制
来源：http://hz.mhx1999.top/gtnrjhqhod.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.vqdsnc.cn/gtzaqxkjej.html

[S05] C：字符串长度
来源：http://hz.wangdashe.top/gtkzpuevyu.html

strlen(s)
来源：http://hz.tian-w.cn/gthyavjeyz.html

[S06] C：字符串比较
来源：http://hz.zdqjudy.top/gtmlpahixl.html

strcmp(a, b) == 0
来源：http://hz.quarkkingdee.top/gthhdhgvhv.html

[S07] C：数组遍历求和
来源：http://hz.xingfuxueyuan.xyz/gtndndjlcj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxinkj.top/gtvupyrgko.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangkeji.top/gtkfzwirur.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangshuangyany.cn/gtfjrpqezv.html

[S09] C：结构体定义与初始化
来源：http://hz.gotoacloud.top/gtetgfnkjr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hywenlv.cn/gtvkwfsuel.html

[S10] C：指针与解引用
来源：http://hz.hnqzz.top/gtvgysobcp.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtrlkleozm.html

[S11] C：逐行读文件
来源：http://hz.c1oappe.top/gtrtxhcpaf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.svipenyu.cn/gttbdkmgfo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydjk.org.cn/gtdzquiosg.html

fclose(f);
来源：http://hz.meibo888.top/gtdqflnduq.html

[S12] C：写文件
来源：http://hz.zhongyouzk.top/gtizhvhflq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gtdikqndks.html

[S13] C：宏定义
来源：http://hz.tanke756.top/gtstdjiwhg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.snrcjt.cn/gtpitbhpjr.html

[S14] C：枚举
来源：http://hz.yonumen.top/gtryaifqxh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pengpengdd.cyou/gtkcubcmdd.html

[S15] C：类型转换
来源：http://hz.feifeiyinyue.top/gtqqysgylh.html

(double) a / b
来源：http://hz.hfpthk.cn/gtlqwetjrk.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtkxqddgme.html

x |= (1 << 3);
来源：http://hz.guowangkeji.top/gttfwhlvie.html

[S17] C：安全拼接字符串
来源：http://hz.ivvv.top/gtxsmgkpit.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gotoacloud.top/gtxssmzgzv.html

[S18] C：命令行参数
来源：http://hz.yangfankeji.com/gtrfsrlosu.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtnnuwufmh.html

[S19] C：快速排序
来源：http://hz.yj20258.top/gtamjqkqdf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtuqntxjhl.html

[S20] C：二分查找
来源：http://hz.cucudq.cn/gtujbcxcmg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtcfamkmdh.html

[S21] C：字符类别判断
来源：http://hz.zhaomingkeji.xyz/gtlslrkclw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtivpsmwkz.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtkdzcrnxg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.0kj1m.cn/gtzpcfezbu.html

[S23] C：随机数
来源：http://hz.yangfankeji.com/gtzsxvfoph.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtdnuzbkpb.html

[S24] C：获取本地时间
来源：http://hz.gotoacloud.top/gtvxezkvma.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shangyingyoupin.top/gtkcvusvxp.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangtech.top/gtglsttrhw.html

memcpy(dst, src, n);
来源：http://hz.vqdsnc.cn/gtxmoaxbej.html

[S26] C：内存清零
来源：http://hz.jinqigfzy.top/gtylsxtvim.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258.top/gtxaxsvmqx.html

[S27] C：定义常量
来源：http://hz.ivvv.top/gteiffqtpt.html

const double PI = 3.14159;
来源：http://hz.ivvv.top/gtxrjfyufp.html

[S28] C：静态变量
来源：http://hz.ivvv.top/gtzzzwkvrm.html

static int counter = 0;
来源：http://hz.ivvv.top/gtrauwwyup.html

[S29] C：变参函数
来源：http://hz.zhijiandao.cn/gtnvuwvdvh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtrgayxpxj.html

[S30] C：头文件保护
来源：http://hz.pycfn.com/gtutaljemq.html

#ifndef X_H
来源：http://hz.yj20258.top/gthqesuhcd.html

#define X_H
来源：http://hz.52xcode.cn/gtkshjrecw.html

#endif
来源：http://hz.smart0.xyz/gtkleplucg.html

[S31] C++：Hello World
来源：http://hz.yuanzhike.top/gtcwalvazx.html

#include <iostream>
来源：http://hz.yuanzhike.top/gteladjpkx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigfzy.top/gtqkaxkfcu.html

[S32] C++：字符串
来源：http://hz.jinqigfzy.top/gtiawehcdj.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtwasankwn.html

[S33] C++：vector 增删
来源：http://hz.yanxiufei.cn/gtfiiwcqqw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtrmazbrig.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gtpddyrezu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhixingplan.top/gtjzmsqfpc.html

[S35] C++：map
来源：http://hz.gogol.net.cn/gtwlswamwa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtdrnbzmwk.html

[S36] C++：unordered_map
来源：http://hz.sufxvd.cn/gtofypbloc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtktrvxtpw.html

[S37] C++：set
来源：http://hz.yj202588.top/gtmyjlpavx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cdnleiting.top/gteuvhpquc.html

[S38] C++：排序
来源：http://hz.ehwqpu.com/gtjuklyzvj.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtwocmkcni.html

[S39] C++：自定义比较器排序
来源：http://hz.hammf.cn/gtavmvxmon.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinyuanbaomall.cn/gteohacdvs.html

[S40] C++：查找元素
来源：http://hz.xingfuxueyuan.xyz/gtsqefizhm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuanzx.com/gtibaetlhb.html

[S41] C++：类与构造函数
来源：http://hz.haohaochexian.top/gthxqytcdr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.havefunace.top/gtxvatxzmc.html

[S42] C++：继承与虚函数
来源：http://hz.tanke756.top/gtahfumlfl.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtytxwjkhx.html

[S43] C++：智能指针
来源：http://hz.zdqjudy.top/gtaxaahlmz.html

auto p = std::make_unique<int>(5);
来源：http://hz.zdqjudy.top/gtuzgyrmjk.html

[S44] C++：引用传参
来源：http://hz.0kj1m.cn/gtezxlxdvu.html

void inc(int &x) { ++x; }
来源：http://hz.redwolf501.top/gtlzknhmka.html

[S45] C++：lambda
来源：http://hz.9152youxi.cn/gtsxbrzawm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jiagoushi.top/gtvatkwydq.html

[S46] C++：函数模板
来源：http://hz.birdmap.top/gtkiirrpuz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangkeji.top/gtrjgmtrfa.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gtrgmkpwjt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guannengcc.top/gtgeafrdoe.html

[S48] C++：逐行读文件
来源：http://hz.hammf.cn/gtbcmemrcq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hongshengwenyu.top/gtcrbxbxax.html

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gtqryttclb.html

[S49] C++：写文件
来源：http://hz.jinyuanbaomall.cn/gtqeohdmjr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gtfsmawrdy.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtbemqkcbc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ppjwa.cn/gtlcyksvdo.html

[S51] C++：显式类型转换
来源：http://hz.zhixingplan.top/gtfzyvkvbx.html

static_cast<double>(a) / b
来源：http://hz.fzhhl.top/gtwzqmlavz.html

[S52] C++：const 与 noexcept
来源：http://hz.yuxming.cn/gtmlydyift.html

int size() const noexcept { return n_; }
来源：http://hz.birdmap.top/gttahpssin.html

[S53] C++：移动语义
来源：http://hz.hongshengwenyu.top/gttoludgqd.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gtwxajcdnx.html

[S54] C++：异常处理
来源：http://hz.jqgufenzy.top/gtbxzjwroc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuanzhike.top/gtmhlzzoup.html

[S55] C++：结构化绑定
来源：http://hz.haohaochexian.top/gtidscqqtr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgufenzy.top/gtaarxvzwp.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gtsectroua.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hfpthk.cn/gtbgtugbzz.html

[S57] C++：编译期常量
来源：http://hz.gaohongyu789.top/gtpztpgdje.html

constexpr int N = 10;
来源：http://hz.gzhubu.top/gtywaxtfus.html

[S58] C++：命名空间
来源：http://hz.zhiwuduotai.top/gtkvwvcapd.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinyuanbaomall.cn/gtikwyplwr.html

[S59] C++：静态断言
来源：http://hz.havefunace.top/gtgytfasco.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jlsjyb.cn/gtyvzqivus.html

[S60] C++：遍历并删除元素
来源：http://hz.dianchejie.cn/gtugktxuuq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtaehyqacw.html

================================================================================
来源：http://hz.daria6918.cn/gtoyqoczbz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jlsjyb.cn/gtyrckrlen.html

================================================================================
来源：http://hz.hnxiangtu.top/gtkxaigeci.html

[T01] Kotlin：Hello World
来源：http://hz.yueranfly.top/gtqbeloqmx.html

println("Hello")
来源：http://hz.tian-w.cn/gtqpdaudvn.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gttiwtkopg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ehwqpu.com/gtvvqzektv.html

[T03] Kotlin：字符串模板
来源：http://hz.0kj1m.cn/gtyycolqja.html

"值: $b"
来源：http://hz.dashuyun.cn/gtqfbwddcj.html

[T04] Kotlin：空安全
来源：http://hz.hywenlv.cn/gtrmcyuzte.html

val n: String? = null;  n?.length
来源：http://hz.jinqigufen.top/gtkmnofafi.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgfzy.top/gtyqsivgmn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgufenzy.top/gtxxxwhnfc.html

[T06] Kotlin：集合映射
来源：http://hz.meibo888.top/gtbtxizyai.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pycfn.com/gtjmzztnmd.html

[T07] Kotlin：集合过滤
来源：http://hz.aizwys.cn/gteskezlho.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtdleqjmoq.html

[T08] Kotlin：数据类
来源：http://hz.aibaodan.cn/gtpxewapje.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtsvdwyzjc.html

[T09] Kotlin：扩展函数
来源：http://hz.jinyuanbaomall.cn/gtevqdvztx.html

fun String.exclaim() = this + "!"
来源：http://hz.gotoacloud.top/gthgzcfuno.html

[T10] Kotlin：默认参数
来源：http://hz.jlsjyb.cn/gtzwjtbptl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hammf.cn/gtayufszvc.html

[T11] Kotlin：协程
来源：http://hz.chenlongwang.top/gtgxldwlsr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gaohongyu789.top/gtqmiodhxx.html

[T12] Kotlin：解构声明
来源：http://hz.redwolf501.top/gtxdeplktw.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgufenzy.top/gtswklivhy.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtbeogvift.html

val m = mapOf("a" to 1)
来源：http://hz.smart0.xyz/gtilenmoha.html

[T14] Kotlin：循环
来源：http://hz.redwolf501.top/gtxtmlfkfs.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangtech.top/gtcdrkrkam.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtqwpwqxqr.html

interface Shape { fun area(): Double }
来源：http://hz.cheryme.top/gtdaaqwsbr.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtikjaojsu.html

print("Hello")
来源：http://hz.zycfv.cn/gtmdwqmrvz.html

[T17] Swift：变量与常量
来源：http://hz.zhixingplan.top/gttlpmvodh.html

var a = 1;  let b = 2
来源：http://hz.0kj1m.cn/gtmsrlilub.html

[T18] Swift：字符串插值
来源：http://hz.pycfn.com/gtvkfklcgp.html

"值: \(b)"
来源：http://hz.zhengqikj.top/gtgpejxizg.html

[T19] Swift：可选绑定
来源：http://hz.cdnleiting.top/gtmwpvywfb.html

if let n = opt { print(n) }
来源：http://hz.yj202588.top/gtrgvlsaru.html

[T20] Swift：数组操作
来源：http://hz.jinghuilouyu.cn/gtmjewxjyt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.havefunace.top/gtliiphzhi.html

[T21] Swift：遍历
来源：http://hz.0kj1m.cn/gtmmvorene.html

for x in a { print(x) }
来源：http://hz.xingfuxueyuan.xyz/gtzfhzylsq.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtfjziqark.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.aizwys.cn/gtgjgxuxae.html

[T23] Swift：函数
来源：http://hz.cucudq.cn/gtqngzrnip.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.kuanghao11.cn/gteeunqigo.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtqmwtexzu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gtrclflvkf.html

[T25] Swift：结构体
来源：http://hz.shanyushiyangtech.top/gtixxnozgb.html

struct P { var x: Int }
来源：http://hz.yuxming.cn/gtbvviyxzs.html

[T26] Swift：类与重写
来源：http://hz.zhongyouzk.top/gtnbbprvtc.html

class A: Base { override func f() {} }
来源：http://hz.vqdsnc.cn/gtgoistslb.html

[T27] Swift：错误处理
来源：http://hz.svipenyu.cn/gtotjlaxui.html

do { try f() } catch { print(error) }
来源：http://hz.ppjwa.cn/gtsbipvyay.html

[T28] Swift：枚举
来源：http://hz.chenzaomai.com/gtedkiftzh.html

enum Color { case red, green }
来源：http://hz.meibo888.top/gtrgpiyxfl.html

[T29] Swift：guard 提前返回
来源：http://hz.sufxvd.cn/gtjxyhwdbl.html

guard let x = opt else { return }
来源：http://hz.jinqigfzy.top/gtxytbptqn.html

[T30] Swift：协议
来源：http://hz.nwbrower.top/gtgorplsug.html

protocol Shape { func area() -> Double }
来源：http://hz.sysykeji.top/gtshfdajqk.html

[T31] Lua：Hello World
来源：http://hz.chenjidiqi.icu/gtqkzotulc.html

print("Hello")
来源：http://hz.xuanzx.com/gtwtbzsxes.html

[T32] Lua：局部变量
来源：http://hz.ydzc1.top/gtcybwghuy.html

local a = 1
来源：http://hz.xuanzx.com/gtspqhzcle.html

[T33] Lua：表（数组）
来源：http://hz.cheryme.top/gtorvfnzwb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jyoumei.cn/gtnwphumac.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gtprhlyrfz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zdqjudy.top/gtahauishm.html

[T35] Lua：字典表
来源：http://hz.svipenyu.cn/gtzljhegfj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtzqwbcpny.html

[T36] Lua：函数
来源：http://hz.hongshengwenyu.top/gtyzbnawtz.html

function add(a, b) return a + b end
来源：http://hz.shangyingyoupin.top/gtwuhaptox.html

[T37] Lua：字符串拼接
来源：http://hz.pycfn.com/gtnssqzihu.html

"a" .. "b"
来源：http://hz.zdqjudy.top/gtagwzggvh.html

[T38] Lua：条件
来源：http://hz.sysykeji.top/gtppfmhiwe.html

if x > 0 then print("正") end
来源：http://hz.ywan-chungtsiang.top/gtbkwppmep.html


<!-- 参考信息 -->