代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xfucjfgn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wcngbjje.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zpekhnub.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3grbdmycy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mudfpgjz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zdswqrxc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qkrmgnep.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3mmmhngvt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gtsjvrlt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xlxgtlhr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3krwfnhdk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ejdyqtbg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bbhhmywl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kxtceeuv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lekmuprh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tfboungj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lkwdrvle.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mqpvxlee.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rbyujkty.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tpsbegoq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dhwislgj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ngcowont.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vwvsuwxp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hhkdizon.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zcvuopbn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzlcsmcd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qcbvkkbb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fqvogngi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mqwwpjzg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jdpdidyl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mjkjnchk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mtmpucch.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3urnuftze.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mfjhqwzi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lubqbmmr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3schhshse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3arzmuyiy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mqgvzciv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3eztoayum.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mioggazb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mopuxate.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqxqmgal.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sirdehtl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ucsbfkyc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3botcyzsm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qipmqrqk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3otgpwdzl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ntilwhaf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dsevwdxs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cilgjntl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gmfoivxo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rbqqitcl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tfocjlij.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3mlytqadt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3lggzffgj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3whuacbss.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xhuhqyow.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yueasezj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ezvgbjcb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sylqfdxj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3knxzfjqk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qqqceukn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3afylmesq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3apydjjjz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3dhgsawxw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ucbmivqq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3whouqpbj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zyfgevpb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3yprhwogb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wsjmmpoh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uckcyilg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3tmbycesx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3glgyxcje.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yukfxdwa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wmnrbkeo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pvbhhboo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wpcphzqa.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wynnpfkq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ytdpdabw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smhzwddc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qzkxerae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfbywwtu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qjawlbax.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3omctoxhd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mjrnhyhg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mktpxney.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3oofguzck.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ltpjjnbw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pnwvqscb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rjbebtca.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3enthfbrz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3buqqfqfn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tuewmvbi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nejzospv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3mnmfkyjw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3syjijoik.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3sryvpmis.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dvxoxpes.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3soadzyqh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rihvrweg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rmmwgdvk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3oihlvoys.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nvsijjtc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kbgyhqjg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qfgqttbs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lvcpuqcs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gxyyngdl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hqrtmkyw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jmrrqzuq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xjzydkce.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ryagutnc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nqcuybca.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wfibvzgt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3drpntsir.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zvolimaf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nzfsofqr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3xmavylpn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dlozlhqj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3myuaxxin.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rzlkcjuz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3aretlqve.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ipqfsglp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xmrrejuk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3acdtqxum.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wtbxnmcb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fchsuuez.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bybwfyfl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3astlkcfi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mpjklbiz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vawfbwvi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qwckztia.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3crltjkbp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3mptxqpuc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qkahzlav.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ssvbpclv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3myeclmmk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xtfxvvwq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kaejujqj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lqoebmcb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zjmfbfmk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gazgvwut.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jidmetru.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gqfarrwa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vmvjhtmh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gfskcupx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3uaxkrgxg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ocyzvcta.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gljpigql.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xfmjpcve.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvweaxti.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vsakawnv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3iqfxzveu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jzcuklym.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nlsinptc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ftubyolf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gmtwwuji.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tenqxijv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fgbqagof.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lyzvgkhe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zphzfnok.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ebjzhppu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gdfcogqx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hggqctdg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dwpecnoc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3pbzzznan.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3uitzynra.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xrdiiadk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zunqyjsz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zltjnoef.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uqrqievy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wdzrspcq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ooqkleud.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hciatfgr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3adsarwox.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ipebhydk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fuivuhjl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fqkslqsq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vhuswrxy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ocsvhhra.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnfvhvr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3blzxrfks.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xpyrgucw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mxvgjfcq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kkcmxotv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dvtopjin.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3thibncqb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yaiqeqxl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pbjkptbp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3obfvyozi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3agnryilc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gmcwzvrn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bfopqalw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzivhrkg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xghrjdnx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xyxhfbja.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vlugokda.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zubrljfj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3sswmyrlc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vkpfuqad.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3offsgrde.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdorbbgf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3baqmijty.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dmohudve.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wivrtfoh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fggbipsc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ncxslrai.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xtmyifdj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pxbhignh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wqmihovz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmwwdnoo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xslxxjne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwrwxwqg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zfissxqn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dwtbjgut.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ixpnumuh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wffyrdey.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ohvlgwkz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zmajunqy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pmxbbmlw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lwuijile.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3unictlie.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rgggbcki.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tkcengxp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mynholpn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aetnexgz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dujowjtp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hymqcmwi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wyjxuwnj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvyhzpzq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hzqcsban.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gwinsbrz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rtvelrsw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jpyeikss.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ojrifqch.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3toyrdxzy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oegljstd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3raigjziz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yfcmwxeu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3udpguidc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hsphiagz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vcrzbsvw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3czthcvim.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gvinaocg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bkytxuta.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jbocixxi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fcwbbeiw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sspjbqci.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rpbyvzjj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zmzmeuav.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vduzhnnj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ojuikntf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3obrnfnun.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3veflvure.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3havrmzwj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bhyhqvjg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pxyjyndy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjdcwykp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gvwcqzjx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3camkdkst.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bbqxuumv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mjrjwurr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mzbsfblt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dwcgsovn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zhnablct.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3brauedas.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vxkuqjju.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xhrtethu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bkoarkzg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mnsaubxy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ruwgxjzz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zlcqwbva.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ttueneax.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3omqvpaav.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zhnciawt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3uegxruhf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wuhfwjcg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vfnwgqts.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jgcsspok.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wnvbypql.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3oscpqatv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hyyxpcrx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mgqbgmuc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zwcabwnz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zbthdaks.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gtnziqws.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zpndsunj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3frskolyp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cwznxcda.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fmayjekt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3swqfryux.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ixzynbhz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3cyhyysei.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tzmnjixz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qroykmul.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zlfcoagh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zlnoidtm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dpxutrdt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wdlrpfgg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wmspfifp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yjzabskx.html


<!-- 参考信息 -->