代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3qxgnjvwk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3uzwpwbdy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wrnrvwyi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bgkztwaf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ythoxedn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cwdqwgok.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3byakzvsa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3nlxrqhhu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uidagshq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nrjqnhcu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3emrkcmpy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sjhqviye.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xrpsycwp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hmfvrxre.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mjhdvghf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jrxtmqnk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ydddfqtl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jseoklci.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ltsqdtkz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nfviwlwn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lpvrtkiz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3olfryhzk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jjvnxfas.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jikcquem.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3tzvkxgme.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3btfmqiyl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dnrenffz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3grjhukcq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vwydtebz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qzwoqxdf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3notopqlb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3raoivydu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ptokpcru.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pfittxgk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3sgrriftw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wesvaycn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ooemtiiw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zryuxdya.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3monsnpxl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3iizpxixf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bktbchcw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mbiawash.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wbijefaa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3siqdvlbf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rxzkcxfb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nsoivdol.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3eypvuqtp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3yukvmdzs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3caoeejol.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lxcuuzpi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sawthlyz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ykyfqzfl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3cjuenylw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ntvvefht.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xgdproaj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zyxfthjr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3cptdflbu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vrriaenn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jceokssh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ubhzeqhh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3wobtvphv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3npwqfzvq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mikosscj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jdscrcnj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gnwiqhrg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rohjapmw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xgxnjsqb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ssasviyn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vcuybeaa.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ctzutsjs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ldyaxvmi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3glujvrgn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mglayivx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kincgzwm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xvvqucaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnyzdjfn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3xhhbjflr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgndffmn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yoahkpxf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3innshyzx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3spqzrvlx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xyrfuilr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3aupddxzf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ejtrqnjm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3acfyaeos.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lziedtqo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gudbxsim.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rrhwqvgg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3udwnunzw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hzcfcwxq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pkqaypur.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lraceogo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rclrxubf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rknqgfjr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3sqbwvzyk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jxpalovg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jbudcrhe.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zvsydoda.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cpwfzaej.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbcpzxtw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rdoqfupx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qxqxtubr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kqbafkff.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmxbtppd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qyqotfik.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hlayubzb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hayfwjal.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qrcfuckc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cbidkmjp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aghuhfzc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hdshohbv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fbswkmvl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odewyeuv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3prccfpic.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uhgftpls.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wwwvgsbb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3cpsidkrl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3cjutnors.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wqjauexi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jgvncocv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pfgexhis.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3olktxelz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rmprqeue.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zexuuhtf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xxarpawu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wmpmxsyo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3risllioz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yyfawanl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3arxelzyq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ynxbmnlf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vjpxtmbb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hacddmuy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hzitfcze.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jdxnmsqp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yymymmwy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3guzfomyl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3oqwpresb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mcbbsozz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3juanblgv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mypjffex.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zesnydvq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ioyqsqrp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zsdtyjcs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3icnrorws.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xgkhsbjy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxvvrgbf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vablzowj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ezkuatsf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rcljbwjj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wpuzupxz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bsjwviih.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzjxmlni.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wyccfsum.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pzoxfitc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qucubgyb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ysqukwne.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3osfbnmji.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nvvosrky.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ckdgzqlf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jzhwvylv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3oeskbjmc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mettgxdd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yvujwvgr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3suomariq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcvenbpv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lglmjgyf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvvbgenc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xrojwnld.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ahgsenpd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vcnmcufw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hmgxckmt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hkhdkxrt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lnnjwdql.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ikphljdp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ipfmajrq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3adtcdpix.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wkyaujup.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzxuxmyv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cuwhsnnl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mfrdhbgn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iuanqvsa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjjoddti.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lklrodkj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3izdufrsu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uztkizvk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rvmtgcal.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gwselssg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rbrujxal.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ranxipys.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lrunmhst.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vrsuwuuy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ezryquyb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3acnrzbxx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zzdouqio.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3taaqaniu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cssonigr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hcytprul.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qstrbmhm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cwehcssp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xisnmnjn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jktatraz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jlucrjcq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bjknyogt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3slplbufn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uonaiznm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etmqloon.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wmlnwasv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpyhzgxt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xqmtiqqs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ckrshsmn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ldjahyvt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ezgcoweb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3akseerhu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hsmljjcv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fljbfztt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3uuflsleu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jrucklhc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hprmawyf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gxvxrpub.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ixdaqkpn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zsznwfjz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hrqioule.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rolvmfya.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dhbahilr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fdpyuvwr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fyzpkfxi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3usgybezm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3sntvgsjd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uppxngfo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3pdppnfuk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mvbjxqqx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bqffuhqw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3aisvmqiv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vchjcrdy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fyyobtjm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fwjhhlwv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hlwbfeod.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qukdjjna.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aegaqwcn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jvqwtcmq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aahdfnsz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3cjchmqjp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zjvmyeak.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3bfbjshif.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3cochnmfc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fwsrsptl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ioylqoto.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvpiohz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ikvempbl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zparhtum.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gsqndyeu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vefnbqyp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zekzhzcd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sernopws.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3usbikarf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbtwftyc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rgqpvozf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qjqcaugw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3muglmvgq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3drvzxzqu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uzdkzdwm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ppjhowqq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ldhwiaad.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dluotwcg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ruhpaodg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gqsgtjis.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3oklzltqp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mhelqurt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mwmkzeyx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wzfwieiy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hsvielkm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixgddoak.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hzytxffr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fiqvailu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mxepdrrs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3aqvmfgni.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cuvghgfl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ujgjvhun.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gbdhujst.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3leuqsfyu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tkhnveuj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ipbprlwg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rjmvyqyv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3venarlvs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jkcdpyue.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wmlbuwna.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ebnwnfzd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3lljcsghk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rnvzhere.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kbgfaxil.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3apfmzwpm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aqqinhve.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zdgyjjti.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cplcpgut.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rczeqasm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3nlfqcdta.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xksyfmho.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3raxiozhq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3egksmldk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xdlxjnge.html


<!-- 参考信息 -->