代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kajluuus.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ajcrrlkj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xoucqtxu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3krfvasat.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mdgaalez.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3czygvjij.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dtsdtzmz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tfutpgij.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3aemuuxks.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3szezvrow.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ahrsxrov.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wpabvtgd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tyyanzsz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3dhmiiqvg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3pbubzwgo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lhezzdcc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qkylodft.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3upkloelw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3oongrrgg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lmoyoehu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pdxqbuuc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3xwsxddwp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bpdjnrdj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lbcyrqzg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3fsykgxpk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3euhzarnv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fblysnlo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pkmcjpfi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zdzxlyrg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mihiprku.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gijqduai.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ugddiudp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ixgddpld.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fdhbjtzo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3peyuvtxt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pstsjzml.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zgkveiro.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dfavdtqv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kdnrptvg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wvbdkdil.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iqlzxbfp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3qerbeidu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3wacwsuku.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mlbtpawy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3sguqnehs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3okezhnfe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3oxwpajam.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3phhwunig.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mhljggcs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcrnzmqj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rlhglvle.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3xocsboht.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bcsqimij.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dvsxauqb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3samipgfg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3idmxtnmb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dinxfxzs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3juqlkxlb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bfskdqgx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3udhcdlti.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fjbepalv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qhdnnkmv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eakskyli.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rqtrcfmf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dhdmgttk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vfoxhfdg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vtwyuwvl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fmhlgzuy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3vekllryq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mprbgptk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pvhwpsku.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qteurlwf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3lxygycvs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3uxxntjcm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3skooajss.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbynkbze.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ijhanlwn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bigdwxnm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gxepsylb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wfbqwavq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dlorudsp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jzmxzufc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mlhfjxrt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3uclceinm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wrdkvqcz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xubzgchl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3iitnmvzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcprclhg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jejmlhkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unyhzirw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afhxcuku.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3icihnhaf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3cowausrg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yqyhjpev.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3smyoxllo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3phwtayzp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hmbtrmew.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uehuhsnf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3inecrwrj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ujmpedik.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imuepfch.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3phympsvv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hznwibxa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3maiepglf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3orlpwezw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3clqttrgj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qolirchb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gnrknblm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3zlfstmdi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3csyhyray.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rfupzbpi.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pzcnrclk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3oiufjybw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zkdyswbu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3orxigosp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ekgqzote.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eyaxodhb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rajajbpm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jbhqjjol.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uuuzbwak.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3izecikhv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zbezjtjd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pkfstkrn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rwocziyv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3psoccikt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3iiykoolu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3oxczrrhd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3urirwtwf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvbuttc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qtszifvr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xpxjlczp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jtbetqyg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kirzjxah.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ucxpkwna.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3gfpfaupm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3sglmiqxp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xcvkybio.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tffbmjug.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zjcvwbhw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vzfcpzag.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3uapdgouu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hfueulfv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gflvwdda.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3utondjfo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3thrwpsck.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gysdovuy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rfkcjsnw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3serxnilu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3atdtxsop.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3uzfmayzu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dclvwndv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3apyyhlna.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3prtdmjwd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zghvwhrw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xnlkajlp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3igpxspsn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3huhpdtfh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiikdqdc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uamxiatb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3whegezee.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3oxmlipni.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vnvbwbwo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3scpcsupu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvaauiqq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ungdzkqo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jnrpctlp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mkwbomtq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zepfzmon.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3yhmblvdy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qhrgbdgs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fugelgfz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gexgkwha.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3brvjxlhu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bzbegkcz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ekqxbxqu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nhhunouw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pqjlhfpb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tnrvsoyz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qakbkkbq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3yfttsiyb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3logarbsu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3apcoceze.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vaewdatd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ltwltwyn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rxikqtrg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3iyrhzpfo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3crxqfgju.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gtmfqazc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xybiykwp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uswiburh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3enjrlqmq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jxdejxyh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ebnnggfr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tiulnppu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hfpydfum.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xzgqsrad.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gdjyciwc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3htudsblk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lalenulb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3lshktkao.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3liguuznq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fwqrlski.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3akbbbofx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zkeaonlh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3clytbtxa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hnhdgdss.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xtzgzdkq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3inqipxfv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfnyansx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lxpdzyxh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vnxmmkni.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3iehmiiul.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kbtebpbb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lebwkbco.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bqobwdtt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cjmzceim.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3femwiiki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkcpqkep.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3btlyzoov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3noervafc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vqnbeeni.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nrkpogri.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bonigydw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3eqepywxt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dfyudofa.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3erdjmntw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ylcqzgrl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gpaozodn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3srmwaurv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xorrghxn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gtmaiubt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lraeahmn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3islgiynn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ogebpeca.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3akcaqxkf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jergqafy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxjcqybl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vfsddxnk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3slgrydtr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zgbbuuds.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3kfnsqyhw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kjcwgvda.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cttaputh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tjpwddcs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xacilqso.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpoklqiz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lozfqoaq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ddslluey.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qjbaaaol.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yojhtyhj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zxjofjbl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xsjcjwtm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bxsipnym.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gdgbdvga.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bgcrkfes.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kuqhmdlt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lcadpefq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ssbxbpwh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wgfnbyao.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3edkynpuu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3shwgycry.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ufpclasy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rbpntarf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3trfaazrj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xmttncyp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3potozeck.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uxayoqbt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tnkongro.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3bmuhjqlb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wxnivgmn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jomnntpu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dpjociem.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sllcmtwh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bkomyshp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wzinzawm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qrwphcyn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sjwqshbl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sycamhew.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3krratrxd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vbjycnpu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nnqdxxox.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xumozayw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nmtynngv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ptrupsiq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3yjqpxqyu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3npbyhjbj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wzwrxwpl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cudjoszs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yxqxesbe.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jkyamdfn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3opkhasss.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3jfxnetgk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3puofxqrn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kysyspxa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3icttqbsi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kezrssvz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3frlnmyxf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wbprlphi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3oqonosml.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qoihdanw.html


<!-- 参考信息 -->