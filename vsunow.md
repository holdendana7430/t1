代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gwhvifzm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ljevmpfe.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pzbtewsv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ijpuegxn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cgpogymh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jbzyijep.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kfnjuenv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jnxukwxo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ziejklwe.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3uynrasiu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rebetsuy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hueedihv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3azjqyxrn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3fmhjxfvj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wtfdijfl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3twbutrbh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fcdfyhrq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3enhkhkaz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tviyfuhf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xcjkpizt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kgxvjmqe.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3juzebroa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sotsxmgs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3mbpdgyfo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vfrklyre.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vjsvhtbb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3asbylzhp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jokoyeex.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fiyxrxjq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ysduzwqz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fxmcydoz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ufmrglml.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3otvbbxtp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jebgdbmk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jlkyhfhx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ojrxtdna.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3pbhvpdbh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3muxtlrzy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dvxkhssh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qbodynwp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rwyhrnqx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3koymodvt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vvcoxhvl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zrgiyzec.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sjoadnmb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3cyklruad.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dtgsfyyw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3whzunirc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3weeafcqh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lpztkswp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cgnsfqdg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nngliblz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3uhlgspwf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3drgcgavp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qkjdhcfc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rnhlxgzi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wboavwpc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3migvvyzj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dbcosjgd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hgohjbbk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qnorsvwq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bhohrtwv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3intlehtl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3luudtuec.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zvdmubbl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezoiigju.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aginsblf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tkfkcwew.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dmkmvkuz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3smxebnhu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mnqhruut.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dtfmyoxz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3oyxswqzc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cyruwlsq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3iwbdypmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruyajzhf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gwcvrqel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgsqkqwh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ouxxvopg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3khofiwbb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3imicrlcy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oblwavuh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vtjjbqce.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3klenzjpf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3stzsdkwp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3nnkcqpjp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3neljoyim.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gljzbory.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upopffbr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tfanvyvk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pcomhmov.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bmgzdgfb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ymetwlxb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gcukcivg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lxyudgks.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bxcbcafe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3zhgajsrh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tefiddam.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vpiaxgci.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rfxwkjuj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3oepxgdee.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iaayjfeu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3byderobr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nkpisabo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3twtgsbsy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nhbidqzd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3udmqvcbu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wjbidkuj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ydmuufbj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3slwbdhyy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3emvfqsmg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fyityhwy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mcbkdgab.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nxfdcmfj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ptrxpyrc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3evwblpzm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zlitsepf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xbejwsoh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3anvzkjwp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jevqzhhy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3otpeotmz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3sdyquhml.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3isabgrrb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3aaipfuuo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3trtofrhk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kebqykxt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qhfqerng.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kgzrgjzt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gxuvinwp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mjpoecpz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kzbdhizx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3bxlageio.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vvorricl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gfakykrc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yalfybya.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ckirnbqv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3uzefeifd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xuwaiofu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3imbcgvig.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rywkjdfa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zuqmtzhw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3solnrknn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gfdvzpvl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3udkflufk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mqhybmam.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rwqwejfh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3elvrdtbf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lcwnaema.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nohxlhev.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ecuvxwvi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bslkxahm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kllkdiea.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rzdnpxai.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bwohmzgr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hnsfjohu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zywxqyue.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hnrnckhj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jxmexnog.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3euwmveqm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3skklaejm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hbirknav.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xoqlsior.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fjsqoswa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yioovgez.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3itlchmgu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zcxswvou.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmogruyt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vdgryoxw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cfrozhnz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bdaauerl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3urqcugwp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3efnlscwb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ivoidrce.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zhzoejqg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cudrdirj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsexsjzf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pkhfpket.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjfqiwcw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yvlpklep.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hmytbmic.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fluvovbw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3arfphbvj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gpgejwsh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3cajgzqgr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3urqsunqv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qaksfxlc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cifdtexg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mubjbnhv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lpwfotjs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3apfaejid.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fkksvmgp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3llnsspag.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jdgkwvcg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cfnhqxhi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wqfbzbtf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hpfrwoif.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3enkkuxzj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zlhzonhk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bbfankjt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ppgwwepz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gtopjxqy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fkuhiilm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mgwksbhl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3usdwyzej.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hoqskkjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3posqmnzf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gktdkkug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcjebgoc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gooqksqc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ahxfkakt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lefrjxez.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rriyguvl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nsxzyqfe.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uabplmsn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xjocgnii.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zcpxilbz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3brdgbzjw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cymzoehh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hyqkgmgq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvqyzhqo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vhhbxvjo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kguisacd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vhygbham.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xjsnbrze.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tjyxkcqa.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3worznekn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dttavflv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3eozwqnfv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3obtdrrgh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3laiusegi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bkldgkxk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ygkekdlk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xvwneemr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3itxdunbl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3imedeusa.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pnvydjqg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3oapmaggd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ndygtiop.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ecwzcmfq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yvtndxcv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vmupxrls.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bdgonwmp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bxygrsgz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dzlmyaqm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mnhpemvw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tmhmnqqx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zqgjcptk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3haqtqaiz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lntbwpay.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xcmdvdge.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3bhuxpkns.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hjuqpsyu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ygwiyocl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gdnkbfdx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nolqdwxe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bqdcebpo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3eplfohmh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ncpiwjte.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3opmbzfuq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3scchxftl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yjarybuh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yygpaibn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3daekhoyu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3oorjiwdf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zfnunjdx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3thlwvgcc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wqbzerws.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zupezkqy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bywgmawu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uubqkrgl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3yqgjvdel.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gdzvbgza.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gcwavufw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ozybesmy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3teqkxjcj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3febgoqge.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rtbymnlm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cwsorvmm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gtlgmqjb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zgcdckpr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bozuuyzb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vooigble.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3kbpxemmc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3paqoizee.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pvnxshfw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qzasxeuh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ksyxeqqn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zmsoulzv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wauuihfb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bavnkhes.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zwnpxkqh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3agtwucrz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kofatver.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3njmymfhe.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3onhbmklq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3utwrrrxm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mseqqmqn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3unazpupd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dvdlvhsk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbxubwlc.html


<!-- 参考信息 -->