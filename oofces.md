代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nrsoriux.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2aoyjorsd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mszpsvmn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zlgjyzav.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gspofjep.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2oaqvqucn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hlvosuri.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2lnpefeea.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ybpyatse.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2adwyapqm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kzcvxebe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2akevvoho.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rqxqjxbg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bmjaqrvk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2muvkkiwc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lbldeszk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zcmhsaqv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2oyxcooqd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2awuoxnbv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bezlhvcz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yufxecjw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jxnobmcj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pvwomgaf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2atepgvyc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2nmelqdvl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ywsflrql.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sfivruwh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2miazvtke.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nnsdhrof.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2aeyavzbz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ltjpsefd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sxmfpeul.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ajdgyuvh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfmcgfcf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zrwwokdn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ixbkfmhk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cnogqldw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ossznlcg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wxbotklo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2evltmpng.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lqgmhhle.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sygoqwkz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2gfiizitp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jxjlyyje.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2miwynppo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kgcryvjm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ahtvmpmr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nzcvvtxl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2oxsiqlhs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mtmocodx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ifarnsum.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2eayocnti.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2eibzqnuf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vlvgdvju.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xewkwdxd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kelfeqvx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2otuognsl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2iowffrnm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jjsjbjow.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wwkhlnjj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2aspqbzjm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qdgavhlb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xzoztudi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ciakwumq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2levininu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2opiylcbf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uozaskqc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dpryzanr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2bvjxphmx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fleqoqog.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmmznujc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2iftsyxbj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jqjxtrxq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ixgbvqjy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qfgohzre.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2csgspdjb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2evusbrrr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2iujtaybu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uefdbvur.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bsrbqwhh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2oddabjab.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kjkwvmiw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lwdtcgxm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xeyzaaag.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2soyngrzp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ovplbzrh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2smkfphwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnmrwygr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dipwfkmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnkhajbv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qlatxndc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ubxtkmet.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2usxexiiy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gzqwbvlr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2inlinsaz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vhhibdbx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fkhxdvpx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xszdznuu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dfeocyzj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2boyvjxoj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2uwnrgnug.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oqenwilu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cjuauxnc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2taiucjwh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ijwgywdn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hdncajjm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2biurzrne.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xlfplulk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2sulybowo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fwraxhct.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gdptopsa.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rinqrwsb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ziicizjd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2uyhvimwy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tirrrzov.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lsjkxtgg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lmhmppuw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2evmdzepf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2naaadwra.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pandnahb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2otxzniuj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qktfvjhl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hdrsdyrn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2epfndmqh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fkelktbs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2maaceguy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2osjtaufx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tbqddmgd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2lkalgztq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hpfoyofj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tglppdut.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zvymndgi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2earwkabq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vqawnuws.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2octyqypv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dimdjvbf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lgbejvnb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2snqnsuub.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vzfyabwb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rkrrixot.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lnoljrzo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lclxgsca.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lhnareeh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2eqaskyyr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bzeygish.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2amexwgcn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dggdjkau.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kdvkjrcv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bbyqhyeb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxpxrykw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qvzilexn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zgepjdwj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zfnjcomi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2orouyshk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2obuhgjnv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kvshdpji.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2baqvaycz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wchiofmj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gzlnhttk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ktchheee.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2btmnqueh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2poqijaxt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cxyhtfhi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2inzxyude.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2frtdohnr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xipyccxm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xoenawjb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xrowpplt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xsfbuban.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cohciwyd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wmgcgrbd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2igwqvelm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2aebqaork.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mjssekrf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2reerobgx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmgtlefz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ybjkdova.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ggxxzjdx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gsrbwqaf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hacubrak.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2fymvjdej.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kcadqjky.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jjcuxnwl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wloxlits.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2eahoolts.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hoyeyhou.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2soixxhbu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ysiwhjco.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gpihyfki.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2frgxysjh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvwzbyqj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ofhvlasc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hxuoetyw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cqsnalvv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ffmurogn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mujdlluc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ygjbavww.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2muzvnoee.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2eqfzgwyy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2zofgfoue.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsnbljgm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bkwqeyrk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yoeibizm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gqbxfwkh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fkkukyzw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oowlotjq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2imfohxls.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2osjfucte.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kfjnmmqs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rutoplej.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ryxrnlvc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wgifogsc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fgqyxwmb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fltrgeic.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ytaruega.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yxfpbtbd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rbumgvht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdgsfbry.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hoausubi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2seckjbsx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ycdozlkc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ogjfkqty.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cbmahjxh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gfwuhjmp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mruakhkz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jhsdnfpd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ucfyuhyw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gkkczebu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jrgvrxwi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lgjtslkl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dgqufpws.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bkhsbqid.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uhznwfjc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2loimuvjg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2aghvnsvt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jsoenxqj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fycjdpgv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2llxljppr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2flnuzfdf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uvvjjpgr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2uxgzxlkw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ovelrbwq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ugcciese.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvgzymo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zycwawjb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2peeodmyx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2swrxjowj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xiuempkn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ixxadyqw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fzkpoirk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wbnajpjq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lxozwhok.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2shpakhcq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2plrrzdir.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2paxcmrii.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2atahfvae.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kupkobbq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zfnbqold.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2glcrulxl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wbdrktfj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hgprozkh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pidozabv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wljzhgad.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2kpecbcrv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mskumdtb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2evephgxn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fvfkchst.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tojbhwkg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fruicowg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2astmuqlf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yauiwmdd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zjjmwmao.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dmigpgqg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2atrrbdtn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qzmrwuki.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tqoqjwos.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ryilukrt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ksoqfwfk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jzcwuzxr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pwnahuav.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bzgclgap.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2skdcwzsn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tcqqrqen.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2chewnbxz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yzfdpldm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mcidgsjj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2roxqmqym.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2yyqmuuac.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lbqszfox.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wckqoncd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2smvesypo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ggobkofm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wpfelnsa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ctrqwlqv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lnatowho.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2kvipbrsq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2autdejyd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2enmwaslx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qsujmgds.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xrrgcfbg.html


<!-- 参考信息 -->